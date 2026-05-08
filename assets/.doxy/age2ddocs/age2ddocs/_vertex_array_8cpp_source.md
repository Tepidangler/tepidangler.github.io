

# File VertexArray.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**VertexArray.cpp**](_vertex_array_8cpp.md)

[Go to the documentation of this file](_vertex_array_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/VertexArray.h"
#include "Render/Public/Renderer.h"
#include "Platform/OpenGL/Public/OpenGLVertexArray.h"

namespace AGE
{
    Ref<VertexArray> VertexArray::Create()
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateRef<OpenGLVertexArray>();
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


