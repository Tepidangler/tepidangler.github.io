

# Class AGE::OpenGLContext



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md)








Inherits the following classes: [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**GetPipeline**](#function-getpipeline) () <br> |
| virtual void | [**Init**](#function-init) () override<br> |
|   | [**OpenGLContext**](#function-openglcontext) (GLFWwindow \* WindowHandle) <br> |
|  void | [**SetPipeline**](#function-setpipeline) ([**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* Pipeline) <br> |
| virtual void | [**SwapBuffers**](#function-swapbuffers) () override<br> |
| virtual  | [**~OpenGLContext**](#function-openglcontext) () <br> |


## Public Functions inherited from AGE::GraphicsContext

See [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_graphics_context.md#function-as-12) () <br> |
|  [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) \* | [**As**](class_a_g_e_1_1_graphics_context.md#function-as-22) () <br> |
| virtual void | [**Init**](class_a_g_e_1_1_graphics_context.md#function-init) () = 0<br> |
| virtual void | [**SwapBuffers**](class_a_g_e_1_1_graphics_context.md#function-swapbuffers) () = 0<br> |
| virtual  | [**~GraphicsContext**](class_a_g_e_1_1_graphics_context.md#function-graphicscontext) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**OpenGLErrorCallback**](#function-openglerrorcallback) (uint32\_t source, uint32\_t type, uint32\_t id, uint32\_t severity, int length, const char \* message, const void \* userParam) <br> |


## Public Static Functions inherited from AGE::GraphicsContext

See [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) &gt; | [**Create**](class_a_g_e_1_1_graphics_context.md#function-create) (void \* Window) <br> |


















































## Public Functions Documentation




### function GetPipeline 

```C++
OpenGLPipeline * AGE::OpenGLContext::GetPipeline () 
```




<hr>



### function Init 

```C++
virtual void AGE::OpenGLContext::Init () override
```



Implements [*AGE::GraphicsContext::Init*](class_a_g_e_1_1_graphics_context.md#function-init)


<hr>



### function OpenGLContext 

```C++
AGE::OpenGLContext::OpenGLContext (
    GLFWwindow * WindowHandle
) 
```




<hr>



### function SetPipeline 

```C++
void AGE::OpenGLContext::SetPipeline (
    OpenGLPipeline * Pipeline
) 
```




<hr>



### function SwapBuffers 

```C++
virtual void AGE::OpenGLContext::SwapBuffers () override
```



Implements [*AGE::GraphicsContext::SwapBuffers*](class_a_g_e_1_1_graphics_context.md#function-swapbuffers)


<hr>



### function ~OpenGLContext 

```C++
virtual AGE::OpenGLContext::~OpenGLContext () 
```




<hr>
## Public Static Functions Documentation




### function OpenGLErrorCallback 

```C++
static void AGE::OpenGLContext::OpenGLErrorCallback (
    uint32_t source,
    uint32_t type,
    uint32_t id,
    uint32_t severity,
    int length,
    const char * message,
    const void * userParam
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGlContext.h`

