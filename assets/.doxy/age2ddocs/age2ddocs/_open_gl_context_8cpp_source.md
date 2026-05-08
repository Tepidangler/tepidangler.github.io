

# File OpenGlContext.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Private**](dir_70227f149653e1f1d3b9a02604511f36.md) **>** [**OpenGlContext.cpp**](_open_gl_context_8cpp.md)

[Go to the documentation of this file](_open_gl_context_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Platform/OpenGL/Public/OpenGlContext.h"
#include "Platform/OpenGL/Public/OpenGLPipeline.h"

#include <GLFW/glfw3.h>
#include <glad/glad.h>
#include "Debug/Public/Instrumentor.h"
namespace AGE
{
    OpenGLContext::OpenGLContext(GLFWwindow* WindowHandle)
        : m_WindowHandle(WindowHandle)
    {

        AGE_CORE_ASSERT(WindowHandle, "Window handle is null");
    }

    OpenGLContext::~OpenGLContext()
    {

    }

    void OpenGLContext::Init()
    {
        AGE_PROFILE_FUNCTION();
        glfwMakeContextCurrent(m_WindowHandle);
        int status = gladLoadGLLoader((GLADloadproc)glfwGetProcAddress);
        AGE_CORE_ASSERT(status, "Failed to initialize GLAD");

        CoreLogger::Info("OpenGL Info: ");

        CoreLogger::Trace(" Vendor: {0}", (const char*)glGetString(GL_VENDOR));
        CoreLogger::Trace(" Renderer: {0}", (const char*)glGetString(GL_RENDERER));
        CoreLogger::Trace(" Version: {0}", (const char*)glGetString(GL_VERSION));
        glDebugMessageCallback(&OpenGLContext::OpenGLErrorCallback,nullptr);


    }
    void OpenGLContext::SwapBuffers()
    {
        AGE_PROFILE_FUNCTION();
        glfwSwapBuffers(m_WindowHandle);


    }

    OpenGLPipeline* OpenGLContext::GetPipeline()
    {
        return m_Pipeline;
    }

    void OpenGLContext::SetPipeline(OpenGLPipeline* Pipeline)
    {
        m_Pipeline = Pipeline;
    }

    void OpenGLContext::OpenGLErrorCallback(uint32_t source, uint32_t type, uint32_t id, uint32_t severity, int length,
        const char *message, const void *userParam)
    {
        switch (type)
        {
            case GL_DEBUG_TYPE_ERROR:
            {
                if (severity == GL_DEBUG_SEVERITY_HIGH)
                {
                    CoreLogger::Error("OpenGL Error: \n\tid:{} \n\tmessage:{}", id,message);
                }
                break;
            }
            default:
            {
                break;
            }
        }

    }

    template<>
    OpenGLContext* GraphicsContext::As()
    {
        return (OpenGLContext*)this;
    }
}
```


