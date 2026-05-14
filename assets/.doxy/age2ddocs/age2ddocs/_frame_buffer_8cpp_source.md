

# File FrameBuffer.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**FrameBuffer.cpp**](_frame_buffer_8cpp.md)

[Go to the documentation of this file](_frame_buffer_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/FrameBuffer.h"
#include "Render/Public/Renderer.h"
#include "Platform/OpenGL/Public/OpenGLFrameBuffer.h"

namespace AGE
{
Ref<FrameBuffer> FrameBuffer::Create(const FrameBufferSpecification& Spec)
    {
            switch (Renderer::GetAPI())
            {
            case 0:
                CoreLogger::Assert(false, "RendererAPI::API::None is currently not supported!");
                return nullptr;
                break;
            case 1:
                return CreateRef<OpenGLFrameBuffer>(Spec);
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
T* FrameBuffer::As()
    {
        CoreLogger::Assert(false, "As() Failed!");
        return nullptr;
    }
}
```


