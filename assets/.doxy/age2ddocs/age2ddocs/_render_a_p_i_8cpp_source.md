

# File RenderAPI.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**RenderAPI.cpp**](_render_a_p_i_8cpp.md)

[Go to the documentation of this file](_render_a_p_i_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/RenderAPI.h"
#include "Platform/OpenGL/Public/OpenGLRendererAPI.h"

namespace AGE
{
    RendererAPI::API RendererAPI::s_API = RendererAPI::API::OpenGL;

    Scope<RendererAPI> RendererAPI::Create()
    {
        switch ((int)s_API)
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateScope<OpenGLRendererAPI>();
            break;
        default:
            AGE_CORE_ASSERT(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }
}
```


