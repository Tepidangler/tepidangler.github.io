

# File OpenGlContext.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGlContext.h**](_open_gl_context_8h.md)

[Go to the documentation of this file](_open_gl_context_8h.md)


```C++
#pragma once

#include "Render/Public/GraphicsContext.h"




struct GLFWwindow;

namespace AGE
{
    class OpenGLPipeline;

class AGE_API OpenGLContext : public GraphicsContext
    {
    public:
        OpenGLContext(GLFWwindow* WindowHandle);
            

        virtual ~OpenGLContext();


        virtual void Init() override;
        virtual void SwapBuffers()  override;


        OpenGLPipeline* GetPipeline();

        void SetPipeline(OpenGLPipeline* Pipeline);

    private:

        GLFWwindow* m_WindowHandle;
        OpenGLPipeline* m_Pipeline;

    };
}
```


