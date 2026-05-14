

# File GraphicsContext.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**GraphicsContext.cpp**](_graphics_context_8cpp.md)

[Go to the documentation of this file](_graphics_context_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/GraphicsContext.h"
#include "Render/Public/Renderer.h"
#include "Platform/OpenGL/Public/OpenGlContext.h"

namespace AGE
{

    
Scope<GraphicsContext> GraphicsContext::Create(void* Window)
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            CoreLogger::Assert(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateScope<OpenGLContext>(static_cast<GLFWwindow*>(Window));
            break;
        default:
            CoreLogger::Assert(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        CoreLogger::Assert(false, "Unknown Renderer API!");
        return nullptr;

    }

    template<typename T>
T* GraphicsContext::As()
    {
        CoreLogger::Assert(false, "As() Failed!");
        return nullptr;
    }

}

```


