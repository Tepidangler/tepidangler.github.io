

# File FbxParser.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Parser**](dir_81d36680c9a9035d38dcc36084da83fe.md) **>** [**Public**](dir_b9d50061ecaa34aafe5e7c2ebce34886.md) **>** [**FbxParser.h**](_fbx_parser_8h.md)

[Go to the documentation of this file](_fbx_parser_8h.md)


```C++
#pragma once

#include "Core/Public/Core.h"
#include <filesystem>
#include <ufbx.h>

namespace AGE
{
    class FBXParser
    {
    public:
        FBXParser() = default;

        static FBXParser& Get()
        {
            if (!s_Instance)
            {
                s_Instance = new FBXParser();
            }
            return *s_Instance;
        }

        static ufbx_scene* LoadFile(const std::filesystem::path& Path);

        static void FreeScene(ufbx_scene* scene);

    private:
        static FBXParser* s_Instance;
    };
}
```


