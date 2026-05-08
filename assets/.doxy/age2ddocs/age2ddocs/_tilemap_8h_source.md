

# File Tilemap.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**TileMap**](dir_be586839b90880a6e3d62d2138e7c26d.md) **>** [**Public**](dir_de3a4886f3cd637e1fda08fe9ad79a10.md) **>** [**Tilemap.h**](_tilemap_8h.md)

[Go to the documentation of this file](_tilemap_8h.md)


```C++
//
// Created by gdmgp on 3/14/2026.
//

#ifndef AGE_TILEMAP_H
#define AGE_TILEMAP_H
#include "Core/Public/Pointers.h"
#include "Scene/Public/Scene.h"
#include "Texture/Public/Texture.h"
#include "Core/Public/UUID.h"
#include <tmx.h>

#include "Core/Public/Types.h"

namespace AGE
{
    class SubTexture2D;
    struct TilesetData
    {
        Ref<Texture2D> AtlasTexture;
        uint32_t FirstGID;
        uint32_t TileWidth, TileHeight = 0;
        std::vector<Ref<SubTexture2D>> SubTexs;
    };
    class Tilemap : public std::enable_shared_from_this<Tilemap>
    {
    public:
        Tilemap(tmx_map* Map);
        ~Tilemap();

        Ref<Scene> GetScene() { return m_Scene; }
        std::vector<TilesetData>& GetData() { return m_Data; }
        [[nodiscard]] std::filesystem::path GetPath() const { return m_Path; }
        std::pair<uint32_t,uint32_t> GetMapDimensions() {return {m_MapWidth,m_MapHeight}; }
        std::map<uint32_t, std::vector<Vector2*>>& GetUVs() {return m_UVs;}
        UUID GetAssetID() { return m_AssetID; }
        void SetScene(Ref<Scene>& scene);
        void SetPath(const std::filesystem::path &Path) {m_Path = Path;}
        void SetShaderData();
        void SetTileLocations();
        void BuildTilemapData();
        void BindData();
        const uint32_t GetNumberOfLayers();

    private:
        Ref<Scene> m_Scene;
        std::vector<TilesetData> m_Data;
        std::filesystem::path m_Path;
        tmx_map* m_Map = nullptr;
        UUID m_AssetID;
        uint32_t m_MapWidth = 0, m_MapHeight = 0;
        std::map<uint32_t, std::vector<Vector2*>> m_UVs;
        int ProcessLayers(tmx_layer* Head);
        void ProcessTilesets(tmx_tileset_list* Head);
        void SetTileData();
    };
} // AGE

#endif //AGE_TILEMAP_H
```


