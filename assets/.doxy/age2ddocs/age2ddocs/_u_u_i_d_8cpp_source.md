

# File UUID.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**UUID.cpp**](_u_u_i_d_8cpp.md)

[Go to the documentation of this file](_u_u_i_d_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Core/Public/UUID.h"

#include <random>

namespace AGE
{
    static std::random_device s_RandomDevice;
    static std::mt19937_64 s_Engine;
    static std::uniform_int_distribution<uint64_t> s_UniformDistribution;




COMMENT:
CONFIDENCE: 1.0;

UUID::UUID()
        :m_UUID(s_UniformDistribution(s_Engine))
    {
    }

UUID::UUID(uint64_t uuid)
        :m_UUID(uuid)
{
}
UUID::UUID(uint64_t uuid)
        :m_UUID(uuid)
    {
    }

}
```


