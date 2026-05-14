

# File TileMapImporter.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**TileMap**](dir_be586839b90880a6e3d62d2138e7c26d.md) **>** [**Public**](dir_de3a4886f3cd637e1fda08fe9ad79a10.md) **>** [**TileMapImporter.h**](_tile_map_importer_8h.md)

[Go to the documentation of this file](_tile_map_importer_8h.md)


```C++
#pragma once
#include <tmx.h>
#include "Core/Public/Core.h"


namespace AGE
{
    class TileMapImporter
    {
    public:

TileMapImporter() = default;
TileMapImporter(const TileMapImporter&) = delete;
~TileMapImporter() = default;

        tmx_map* ImportMap(const std::string& FilePath);


    };
}
```


