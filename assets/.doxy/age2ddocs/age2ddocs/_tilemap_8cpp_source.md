

# File Tilemap.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**TileMap**](dir_be586839b90880a6e3d62d2138e7c26d.md) **>** [**Private**](dir_0ee4e07c8389fb9e068d205bcc0e985a.md) **>** [**Tilemap.cpp**](_tilemap_8cpp.md)

[Go to the documentation of this file](_tilemap_8cpp.md)


```C++
//
// Created by gdmgp on 3/14/2026.
//

#include "TileMap/Public/Tilemap.h"

#include "Debug/Public/Instrumentor.h"
#include "Platform/OpenGL/Public/OpenGLTexture.h"
#include "Texture/Public/SubTexture.h"
#include "Render/Public/RenderCommand.h"

namespace AGE
{
    Tilemap::Tilemap(tmx_map* Map)
        :m_Map(Map)
    {

    }

    Tilemap::~Tilemap()
    {
        for (auto [k,v] : m_UVs)
        {
            for (auto vec : v)
            {
                delete vec;
            }
        }
    }

    void Tilemap::SetScene(Ref<Scene>& scene)
    {
        m_Scene =scene;
    }

    void Tilemap::SetShaderData()
    {
    }

    void Tilemap::BuildTilemapData()
    {
        ProcessTilesets(m_Map->ts_head);
        SetTileLocations();
        SetTileData();
    }

    void Tilemap::BindData()
    {
        std::ranges::for_each(m_Data,[&](const TilesetData& data)
        {
            auto it = std::ranges::find(RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures,data.AtlasTexture);
            if (it == RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures.end())
            {
                auto it2 = std::ranges::find(RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures, nullptr);
                if (it2 != RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures.end())
                {
                    auto dist = std::distance(RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures.begin(), it2);
                    RenderCommand::s_GraphicsPipeline->GetData().TileSetTextures[dist] = data.AtlasTexture;
                }
            }
        });
    }

    const uint32_t Tilemap::GetNumberOfLayers()
    {
        return (uint32_t)ProcessLayers(m_Map->ly_head);
    }

    int Tilemap::ProcessLayers(tmx_layer* Head)
    {
        int Tmp = 0;
        tmx_layer* Current = Head;
        while (Current)
        {
            Current = Current->next;
            Tmp++;
        }

        return Tmp;
    }

    void Tilemap::ProcessTilesets(tmx_tileset_list *Head)
    {
        tmx_tileset_list* Current = Head;
        TextureSpecification Spec{};

        while (Current)
        {
            if (Current->tileset->image)
            {
                Spec.Width = Current->tileset->image->width;
                Spec.Height = Current->tileset->image->height;
                Spec.Format = ImageFormat::RGBA8;
                TilesetData data{};
                data.AtlasTexture = Texture2D::Create((uint8_t*)Current->tileset->image->resource_image,Spec);
                data.FirstGID =Current->firstgid;
                data.TileWidth =Current->tileset->tile_width;
                data.TileHeight =Current->tileset->tile_height;
                m_Data.emplace_back(data);
            }
            Current = Current->next;
        }
    }

    void Tilemap::SetTileLocations()
    {
        AGE_PROFILE_FUNCTION();
        uint32_t Width= 0, Height = 0 ;
        size_t UvTextureSize = 0;
        uint32_t UvTextureWidth = 0 ,UvTextureHeight = 0;
        std::ranges::for_each(m_Data,[&](TilesetData& data)
        {
            Width = data.AtlasTexture->GetWidth();
            Height = data.AtlasTexture->GetHeight();
            UvTextureWidth += Width/data.TileWidth;
            UvTextureHeight += Height/data.TileHeight;
            std::vector<Vector2> TileLocs;
            for (int y = UvTextureHeight-1; y >= 0 ; y--)
            {
                for (int x = 0; x < UvTextureWidth ; x++)
                {
                    TileLocs.push_back(Vector2(x, y));
                }
            }

            for (int i = 0; i < TileLocs.size(); i++)
            {
                Ref<SubTexture2D> subtex = SubTexture2D::CreateFromCoords(data.AtlasTexture, TileLocs[i], { (float)data.TileWidth,(float)data.TileHeight});
                data.SubTexs.emplace_back(subtex);
            }
        });
    }

    void Tilemap::SetTileData()
    {
        m_MapWidth = m_Map->width;
        m_MapHeight = m_Map->height;

        tmx_layer* layer = m_Map->ly_head;
        uint32_t LayerCount = 0;
        uint32_t GID;
        std::vector<Vector2*> UVs;
        while (layer)
        {
            switch (layer->type)
            {
                case L_LAYER:
                {
                    for (uint32_t ty =0; ty <m_MapHeight; ty++ )
                    {
                        for (uint32_t tx =0; tx <m_MapWidth; tx++)
                        {
                            GID = (layer->content.gids[ty*m_MapWidth+tx]) & TMX_FLIP_BITS_REMOVAL;

                            if (m_Map->tiles[GID])
                            {
                                uint32_t LID = m_Map->tiles[GID]->id;
                                UVs.emplace_back(const_cast<Vector2 *>(m_Data.back().SubTexs[LID]->GetTexCoords()));
                            }
                        }
                    }
                }
                default:
                {
                    break;
                }
            }
            layer = layer->next;

            std::ranges::reverse(UVs);
            for (size_t x = 0; x < UVs.size(); x++)
            {
                m_UVs[LayerCount].emplace_back(UVs[x]);
            }
            LayerCount++;
            UVs.clear();

        }


    }
} // AGE
```


