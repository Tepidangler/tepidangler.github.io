

# File TileMapManager.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**TileMap**](dir_be586839b90880a6e3d62d2138e7c26d.md) **>** [**Public**](dir_de3a4886f3cd637e1fda08fe9ad79a10.md) **>** [**TileMapManager.h**](_tile_map_manager_8h.md)

[Go to the documentation of this file](_tile_map_manager_8h.md)


```C++
#pragma once
#include "TileMap/Public/TileMapImporter.h"
#include "Core/Public/UUID.h"
#include "Core/Public/Pointers.h"
#include <tmx.h>


namespace AGE
{
    class Tilemap;

    class TileMapManager
    {
    public:

        TileMapManager();
        ~TileMapManager() = default;

        static TileMapManager& Get()
        {
            static TileMapManager* instance;
            if (!instance)
            {
                instance = new TileMapManager();
            }
            return *instance;
        }
        Ref<Tilemap> LoadTileMap(const std::filesystem::path& Path);
        void LoadTileMaps(const std::vector<std::filesystem::path>& Paths);
        void LoadTileMaps(void* Addr);

        static void* ImageLoad(const char* Path);
        static void ImageFree(void* Address);
    private:

        Ref<TileMapImporter> m_Importer;
        tmx_resource_manager* m_Manager;
        std::vector<Ref<Tilemap>> m_TileMaps;


    };

}
```


