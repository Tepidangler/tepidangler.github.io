

# File Pipeline.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Public**](dir_68ba7e1260de504efb39109a85960357.md) **>** [**Pipeline.h**](_pipeline_8h.md)

[Go to the documentation of this file](_pipeline_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Structs/Public/DataStructures.h"
#include "Render/Public/RenderBuffer.h"
#include "Texture/Public/Texture.h"
#include "Render/Public/Shader.h"
#include "Render/Public/VertexArray.h"


namespace AGE
{
    struct Renderer2DData
    {
        static const uint32_t MaxQuadCount = 20000;
        static const uint32_t MaxVertices = MaxQuadCount * 4;
        static const uint32_t MaxIndexCount = MaxQuadCount * 6;
        static const uint32_t MaxTextureSlots = 32;

        Ref<VertexArray> QuadVertexArray = nullptr;
        Ref<Shader> QuadShader = nullptr;
        Ref<Texture2D> WhiteTexture = nullptr;
        ShaderLibrary Library;

        uint32_t QuadIndexCount = 0;
        Vertex* QuadVertexBufferBase = nullptr;
        Vertex* QuadVertexBufferPtr = nullptr;

        Ref<VertexArray> CircleVertexArray = nullptr;
        Ref<Shader> CircleShader = nullptr;

        uint32_t CircleIndexCount = 0;
        CircleVertex* CircleVertexBufferBase = nullptr;
        CircleVertex* CircleVertexBufferPtr = nullptr;


        Ref<VertexArray> LineVertexArray;
        Ref<Shader> LineShader;

        uint32_t LineVertexCount = 0;
        LineVertex* LineVertexBufferBase = nullptr;
        LineVertex* LineVertexBufferPtr = nullptr;
        float LineWidth = 2.f;

        Ref<VertexArray> TextVertexArray;
        Ref<Shader> TextShader;

        uint32_t TextIndexCount = 0;
        TextVertex* TextVertexBufferBase = nullptr;
        TextVertex* TextVertexBufferPtr = nullptr;

        Ref<VertexArray> TileVertexArray;
        TilemapVertex* TileVertexBufferBase;
        TilemapVertex* TileVertexBufferPtr;
        uint32_t TileVertexCount = 0;
        uint32_t TileIndexCount = 0;
        Ref<Shader> TileShader;
        Ref<class Tilemap> CurrentTilemap;
        std::array<Ref<Texture2D>, MaxTextureSlots> FontAtlasTextures;
        std::array<Ref<Texture2D>, MaxTextureSlots> TileSetTextures;

        std::array<Ref<Texture2D>, MaxTextureSlots> TextureSlots;
        uint32_t TextureSlotIndex = 1; //0 Should ALWAYS be the white texture
        uint32_t AtlusSlotIndex = 1; //0 Should ALWAYS be the Default Atlus
        uint32_t TilesetSlotIndex = 1; //0 Should ALWAYS be the Default Atlus

        Vector4 QuadVertexPositions[4];
        Vector4 TileVertexPositions[6];


        struct CameraData
        {
            Matrix4D CameraViewProjection;
        };

        struct TexCoordData
        {
            std::vector<Vector2*> Coords;
        };

        CameraData CameraBuffer;
        Ref<UniformBuffer> CameraUniformBuffer;

        TexCoordData CoordBuffer;
        Ref<UniformBuffer> TexCoordUniformBuffer;


        std::unordered_map<std::string, Ref<VertexBuffer>> VertexBuffers;
        Ref<VertexBuffer> GetVertexBuffer(const std::string& Name)
        {
            return VertexBuffers[Name]; 
        }


        Statistics Stats;
    };

    class Pipeline
    {
    public:

        virtual ~Pipeline() = default;

        virtual void Init() = 0;
        virtual void StartBatch2D() = 0;
        virtual void NextBatch2D() = 0;
        virtual void Flush2D() = 0;

        virtual Renderer2DData& GetData() = 0;


        virtual void ResetStats() =0;

        virtual Statistics& GetStats() = 0;

        template<typename T>
        T* As();

        static Scope<Pipeline> Create();
    };

}
```


