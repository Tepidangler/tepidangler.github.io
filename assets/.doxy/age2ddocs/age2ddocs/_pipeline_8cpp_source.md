

# File Pipeline.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**Pipeline.cpp**](_pipeline_8cpp.md)

[Go to the documentation of this file](_pipeline_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/Pipeline.h"
#include "Platform/OpenGL/Public/OpenGLPipeline.h"
#include "Render/Public/RenderAPI.h"

namespace AGE
{
Scope<Pipeline> Pipeline::Create()
    {
        switch (RendererAPI::GetAPI())
        {
            case 0:
            {
                return nullptr;
            }
            case 1: //OpenGL
            {
                return CreateScope<OpenGLPipeline>();
            }
        }
        return nullptr;
    }

    template<typename T>
T* Pipeline::As()
    {
        CoreLogger::Assert(false, "As() Failed!");
        return nullptr;
    }
}

```


