

# File Statics.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Statics**](dir_26b1c48ab039ca56dd2605bba0caa957.md) **>** [**Public**](dir_1a2ee474f8e9f02a28d524d805dd06ff.md) **>** [**Statics.h**](_statics_8h.md)

[Go to the documentation of this file](_statics_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"


namespace AGE
{
    namespace Utils
    {
        class EngineStatics
        {
        public:
            static bool IsBigEndian(void)
            {
                union {
                    uint32_t i;
                    char c[4];
                } bint = { 0x01020304 };

                return bint.c[0] == 1;
            }

            template<typename T>
            static bool IsBitSet(T Num, T Pos)
            {
                T Mask = 1 << Pos;

                return (Num & Mask) != 0;
            }

            static std::string GetFilename(std::filesystem::path& Name)
            {
                return Name.replace_extension().filename().string();
            }
        };
    }
}
```


