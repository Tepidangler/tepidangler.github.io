

# File OpenGLRendererAPI.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Private**](dir_70227f149653e1f1d3b9a02604511f36.md) **>** [**OpenGLRendererAPI.cpp**](_open_g_l_renderer_a_p_i_8cpp.md)

[Go to the documentation of this file](_open_g_l_renderer_a_p_i_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Platform/OpenGL/Public/OpenGLRendererAPI.h"

#include <glad/glad.h>
#include "Debug/Public/Instrumentor.h"
namespace AGE
{
    void OpenGLRendererAPI::Init()
    {
        AGE_PROFILE_FUNCTION();
        glEnable(GL_BLEND);
        glBlendEquation(GL_FUNC_ADD);
        glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA);
        glEnable(GL_DEPTH_TEST);
        //glDepthFunc(GL_LEQUAL);
        //glClearDepth(1.0f);
        glEnable(GL_LINE_SMOOTH);
        glFrontFace(GL_CW);
    }
    void OpenGLRendererAPI::SetClearColor(const Vector4 Color)
    {
        glClearColor(Color[0], Color[1], Color[2], Color[3]);
        glBlendColor(1.f, 1.f, 1.f, 1.f);
        
    }
    void OpenGLRendererAPI::SetViewport(uint32_t x, uint32_t y, uint32_t Width, uint32_t Height)
    {
        glViewport(-1, -1, (int)Width, (int)Height);
        
    }
    void OpenGLRendererAPI::Clear()
    {
        glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);
        
    }
    void OpenGLRendererAPI::Flush()
    {
        glFlush();
    }
    void OpenGLRendererAPI::DrawIndexed(const Ref<VertexArray>& VertexArray, uint32_t IndexCount)
    {
        VertexArray->Bind();

        uint32_t Count = IndexCount ? IndexCount : VertexArray->GetIndexBuffer()->GetCount();
        glDrawElements(GL_TRIANGLES, (int)Count, GL_UNSIGNED_INT, nullptr);
        glBindTexture(GL_TEXTURE_2D, 0);

    }

    void OpenGLRendererAPI::DrawArrays(const Ref<VertexArray> &VertexArray, uint32_t IndexCount)
    {
        VertexArray->Bind();

        glDrawArrays(GL_TRIANGLES, 0, (int)IndexCount);
    }

    void OpenGLRendererAPI::DrawLines(const Ref<VertexArray>& VertexArray, uint32_t VertexCount)
    {
        VertexArray->Bind();
        glDrawArrays(GL_LINES, 0, (int)VertexCount);
    }
    void OpenGLRendererAPI::DrawStrips(const Ref<VertexArray>& VertexArray, uint32_t IndexCount)
    {
        VertexArray->Bind();

        uint32_t Count = IndexCount ? IndexCount : VertexArray->GetIndexBuffer()->GetCount();
        glDrawElements(GL_TRIANGLE_STRIP, (int)Count, GL_UNSIGNED_INT, nullptr);
        glBindTexture(GL_TEXTURE_2D, 0);
    }
    void OpenGLRendererAPI::SetLineWidth(float Width)
    {
        glLineWidth(Width);
    }
    void OpenGLRendererAPI::Submit()
    {
    }
    void OpenGLRendererAPI::Present()
    {
    }
}
```


