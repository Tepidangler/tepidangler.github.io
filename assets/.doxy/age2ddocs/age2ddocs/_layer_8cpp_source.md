

# File Layer.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**Layer.cpp**](_layer_8cpp.md)

[Go to the documentation of this file](_layer_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Layer.h"

#include <GLFW/glfw3.h>

namespace AGE
{
Layer::Layer(const std::string& DebugName)
        : m_DebugName(DebugName)
    {


    }

Layer::~Layer()
    {

    }
float Layer::GetTime()
    {
        return static_cast<float>(glfwGetTime());
    }
}
```


