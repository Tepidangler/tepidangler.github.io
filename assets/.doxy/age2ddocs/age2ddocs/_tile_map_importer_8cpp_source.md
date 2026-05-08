

# File TileMapImporter.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**TileMap**](dir_be586839b90880a6e3d62d2138e7c26d.md) **>** [**Private**](dir_0ee4e07c8389fb9e068d205bcc0e985a.md) **>** [**TileMapImporter.cpp**](_tile_map_importer_8cpp.md)

[Go to the documentation of this file](_tile_map_importer_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "TileMap/Public/TileMapImporter.h"

#include "Platform/OpenGL/Public/OpenGLTexture.h"
#include "Scene/Public/Scene.h"
#include "Scene/Public/Entity.h"
#include "Texture/Public/Texture.h"



namespace AGE
{
    tmx_map* TileMapImporter::ImportMap(const std::string& FilePath)
    {
        if (FilePath == "")
        {
            return nullptr;
        }
        tmx_map* Map = nullptr;
        Map = tmx_load(FilePath.c_str());
        if (!Map)
        {
            CoreLogger::Error("Could not Load TileMap At {0} !", FilePath.c_str());
            return nullptr;
        }
        CoreLogger::Info("{0} Loaded Successfully!", FilePath.c_str());
        return Map;
    }

}
```


