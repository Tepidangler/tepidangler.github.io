

# File Renderer.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Public**](dir_68ba7e1260de504efb39109a85960357.md) **>** [**Renderer.h**](_renderer_8h.md)

[Go to the documentation of this file](_renderer_8h.md)


```C++
#pragma once
#include "Render/Public/RenderAPI.h"
#include "Camera/Public/Camera.h"
#include "Camera/Public/EditorCamera.h"
#include "UI/Public/WidgetStack.h"

namespace AGE
{
    class Renderer
    {
        public:

            static void Init();
            static void BeginScene(const Camera&  Camera, const Matrix4D& Transform);
            static void BeginScene(const EditorCamera&  Camera);
            static void OnWindowResize(uint32_t Width, uint32_t Height);
            static void OnFramebufferResize(uint32_t Width, uint32_t Height);
            static void EndScene();
            static void Shutdown();

            static void Submit();

            static void Flush();

static inline RendererAPI::API GetAPI() { return RendererAPI::GetAPI(); }
COMMENT:
CONFIDENCE: 1.0;

static inline void SetAPI(RendererAPI::API Renderer) { RendererAPI::SetAPI(Renderer); }
        private:
            struct SceneData
            {
                Matrix4D ViewProjectionMatrix;

                Matrix4D ViewProjectionModelMatrix;
            };

            static SceneData* m_SceneData;



    };
}
```


