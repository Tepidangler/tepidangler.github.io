

# File SpriteAPI.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Sprite**](dir_98f921a13af52dba16d3bd4307347abb.md) **>** [**Public**](dir_004ba52baf3cfab84cfd4a68d034b9b5.md) **>** [**SpriteAPI.h**](_sprite_a_p_i_8h.md)

[Go to the documentation of this file](_sprite_a_p_i_8h.md)


```C++
#pragma once
#include "Texture/Public/SubTexture.h"
#include "Structs/Public/DataStructures.h"


namespace AGE
{
    class SpriteSheetUtils
    {
    public:

        static void SetTexCoords(const Ref<SubTexture2D> SubTex, QuadProperties& Properties, bool Reverse = false);

    private:

    };
}
```


