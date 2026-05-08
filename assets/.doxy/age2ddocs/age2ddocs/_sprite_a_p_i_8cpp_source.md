

# File SpriteAPI.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Sprite**](dir_98f921a13af52dba16d3bd4307347abb.md) **>** [**Private**](dir_fa5d7c06fd339e78ef99ea94da2e8bec.md) **>** [**SpriteAPI.cpp**](_sprite_a_p_i_8cpp.md)

[Go to the documentation of this file](_sprite_a_p_i_8cpp.md)


```C++
#include "AGEpch.hpp"

#include "Sprite/Public/SpriteAPI.h"

namespace AGE
{
    void SpriteSheetUtils ::SetTexCoords(const Ref<SubTexture2D> SubTex, QuadProperties& Properties, bool Reverse)
    {
        if (!Reverse)
        {
            Properties.TextureCoords[0] = SubTex->GetTexCoords()[0];
            Properties.TextureCoords[1] = SubTex->GetTexCoords()[1];
            Properties.TextureCoords[2] = SubTex->GetTexCoords()[2];
            Properties.TextureCoords[3] = SubTex->GetTexCoords()[3];
        }
        else
        {
            Properties.TextureCoords[0] = SubTex->GetTexCoords()[1];
            Properties.TextureCoords[1] = SubTex->GetTexCoords()[0];
            Properties.TextureCoords[2] = SubTex->GetTexCoords()[3];
            Properties.TextureCoords[3] = SubTex->GetTexCoords()[2];
        }
    }
}
```


