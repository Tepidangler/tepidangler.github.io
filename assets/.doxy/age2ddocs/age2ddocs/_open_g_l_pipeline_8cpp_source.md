

# File OpenGLPipeline.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Private**](dir_70227f149653e1f1d3b9a02604511f36.md) **>** [**OpenGLPipeline.cpp**](_open_g_l_pipeline_8cpp.md)

[Go to the documentation of this file](_open_g_l_pipeline_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Platform/OpenGL/Public/OpenGLPipeline.h"
#include "Render/Public/RenderCommand.h"
#include "Assets/Public/AssetManager.h"
#include <glm/glm.hpp>

#include "App.h"
#include "Debug/Public/Instrumentor.h"
namespace AGE
{
    extern std::filesystem::path g_EditorAssetPath;

    OpenGLPipeline::OpenGLPipeline()
    {
    }
    OpenGLPipeline::~OpenGLPipeline()
    {
        AGE_PROFILE_FUNCTION();

        delete[] m_Data.QuadVertexBufferBase;
        delete[] m_Data.CircleVertexBufferBase;
        delete[] m_Data.LineVertexBufferBase;
        delete[] m_Data.TextVertexBufferBase;
    }
    void OpenGLPipeline::Init()
    {
        //2D Init

        CoreLogger::Info("Initializing OpenGL Pipeline");
        m_Data.CameraUniformBuffer = UniformBuffer::Create(sizeof(Renderer2DData::CameraData), 0);

        m_Data.QuadVertexArray = VertexArray::Create();

        m_Data.VertexBuffers["Quad"] = VertexBuffer::Create(m_Data.MaxVertices * sizeof(Vertex));
        m_Data.VertexBuffers["Quad"]->SetLayout({
            { ShaderDataType::Float3, "a_Position" },
            { ShaderDataType::Float2, "a_TexCoord" },
            { ShaderDataType::Float4, "a_Color"},
            { ShaderDataType::Float, "a_TextureID"},
            { ShaderDataType::Float, "a_TilingFactor"},
            { ShaderDataType::Int, "a_EntityID"}

            });

        m_Data.QuadVertexArray->AddVertexBuffer(m_Data.VertexBuffers["Quad"]);

        m_Data.QuadVertexBufferBase = new Vertex[m_Data.MaxVertices];


        uint32_t Offset = 0;

        uint32_t* PrimIndices = new uint32_t[m_Data.MaxIndexCount];
        for (uint32_t i = 0; i < m_Data.MaxIndexCount; i += 6)
        {
            //Front
            PrimIndices[i + 0] = Offset + 0;
            PrimIndices[i + 1] = Offset + 1;
            PrimIndices[i + 2] = Offset + 2;

            PrimIndices[i + 3] = Offset + 2;
            PrimIndices[i + 4] = Offset + 3;
            PrimIndices[i + 5] = Offset + 0;

            Offset += 4;
        }

        Ref<IndexBuffer> PrimIB;
        PrimIB = IndexBuffer::Create(PrimIndices, m_Data.MaxIndexCount);
        m_Data.QuadVertexArray->SetIndexBuffer(PrimIB);
        delete[] PrimIndices;

        m_Data.CircleVertexArray = VertexArray::Create();
        m_Data.VertexBuffers["Circle"] = VertexBuffer::Create(m_Data.MaxVertices * sizeof(CircleVertex));
        m_Data.VertexBuffers["Circle"]->SetLayout({
            { ShaderDataType::Float3, "a_WorldPosition" },
            { ShaderDataType::Float3, "a_LocalPosition" },
            { ShaderDataType::Float4, "a_Color"},
            { ShaderDataType::Float, "a_Thickness"},
            { ShaderDataType::Float, "a_Fade"},
            { ShaderDataType::Int, "a_EntityID"}

            });

        m_Data.CircleVertexArray->AddVertexBuffer(m_Data.VertexBuffers["Circle"]);
        m_Data.CircleVertexArray->SetIndexBuffer(PrimIB);

        m_Data.CircleVertexBufferBase = new CircleVertex[m_Data.MaxVertices];

        m_Data.LineVertexArray = VertexArray::Create();
        m_Data.VertexBuffers["Line"] = VertexBuffer::Create(m_Data.MaxVertices * sizeof(LineVertex));
        m_Data.VertexBuffers["Line"]->SetLayout({
            { ShaderDataType::Float3, "a_Position" },
            { ShaderDataType::Float4, "a_Color"},
            { ShaderDataType::Int, "a_EntityID"}

            });

        m_Data.LineVertexArray->AddVertexBuffer(m_Data.VertexBuffers["Line"]);
        m_Data.LineVertexArray->SetIndexBuffer(PrimIB);

        m_Data.LineVertexBufferBase = new LineVertex[m_Data.MaxVertices];

        m_Data.TextVertexArray = VertexArray::Create();

        m_Data.VertexBuffers["Text"] = VertexBuffer::Create(m_Data.MaxVertices * sizeof(TextVertex));
        m_Data.VertexBuffers["Text"]->SetLayout({
            {ShaderDataType::Float3, "a_Position"},
            {ShaderDataType::Float4, "a_Color"},
            {ShaderDataType::Float2, "a_TexCoord"},
            {ShaderDataType::Float, "a_TexID"},
            {ShaderDataType::Int, "a_EntityID"}

            });

        m_Data.TextVertexArray->AddVertexBuffer(m_Data.VertexBuffers["Text"]);
        m_Data.TextVertexArray->SetIndexBuffer(PrimIB);
        m_Data.TextVertexBufferBase = new TextVertex[m_Data.MaxVertices];

        m_Data.TileVertexArray = VertexArray::Create();

        m_Data.VertexBuffers["Tilemap"] = VertexBuffer::Create(m_Data.MaxVertices * sizeof(TilemapVertex));
        m_Data.VertexBuffers["Tilemap"]->SetLayout(
        {
            {ShaderDataType::Float3, "a_Position"},
            {ShaderDataType::Float4, "a_Color"},
            {ShaderDataType::Float2, "a_UV"},
            {ShaderDataType::UInt, "a_TilesetID"},
            {ShaderDataType::Int, "a_EntityID"},
        });
        m_Data.TileVertexArray->AddVertexBuffer(m_Data.VertexBuffers["Tilemap"]);
        m_Data.TileVertexBufferBase = new TilemapVertex[m_Data.MaxVertices];

        m_Data.TileVertexArray->SetIndexBuffer(PrimIB);
        GenerateDefaultTextures();

#ifdef __clang__
        int32_t Samplers[32];
        int32_t TSSamplers[32];
#else
        int32_t Samplers[m_Data.MaxTextureSlots];
        int32_t TSSamplers[m_Data.MaxTextureSlots];
#endif
        for (int i = 0; i < m_Data.MaxTextureSlots; i++)
        {
            Samplers[i] = i;
            TSSamplers[i] = i;
        }
        AppConfig& AppConfigRef = App::Get().GetAppConfig();
        AssetManager::Get().LoadShader(AppConfigRef.EditorAssetPath.string() +"Shaders/GLSL/Vertex/QuadShader.glsl");
        AssetManager::Get().LoadShader(AppConfigRef.EditorAssetPath.string() +"Shaders/GLSL/Vertex/CircleShader.glsl");
        AssetManager::Get().LoadShader(AppConfigRef.EditorAssetPath.string() +"Shaders/GLSL/Vertex/LineShader.glsl");
        AssetManager::Get().LoadShader(AppConfigRef.EditorAssetPath.string() +"Shaders/GLSL/Vertex/TextShader.glsl");
        AssetManager::Get().LoadShader(AppConfigRef.EditorAssetPath.string() +"Shaders/GLSL/Vertex/TileShader.glsl");

        m_Data.QuadShader = AssetManager::Get().GetShader("QuadShader");
        m_Data.CircleShader = AssetManager::Get().GetShader("CircleShader");
        m_Data.LineShader = AssetManager::Get().GetShader("LineShader");
        m_Data.TextShader = AssetManager::Get().GetShader("TextShader");
        m_Data.TileShader = AssetManager::Get().GetShader("TileShader");
        m_Data.QuadShader->SetInt("u_Textures", 0, Samplers, m_Data.MaxTextureSlots);
        m_Data.TileShader->SetInt("u_Tilesets", 0, TSSamplers, m_Data.MaxTextureSlots);


        m_Data.TextureSlots[0] = m_Data.WhiteTexture;
        m_Data.FontAtlasTextures[0] = AGEFont::GetDefault()->GetAtlasTexture();


        m_Data.QuadVertexPositions[0] = { .5f, .5f, 0.f, 1.f };
        m_Data.QuadVertexPositions[1] = { .5f, -.5f, 0.f, 1.f };
        m_Data.QuadVertexPositions[2] = { -.5f, -.5f, 0.f, 1.f };
        m_Data.QuadVertexPositions[3] = { -.5f, .5f, 0.f, 1.f };

        m_Data.TileVertexPositions[0] = { .5f, .5f, 0.f, 1.f };
        m_Data.TileVertexPositions[1] = { .5f, -.5f, 0.f, 1.f };
        m_Data.TileVertexPositions[2] = { -.5f, -.5f, 0.f, 1.f };
        m_Data.TileVertexPositions[3] = { -.5f, -.5f, 0.f, 1.f };
        m_Data.TileVertexPositions[4] = { .5f, .5f, 0.f, 1.f };
        m_Data.TileVertexPositions[5] = { -.5f, .5f, 0.f, 1.f };
    }
    void OpenGLPipeline::StartBatch2D()
    {
        m_Data.QuadIndexCount = 0;
        m_Data.QuadVertexBufferPtr = m_Data.QuadVertexBufferBase;

        m_Data.CircleIndexCount = 0;
        m_Data.CircleVertexBufferPtr = m_Data.CircleVertexBufferBase;

        m_Data.LineVertexCount = 0;
        m_Data.LineVertexBufferPtr = m_Data.LineVertexBufferBase;

        m_Data.TextIndexCount = 0;
        m_Data.TextVertexBufferPtr = m_Data.TextVertexBufferBase;

        m_Data.TileIndexCount = 0;
        m_Data.TileVertexCount = 0;
        m_Data.TileVertexBufferPtr = m_Data.TileVertexBufferBase;

        m_Data.TextureSlotIndex = 1;
        m_Data.AtlusSlotIndex = 1;
        m_Data.TilesetSlotIndex = 0;
    }
    void OpenGLPipeline::NextBatch2D()
    {
        Flush2D();
        StartBatch2D();
    }
    void OpenGLPipeline::Flush2D()
    {
        if (m_Data.QuadIndexCount)
        {
            uint32_t DataSize = (uint32_t)((uint8_t*)m_Data.QuadVertexBufferPtr - (uint8_t*)m_Data.QuadVertexBufferBase);
            m_Data.VertexBuffers["Quad"]->AddDataToBuffer(m_Data.QuadVertexBufferBase, DataSize);

            for (uint32_t i = 0; i < m_Data.TextureSlotIndex; i++)
            {
                if (m_Data.TextureSlots[i])
                {
                    m_Data.TextureSlots[i]->Bind(i);
                }
            }

            m_Data.QuadShader->Bind();
            RenderCommand::DrawIndexed(m_Data.QuadVertexArray, m_Data.QuadIndexCount);
            m_Data.Stats.DrawCalls++;
        }

        if (m_Data.CircleIndexCount)
        {
            uint32_t DataSize = (uint32_t)((uint8_t*)m_Data.CircleVertexBufferPtr - (uint8_t*)m_Data.CircleVertexBufferBase);
            m_Data.VertexBuffers["Circle"]->AddDataToBuffer(m_Data.CircleVertexBufferBase, DataSize);

            m_Data.CircleShader->Bind();
            RenderCommand::DrawIndexed(m_Data.CircleVertexArray, m_Data.CircleIndexCount);
            m_Data.Stats.DrawCalls++;
        }

        if (m_Data.LineVertexCount)
        {
            uint32_t DataSize = (uint32_t)((uint8_t*)m_Data.LineVertexBufferPtr - (uint8_t*)m_Data.LineVertexBufferBase);
            m_Data.VertexBuffers["Line"]->AddDataToBuffer(m_Data.LineVertexBufferBase, DataSize);

            m_Data.LineShader->Bind();
            RenderCommand::SetLineWidth(m_Data.LineWidth);
            RenderCommand::DrawLines(m_Data.LineVertexArray, m_Data.LineVertexCount);
            m_Data.Stats.DrawCalls++;
        }

        if (m_Data.TextIndexCount)
        {
            uint32_t DataSize = (uint32_t)((uint8_t*)m_Data.TextVertexBufferPtr - (uint8_t*)m_Data.TextVertexBufferBase);
            m_Data.VertexBuffers["Text"]->AddDataToBuffer(m_Data.TextVertexBufferBase, DataSize);

            //[[maybe_unused]] auto Buffer = m_Data.TextVertexBufferBase;
            for (size_t i = 0; i < m_Data.FontAtlasTextures.size(); i++)
            {
                if (m_Data.FontAtlasTextures[i])
                {
                    m_Data.FontAtlasTextures[i]->Bind((uint32_t)i);
                }

            }

            m_Data.TextShader->Bind();
            RenderCommand::SetLineWidth(m_Data.LineWidth);
            RenderCommand::DrawIndexed(m_Data.TextVertexArray, m_Data.TextIndexCount);
            m_Data.Stats.DrawCalls++;
        }
        if (m_Data.TileVertexCount)
        {
            auto DataSize = (uint32_t)((uint8_t*)m_Data.TileVertexBufferPtr - (uint8_t*)m_Data.TileVertexBufferBase);

            m_Data.VertexBuffers["Tilemap"]->AddDataToBuffer(m_Data.TileVertexBufferBase, DataSize);
            uint32_t texindex = 0;

            for (auto t : m_Data.TileSetTextures)
            {
                if (t)
                {
                    t->Bind(texindex);
                }
                texindex++;

            }
            m_Data.TileShader->Bind();
            m_Data.CurrentTilemap->BindData();
            RenderCommand::DrawArray(m_Data.TileVertexArray, m_Data.TileVertexCount);
            m_Data.Stats.DrawCalls++;
        }
    }

    Renderer2DData& OpenGLPipeline::GetData()
    {
        return m_Data;
    }
    void OpenGLPipeline::ResetStats()
    {
        memset(&m_Data.Stats, 0, sizeof(Statistics));
    }
    Statistics& OpenGLPipeline::GetStats()
    {
        return m_Data.Stats;
    }

    void OpenGLPipeline::GenerateDefaultTextures()
    {
        uint32_t WhiteTexData = 0xffffffff;
        m_Data.WhiteTexture = Texture2D::Create(TextureSpecification());
        m_Data.WhiteTexture->SetData(&WhiteTexData, sizeof(uint32_t));
    }

    template<>
    OpenGLPipeline* Pipeline::As()
    {
        return (OpenGLPipeline*)this;
    }
}
```


