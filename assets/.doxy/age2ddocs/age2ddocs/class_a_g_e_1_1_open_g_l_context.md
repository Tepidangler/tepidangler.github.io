

# Class AGE::OpenGLContext



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md)



_Constructor for_ [_**OpenGLContext**_](class_a_g_e_1_1_open_g_l_context.md) _. Initializes the context with a GLFW window handle._[More...](#detailed-description)

* `#include <OpenGlContext.h>`



Inherits the following classes: [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**GetPipeline**](#function-getpipeline) () <br>_Get the pipeline object associated with this context._  |
| virtual void | [**Init**](#function-init) () override<br>_Initializes the OpenGL context._  |
|   | [**OpenGLContext**](#function-openglcontext) (GLFWwindow \* WindowHandle) <br>_Constructs an_ [_**OpenGLContext**_](class_a_g_e_1_1_open_g_l_context.md) _object._ |
|  void | [**SetPipeline**](#function-setpipeline) ([**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* Pipeline) <br>_This function sets the pipeline for the OpenGL context._  |
| virtual void | [**SwapBuffers**](#function-swapbuffers) () override<br>_Swaps the front and back buffers of the specified window._  |
| virtual  | [**~OpenGLContext**](#function-openglcontext) () <br>_Destructor for the_ [_**OpenGLContext**_](class_a_g_e_1_1_open_g_l_context.md) _class._ |


## Public Functions inherited from AGE::GraphicsContext

See [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_graphics_context.md#function-as-12) () <br>_This function is a placeholder for future use. It currently always asserts false and returns null._  |
|  [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) \* | [**As**](class_a_g_e_1_1_graphics_context.md#function-as-22) () <br>_This function returns a pointer to the OpenGL context associated with this instance of_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _._ |
| virtual void | [**Init**](class_a_g_e_1_1_graphics_context.md#function-init) () = 0<br> |
| virtual void | [**SwapBuffers**](class_a_g_e_1_1_graphics_context.md#function-swapbuffers) () = 0<br> |
| virtual  | [**~GraphicsContext**](class_a_g_e_1_1_graphics_context.md#function-graphicscontext) () <br>_Virtual destructor for the_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _class._ |




## Public Static Functions inherited from AGE::GraphicsContext

See [AGE::GraphicsContext](class_a_g_e_1_1_graphics_context.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) &gt; | [**Create**](class_a_g_e_1_1_graphics_context.md#function-create) (void \* Window) <br>_Creates a graphics context based on the current renderer API._  |


















































## Detailed Description




**Parameters:**


* `WindowHandle` A pointer to an existing GLFWwindow object that this context will be bound to.

This class represents an OpenGL context. It is responsible for initializing and managing the OpenGL pipeline.




**Parameters:**


* `WindowHandle` A pointer to a GLFWwindow object, which represents the window that this context will be associated with. 




    
## Public Functions Documentation




### function GetPipeline 

_Get the pipeline object associated with this context._ 
```C++
OpenGLPipeline * AGE::OpenGLContext::GetPipeline () 
```



This function returns a pointer to the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object that is currently bound to this context. The returned object can be used for rendering operations.




**Returns:**

OpenGLPipeline\* A pointer to the current [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object, or nullptr if no pipeline is set.


Get the pipeline object associated with this context.


This function returns a pointer to the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object that is currently bound to this context. The returned object can be used for rendering operations.




**Returns:**

OpenGLPipeline\* A pointer to the current [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object, or nullptr if no pipeline has been set. 





        

<hr>



### function Init 

_Initializes the OpenGL context._ 
```C++
virtual void AGE::OpenGLContext::Init () override
```



This function sets up the OpenGL context for use by making it the current context using glfwMakeContextCurrent(). It then initializes GLAD, a library that provides easy access to OpenGL functions and extensions in desktop OpenGL. The status of this initialization is checked with an assertion to ensure successful completion. Finally, information about the OpenGL implementation is logged.




**Returns:**

void 





        
Implements [*AGE::GraphicsContext::Init*](class_a_g_e_1_1_graphics_context.md#function-init)


<hr>



### function OpenGLContext 

_Constructs an_ [_**OpenGLContext**_](class_a_g_e_1_1_open_g_l_context.md) _object._
```C++
AGE::OpenGLContext::OpenGLContext (
    GLFWwindow * WindowHandle
) 
```



This constructor initializes the OpenGL context using a GLFWwindow pointer. It asserts that the window handle is not null.




**Parameters:**


* `WindowHandle` A pointer to the GLFWwindow instance for which this [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) will be created.

Constructor for [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) class.


This constructor initializes an instance of the [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) class with a GLFWwindow pointer. It asserts that the window handle is not null, logging an error if it is.




**Parameters:**


* `WindowHandle` Pointer to the GLFWwindow object. 




        

<hr>



### function SetPipeline 

_This function sets the pipeline for the OpenGL context._ 
```C++
void AGE::OpenGLContext::SetPipeline (
    OpenGLPipeline * Pipeline
) 
```





**Parameters:**


* [**Pipeline**](class_a_g_e_1_1_pipeline.md) The new OpenGL pipeline to be set.

Sets the OpenGL pipeline for rendering.


This function sets the OpenGL pipeline that will be used to render graphics. The pipeline is an object of type `OpenGLPipeline`, which encapsulates all the necessary settings and shaders to perform a full-featured 3D rendering operation.




**Parameters:**


* [**Pipeline**](class_a_g_e_1_1_pipeline.md) A pointer to the OpenGL pipeline to use for rendering. 




        

<hr>



### function SwapBuffers 

_Swaps the front and back buffers of the specified window._ 
```C++
virtual void AGE::OpenGLContext::SwapBuffers () override
```



This function is used to swap the front and back buffers of a window when rendering, effectively displaying what has been rendered. The behavior of this function depends on the specific implementation of the OpenGL library being used.




**Returns:**

void


Swaps the front and back buffers of the specified window.


This function is used to swap the front and back buffers of a window when rendering, effectively displaying what has been rendered so far on the screen. The behavior of this function depends on the platform and graphics API being used. For example, it may not be necessary or possible to call this function at every frame. However, calling it once per frame ensures that the display is updated as quickly as possible. 


        
Implements [*AGE::GraphicsContext::SwapBuffers*](class_a_g_e_1_1_graphics_context.md#function-swapbuffers)


<hr>



### function ~OpenGLContext 

_Destructor for the_ [_**OpenGLContext**_](class_a_g_e_1_1_open_g_l_context.md) _class._
```C++
virtual AGE::OpenGLContext::~OpenGLContext () 
```



This function is responsible for cleaning up any resources that were acquired during the lifetime of this object, such as deleting buffers and textures. It does not perform any operations on the actual rendering context itself.


Destructor for the [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) class. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGlContext.h`

