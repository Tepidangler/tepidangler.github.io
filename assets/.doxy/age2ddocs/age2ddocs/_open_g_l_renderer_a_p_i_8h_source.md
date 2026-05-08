

# File OpenGLRendererAPI.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGLRendererAPI.h**](_open_g_l_renderer_a_p_i_8h.md)

[Go to the documentation of this file](_open_g_l_renderer_a_p_i_8h.md)


```C++
#pragma once
#include "Render/Public/RenderAPI.h"

namespace AGE
{
    class OpenGLRendererAPI : public RendererAPI
    {
    public: //functions

        ~OpenGLRendererAPI() =default;
        void Init() override;
        void SetClearColor(const Vector4 Color) override;
        void SetViewport(uint32_t x, uint32_t y, uint32_t Width, uint32_t Height) override;
        void Clear() override;

        void Flush() override;
        void DrawIndexed(uint32_t IndexCount, uint32_t IndexStart, int VertexStart) override {}
        void DrawIndexed(const Ref<VertexArray>& VertexArray, uint32_t IndexCount) override;
        void DrawArrays(const Ref<VertexArray>& VertexArray,uint32_t IndexCount) override;
        void DrawLines(const Ref<VertexArray>& VertexArray, uint32_t VertexCount) override;
        void DrawStrips(const Ref<VertexArray>& VertexArray, uint32_t IndexCount) override;
        void SetLineWidth(float Width) override;


        void Submit() override;
        void Present() override;
    };
}
```


