

# File Renderer.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Private**](dir_842c434ff407c74a15cf46e820448801.md) **>** [**Renderer.cpp**](_renderer_8cpp.md)

[Go to the documentation of this file](_renderer_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Render/Public/Renderer.h"
#include "Render/Public/Renderer2D.h"
#include "Core/Public/App.h"
#include "Render/Public/RenderCommand.h"


namespace AGE
{
    Renderer::SceneData* Renderer::m_SceneData = new SceneData;

    void Renderer::Init()
    {
        AGE_PROFILE_FUNCTION();
        RenderCommand::Init();
    }

    
    void Renderer::BeginScene(const Camera& Camera, const Matrix4D& Transform)
    {
        Renderer2D::BeginScene(Camera, Transform);
    }

    void Renderer::BeginScene(const EditorCamera& Camera)
    {
        Renderer2D::BeginScene(Camera);
    }

    void Renderer::OnWindowResize(uint32_t Width, uint32_t Height)
    {
        RenderCommand::SetViewport(0, 0, Width, Height);
    }

    void Renderer::OnFramebufferResize(uint32_t Width, uint32_t Height)
    {
        RenderCommand::SetViewport(0, 0, Width, Height);
    }
    
    void Renderer::EndScene()
    {
        Renderer2D::EndScene();
    }
    void Renderer::Shutdown()
    {
        Renderer2D::Shutdown();
    }

    void Renderer::Submit()
    {
        RenderCommand::Submit();
    }
    void Renderer::Flush()
    {
        RenderCommand::Flush();
    }
}
```


