

# File Renderer2D.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**Renderer2D.cpp**](_renderer2_d_8cpp.md)

[Go to the documentation of this file](_renderer2_d_8cpp.md)


```C++
#include "AGEpch.hpp"

#include "Render/Public/Renderer2D.h"
#include "Render/Public/RenderCommand.h"
#include "Render/Public/VertexArray.h"
#include "Scene/Public/Entity.h"
#include "Platform/OpenGL/Public/OpenGLShader.h"
#include "Sprite/Public/SpriteAPI.h"
#include <glm/gtc/matrix_transform.hpp>
#ifdef __clang__
#pragma clang diagnostic push
#pragma clang diagnostic ignored "-Wconversion"
#pragma clang diagnostic ignored "-Wfloat-conversion"
#ifdef AG_PLATFORM_WINDOWS
#pragma GCC diagnostic ignored "-Wmicrosoft-unqualified-friend"
#endif
#include "Render/Public/MSDFData.h"
#include <rttr/registration>
#pragma clang diagnostic pop
#elif defined(__GNUC__)
#pragma GCC diagnostic push
#pragma GCC diagnostic ignored "-Wconversion"
#pragma GCC diagnostic ignored "-Wfloat-conversion"
#ifdef AG_PLATFORM_WINDOWS
#pragma GCC diagnostic ignored "-Wmicrosoft-unqualified-friend"
#endif
#include <rttr/registration>
#include "Render/Public/MSDFData.h"
#pragma GCC diagnostic pop
#elif defined(_MSC_VER)
#pragma warning(push, 0)
#include <rttr/registration>
#include "Render/Public/MSDFData.h"
#pragma warning(pop)
#else
#error "Compiler is not supported with AGE yet"
#endif
RTTR_REGISTRATION
{
    rttr::registration::method("Draw String", &AGE::Renderer2D::DrawString);
}

namespace AGE
{

    void Renderer2D::Init()
    {

    }
        

    void Renderer2D::Shutdown()
    {

    }
    
    void Renderer2D::BeginScene(const Camera& Camera, const Matrix4D& Transform)
    {
        AGE_PROFILE_FUNCTION();
        RenderCommand::s_GraphicsPipeline->StartBatch2D();
    }
    void Renderer2D::BeginScene(const EditorCamera& Camera)
    {
        AGE_PROFILE_FUNCTION();

        Matrix4D WVPM = (Camera.GetProjection() * Camera.GetViewMatrix()) * Camera.GetWorldMatrix();
        RenderCommand::s_GraphicsPipeline->GetData().CameraUniformBuffer->SetData(&WVPM, sizeof(Renderer2DData::CameraData));
        RenderCommand::s_GraphicsPipeline->StartBatch2D();
    }
    void Renderer2D::EndScene()
    {
        AGE_PROFILE_FUNCTION();

        RenderCommand::s_GraphicsPipeline->Flush2D();
    }
    void Renderer2D::Flush()
    {
        RenderCommand::s_GraphicsPipeline->Flush2D();       
    }

    void Renderer2D::DrawQuad(const QuadProperties& Props)
    {
        if (RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount >= Renderer2DData::MaxIndexCount)
        {
            RenderCommand::s_GraphicsPipeline->NextBatch2D();
        }
        RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Quad"]->CreateQuad(RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr, Props.Color, RenderCommand::s_GraphicsPipeline->GetData().QuadVertexPositions, Props.Size, Props.Transform, Props.TextureCoords, Props.TilingFactor, 0, Props.EntityID);
        RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount += 6;

        RenderCommand::s_GraphicsPipeline->GetData().Stats.QuadCount++;
    }
    void Renderer2D::DrawQuad(const Ref<Texture2D>& Texture, const QuadProperties& Props)
    {
        if (RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount >= Renderer2DData::MaxIndexCount)
        {
            RenderCommand::s_GraphicsPipeline->NextBatch2D();
        }
        float TextureIndex = 0.f;
    
        if (Texture != nullptr)
        {
            for (uint32_t i = 0; i < RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex; i++)
            {
                if (*RenderCommand::s_GraphicsPipeline->GetData().TextureSlots[i].get() == *Texture.get())
                {
                    TextureIndex = (float)i;
                    break;
                }
            }
    
            if (TextureIndex == 0.f)
            {
                TextureIndex = (float)RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex;
                RenderCommand::s_GraphicsPipeline->GetData().TextureSlots[RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex] = Texture;
                RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex++;
    
            }
        }
        RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Quad"]->CreateQuad(RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr, Props.TintColor, RenderCommand::s_GraphicsPipeline->GetData().QuadVertexPositions, Props.Size, Props.Transform, Props.TextureCoords, Props.TilingFactor, TextureIndex, Props.EntityID);
        RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount += 6;
        RenderCommand::s_GraphicsPipeline->GetData().Stats.QuadCount++;
    }
    void Renderer2D::DrawQuad(const Ref<SubTexture2D>& Subtexture, const QuadProperties& Props)
    {
        if (RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount >= Renderer2DData::MaxIndexCount)
        {
            RenderCommand::s_GraphicsPipeline->NextBatch2D();
        }
        const Ref<Texture2D> texture = Subtexture->GetTexture();
        float TextureIndex = 0.f;

        if (texture != nullptr)
        {
            for (uint32_t i = 1; i < RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex; i++)
            {
                if (*RenderCommand::s_GraphicsPipeline->GetData().TextureSlots[i].get() == *texture.get())
                {
                    TextureIndex = (float)i;
                    break;
                }
            }

            if (TextureIndex == 0.f)
            {
                TextureIndex = (float)RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex;
                RenderCommand::s_GraphicsPipeline->GetData().TextureSlots[RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex] = texture;
                RenderCommand::s_GraphicsPipeline->GetData().TextureSlotIndex++;

            }
        }
        RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Quad"]->CreateQuad(RenderCommand::s_GraphicsPipeline->GetData().QuadVertexBufferPtr, Props.TintColor, RenderCommand::s_GraphicsPipeline->GetData().QuadVertexPositions, Props.Size, Props.Transform, Props.TextureCoords, Props.TilingFactor, TextureIndex, Props.EntityID);
        RenderCommand::s_GraphicsPipeline->GetData().QuadIndexCount += 6;
        RenderCommand::s_GraphicsPipeline->GetData().Stats.QuadCount++;
    }
    void Renderer2D::DrawCircle(const Matrix4D& Transform, const Vector4& Color, float Thickness, float Fade, int EntityID)
    {
        AGE_PROFILE_FUNCTION();

        //TODO:: Implement for circles
        //if (RenderCommand::s_GraphicsPipeline->GetData().CircleIndexCount >= Renderer2DData::MaxIndexCount)
        //{
        //  NextBatch();
        //}


        RenderCommand::s_GraphicsPipeline->GetData().CircleVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Circle"]->CreateCircle(RenderCommand::s_GraphicsPipeline->GetData().CircleVertexBufferPtr, Transform, RenderCommand::s_GraphicsPipeline->GetData().QuadVertexPositions, Color, Thickness, Fade, EntityID);
        
        RenderCommand::s_GraphicsPipeline->GetData().CircleIndexCount += 6;
        RenderCommand::s_GraphicsPipeline->GetData().Stats.CircleCount++;
    }

    void Renderer2D::DrawLine(const Vector3& Pos0, const Vector3& Pos1, const Vector4& Color, int EntityID)
    {
        RenderCommand::s_GraphicsPipeline->GetData().LineVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Line"]->CreateLine(RenderCommand::s_GraphicsPipeline->GetData().LineVertexBufferPtr, Color, Pos0, Pos1, EntityID);

        RenderCommand::s_GraphicsPipeline->GetData().LineVertexCount += 2;
    }

    void Renderer2D::DrawRect(const Vector3& Position, const Vector2& Size, const Vector4& Color, int EntityID)
    {
        Vector3 p0 = Vector3(Position.x - Size.x * .5f, Position.y - Size.y * .5f, Position.z);
        Vector3 p1 = Vector3(Position.x + Size.x * .5f, Position.y - Size.y * .5f, Position.z);
        Vector3 p2 = Vector3(Position.x + Size.x * .5f, Position.y + Size.y * .5f, Position.z);
        Vector3 p3 = Vector3(Position.x - Size.x * .5f, Position.y + Size.y * .5f, Position.z);

        DrawLine(p0,p1 , Color);
        DrawLine(p1,p2 , Color);
        DrawLine(p2,p3 , Color);
        DrawLine(p3,p0 , Color);
    }

    void Renderer2D::DrawRect(const Matrix4D& Transform, const Vector4& Color, int EntityID)
    {
        Vector3 LineVertices[4];
        for (int i = 0; i < 4; i++)
        {
            LineVertices[i] = Transform * RenderCommand::s_GraphicsPipeline->GetData().QuadVertexPositions[i];
        }

        DrawLine(LineVertices[0], LineVertices[1], Color);
        DrawLine(LineVertices[1], LineVertices[2], Color);
        DrawLine(LineVertices[2], LineVertices[3], Color);
        DrawLine(LineVertices[3], LineVertices[0], Color);

    }

    void Renderer2D::DrawSprite(SpriteRendererComponent& SRC)
    {
        if (SRC.Texture)
        {
            DrawQuad(SRC.Texture, SRC.QuadProps);
        }

        if (SRC.AnimTextures.size() > 0)
        {
            SRC.AnimInstance.SetCurrentTexture(SRC.MovementStatus);
            SpriteSheetUtils::SetTexCoords(SRC.AnimInstance.GetCurrentTexture(), SRC.QuadProps, false);
            DrawQuad(SRC.AnimInstance.GetCurrentTexture(), SRC.QuadProps);
        }

        if (SRC.AnimTextures.size() == 0 && !SRC.Texture && !SRC.SubTexture)
        {
            DrawQuad(SRC.QuadProps);
        }

        if (SRC.SubTexture)
        {
            SpriteSheetUtils::SetTexCoords(SRC.SubTexture, SRC.QuadProps, false);
            DrawQuad(SRC.SubTexture, SRC.QuadProps);
        }
    }
    void Renderer2D::DrawString(const StringProperties& Props)
    {

        const auto& FontGeometry = Props.TextFont->GetMSDFData()->FontGeometry;
        const auto& Metrics = FontGeometry.getMetrics();

        Ref<Texture2D> FontAtlas = Props.TextFont->GetAtlasTexture();
        float TextureIndex = 0.f;
        if (FontAtlas != nullptr)
        {
            for (uint32_t i = 1; i < RenderCommand::s_GraphicsPipeline->GetData().AtlusSlotIndex; i++)
            {
                if (*RenderCommand::s_GraphicsPipeline->GetData().FontAtlasTextures[i].get() == *FontAtlas.get())
                {
                    TextureIndex = (float)i;
                    break;
                }
            }

            if (TextureIndex == 0.f)
            {
                TextureIndex = (float)RenderCommand::s_GraphicsPipeline->GetData().AtlusSlotIndex;
                RenderCommand::s_GraphicsPipeline->GetData().FontAtlasTextures[RenderCommand::s_GraphicsPipeline->GetData().AtlusSlotIndex] = FontAtlas;
                RenderCommand::s_GraphicsPipeline->GetData().AtlusSlotIndex++;

            }
        }

        double x = 0.0;
        double FSScale = (0.1 * Props.FontSize) / (Metrics.ascenderY - Metrics.descenderY);
        double y = 0.0;
        float LineHeightOffset = 0.f;


        for (size_t i = 0; i < Props.Text.size(); i++)
        {
            char Character = Props.Text[i];
            if (Character == '\r')
            {
                continue;
            }

            if (Character == '\n')
            {
                x = 0;
                y -= FSScale * Metrics.lineHeight + LineHeightOffset;
                continue;
            }
            auto Glyph = FontGeometry.getGlyph((uint32_t)Character);
            if (!Glyph)
            {
                Glyph = FontGeometry.getGlyph('?');
            }
            if (!Glyph)
            {
                return;
            }

            if (Character == '\t')
            {
                Glyph = FontGeometry.getGlyph(' ');
            }

            double al, ab, ar, at;
            Glyph->getQuadAtlasBounds(al, ab, ar, at);
            Vector2 TexCoordMin((float)al, (float)ab);
            Vector2 TexCoordMax((float)ar, (float)at);

            double pl, pb, pr, pt;
            Glyph->getQuadPlaneBounds(pl, pb, pr, pt);
            Vector2 QuadMin((float)pl, (float)pb);
            Vector2 QuadMax((float)pr, (float)pt);

            QuadMin *= (float)FSScale, QuadMax *= (float)FSScale;
            QuadMin += Vector2((float)x, (float)y);
            QuadMax += Vector2((float)x, (float)y);

            double TexelWidth = 1.f / (float)FontAtlas->GetWidth();
            double TexelHeight = 1.f / (float)FontAtlas->GetHeight();

            TexCoordMin.x *= (float)TexelWidth;
            TexCoordMin.y *= (float)TexelHeight;
            TexCoordMax.x *= (float)TexelWidth;
            TexCoordMax.y *= (float)TexelHeight;

            Vector4 Pos[4];
            Pos[0] = { QuadMin.x, QuadMin.y, 0.f,1.f };
            Pos[1] = { QuadMin.x, QuadMax.y, 0.f,1.f };
            Pos[2] = { QuadMax.x, QuadMax.y, 0.f,1.f };
            Pos[3] = { QuadMax.x, QuadMin.y, 0.f,1.f };

            Vector2 Coords[4];
            Coords[0] = TexCoordMin;
            Coords[1] = { TexCoordMin.x, TexCoordMax.y };
            Coords[2] = TexCoordMax;
            Coords[3] = { TexCoordMax.x, TexCoordMin.y };

            Matrix4D Transform  = Math::MakeTransform(Props.Position, Props.Rotation, Vector3(1.f));
            RenderCommand::s_GraphicsPipeline->GetData().TextVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Text"]->CreateText(RenderCommand::s_GraphicsPipeline->GetData().TextVertexBufferPtr, Transform, Pos, Props.Color, Coords, TextureIndex,0);
            RenderCommand::s_GraphicsPipeline->GetData().TextIndexCount += 6;
            RenderCommand::s_GraphicsPipeline->GetData().Stats.QuadCount++;

            if (i < Props.Text.size() - 1)
            {
                double Advance = Glyph->getAdvance();
                char NextCharacter = Props.Text[i + 1];
                FontGeometry.getAdvance(Advance, (uint32_t)Character, (uint32_t)NextCharacter);

                float KerningOffset = 0.f;
                x += FSScale * Advance + KerningOffset;
            }
        }

    }

    void Renderer2D::DrawTileMap(const Ref<Tilemap>& Map, const TilemapProperties &Props)
    {
        if (RenderCommand::s_GraphicsPipeline->GetData().TileVertexCount >= Renderer2DData::MaxVertices)
        {
            RenderCommand::s_GraphicsPipeline->NextBatch2D();
        }

        int NumOfTiles = Map->GetMapDimensions().first * Map->GetMapDimensions().second;
        Vector4* BasePos = RenderCommand::s_GraphicsPipeline->GetData().TileVertexPositions;
        Vector2* BaseUV;
        Vector4 CurrentPos[6];
        Vector2 CurrentUV[6];
        for (uint32_t l = 0; l < Props.NumofLayers; l++)
        {
            for (int i =0,y =0, x =0; i < NumOfTiles; i++, x++)
            {
                if (i % Map->GetMapDimensions().first == 0 && i != 0)
                {
                    y++;
                    x=0;
                }
                BaseUV = Props.UV.at(l)[i];
                CurrentPos[0] = {BasePos[0].x + (float)x,BasePos[0].y + (float)y,BasePos[0].z+ (float)l,BasePos[0].w};
                CurrentPos[1] = {BasePos[1].x + (float)x,BasePos[1].y + (float)y,BasePos[1].z+ (float)l,BasePos[1].w};
                CurrentPos[2] = {BasePos[2].x + (float)x,BasePos[2].y + (float)y,BasePos[2].z+ (float)l,BasePos[2].w};
                CurrentPos[3] = {BasePos[3].x + (float)x,BasePos[3].y + (float)y,BasePos[3].z+ (float)l,BasePos[3].w};
                CurrentPos[4] = {BasePos[4].x + (float)x,BasePos[4].y + (float)y,BasePos[4].z+ (float)l,BasePos[4].w};
                CurrentPos[5] = {BasePos[5].x + (float)x,BasePos[5].y + (float)y,BasePos[5].z+ (float)l,BasePos[5].w};

                CurrentUV[0] = BaseUV[0]; // Max, Max
                CurrentUV[1] = BaseUV[1]; // Max, Min
                CurrentUV[2] = BaseUV[2]; // Min, Min
                CurrentUV[3] = BaseUV[2]; // Min, Min
                CurrentUV[4] = BaseUV[0]; // Max,Max
                CurrentUV[5] = BaseUV[3]; // Min,Max

                RenderCommand::s_GraphicsPipeline->GetData().TileVertexBufferPtr = RenderCommand::s_GraphicsPipeline->GetData().VertexBuffers["Tilemap"]->CreateTile(RenderCommand::s_GraphicsPipeline->GetData().TileVertexBufferPtr, Props.Color,CurrentPos,Props.Transform, CurrentUV,Props.TileSetID,Props.EntityID );
                RenderCommand::s_GraphicsPipeline->GetData().TileVertexCount += 6;
                RenderCommand::s_GraphicsPipeline->GetData().Stats.TileCount++;

                if (RenderCommand::s_GraphicsPipeline->GetData().TileVertexCount >= Renderer2DData::MaxVertices)
                {
                    RenderCommand::s_GraphicsPipeline->NextBatch2D();
                }
            }
        }
    }

    Statistics Renderer2D::GetStats()
    {
        return RenderCommand::s_GraphicsPipeline->GetData().Stats;
    }
    float Renderer2D::GetLineWidth()
    {
        return RenderCommand::s_GraphicsPipeline->GetData().LineWidth;
    }
    void Renderer2D::SetLineWidth(float Width)
    {
        RenderCommand::s_GraphicsPipeline->GetData().LineWidth = Width;
    }
}
```


