

# Class AGE::Renderer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Renderer**](class_a_g_e_1_1_renderer.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br>_Sets the rendering API to be used by the application._  |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginScene**](#function-beginscene-12) (const [**Camera**](class_a_g_e_1_1_camera.md) & Camera, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform) <br>_Begins a 3D scene with the given camera and transformation._  |
|  void | [**BeginScene**](#function-beginscene-22) (const [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br>_Begins a new scene with the specified camera._  |
|  void | [**EndScene**](#function-endscene) () <br>_Ends the current scene rendering._  |
|  void | [**Flush**](#function-flush) () <br>_Flushes the rendering queue by calling the_ `Flush` _function of the_`RenderCommand` _class._ |
|  RendererAPI::API | [**GetAPI**](#function-getapi) () <br>_This function returns the current API being used by the renderer._  |
|  void | [**Init**](#function-init) () <br>_Initializes the renderer._  |
|  void | [**OnFramebufferResize**](#function-onframebufferresize) (uint32\_t Width, uint32\_t Height) <br>_This function is called when the framebuffer size changes. It sets the viewport to match the new dimensions._  |
|  void | [**OnWindowResize**](#function-onwindowresize) (uint32\_t Width, uint32\_t Height) <br>_This function is called when the window size is resized. It sets the viewport to match the new dimensions._  |
|  void | [**SetAPI**](#function-setapi) (RendererAPI::API Renderer) <br> |
|  void | [**Shutdown**](#function-shutdown) () <br>_Shuts down the renderer and its 2D component._  |
|  void | [**Submit**](#function-submit) () <br>_Submits a render command to the queue._  |


























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

_Sets the rendering API to be used by the application._ 
```C++
COMMENT AGE::Renderer::__pad0__;
```



This function sets the API that will be used for rendering operations in the application. The API can be one of three types: OpenGL, DirectX or Vulkan. It is important to note that this function does not handle any errors or exceptions related to invalid APIs. Therefore, it's crucial to ensure that the input value is a valid one (OpenGL, DirectX or Vulkan).




**Parameters:**


* [**Renderer**](class_a_g_e_1_1_renderer.md) The API to be set for rendering operations. It can be either RendererAPI::API::OPENGL, RendererAPI::API::DIRECTX or RendererAPI::API::VULKAN. 




        

<hr>
## Public Static Functions Documentation




### function BeginScene [1/2]

_Begins a 3D scene with the given camera and transformation._ 
```C++
static void AGE::Renderer::BeginScene (
    const Camera & Camera,
    const Matrix4D & Transform
) 
```



This function begins a new 3D scene using the provided camera and transformation matrix. It uses the [**Renderer2D::BeginScene()**](class_a_g_e_1_1_renderer2_d.md#function-beginscene-12) method to do this, passing in the camera and transform as parameters.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) The camera used for rendering the scene. 
* `Transform` The transformation matrix applied to the scene objects.



**Returns:**

void No return value is expected.


Begins a new scene with the given camera and transformation.


This function begins a new rendering scene using the provided camera and transformation matrix. It uses [**Renderer2D::BeginScene**](class_a_g_e_1_1_renderer2_d.md#function-beginscene-12) to start the scene, which is expected to handle the actual setup of the scene.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) The camera that will be used for this scene. 
* `Transform` The transformation matrix that will be applied to everything in this scene. 




        

<hr>



### function BeginScene [2/2]

_Begins a new scene with the specified camera._ 
```C++
static void AGE::Renderer::BeginScene (
    const EditorCamera & Camera
) 
```



This function begins a new rendering scene using the provided [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) object. It utilizes the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) class to begin the scene, which allows for efficient rendering of 2D graphics.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) The editor camera that will be used in this scene.

Begins a new scene with the specified camera.


This function begins a new rendering scene using the provided [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) object. It uses [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md)'s BeginScene method to start the scene, passing in the camera as an argument.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) The editor camera that will be used for this scene. 




        

<hr>



### function EndScene 

_Ends the current scene rendering._ 
```C++
static void AGE::Renderer::EndScene () 
```



This function is used to end the current scene rendering by calling the `EndScene` method of the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) class. It does not take any parameters and returns void.




**Returns:**

None


Ends the current scene rendering.


This function is used to end the current scene rendering by calling the `EndScene` method of the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) class. It does not take any parameters and returns void. 


        

<hr>



### function Flush 

_Flushes the rendering queue by calling the_ `Flush` _function of the_`RenderCommand` _class._
```C++
static void AGE::Renderer::Flush () 
```



This function is used to clear the rendering queue and ensure that all previous render commands are executed before any new ones are added. It calls the `Flush` function from the `RenderCommand` class, which should handle the actual flushing process.


Flushes the rendering queue.


This function is used to flush the rendering queue by calling the `Flush` method of the [**RenderCommand**](class_a_g_e_1_1_render_command.md) class. It ensures that all pending render commands are executed immediately, without waiting for a new command to be added. 


        

<hr>



### function GetAPI 

_This function returns the current API being used by the renderer._ 
```C++
static inline RendererAPI::API AGE::Renderer::GetAPI () 
```





**Returns:**

The enum value representing the currently active API (RendererAPI::OpenGL, RendererAPI::Vulkan, etc.).


This function returns the current API being used by the renderer. 

**Returns:**

The enum value representing the current API, which can be either RendererAPI::None, RendererAPI::OpenGL, or RendererAPI::DirectX. 





        

<hr>



### function Init 

_Initializes the renderer._ 
```C++
static void AGE::Renderer::Init () 
```



This function initializes various subsystems of the renderer, including [**RenderCommand**](class_a_g_e_1_1_render_command.md) and [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md). It uses AGE\_PROFILE\_FUNCTION to record its performance.




**Returns:**

void


Initializes the renderer.


This function initializes the renderer by calling the Init function from [**RenderCommand**](class_a_g_e_1_1_render_command.md) class. It is used to prepare the renderer for rendering operations.




**Returns:**

void 





        

<hr>



### function OnFramebufferResize 

_This function is called when the framebuffer size changes. It sets the viewport to match the new dimensions._ 
```C++
static void AGE::Renderer::OnFramebufferResize (
    uint32_t Width,
    uint32_t Height
) 
```





**Parameters:**


* `Width` The width of the new framebuffer in pixels. 
* `Height` The height of the new framebuffer in pixels.

This function is called when the framebuffer size changes. It sets the viewport to match the new dimensions. 

**Parameters:**


* `Width` The width of the new framebuffer in pixels. 
* `Height` The height of the new framebuffer in pixels. 




        

<hr>



### function OnWindowResize 

_This function is called when the window size is resized. It sets the viewport to match the new dimensions._ 
```C++
static void AGE::Renderer::OnWindowResize (
    uint32_t Width,
    uint32_t Height
) 
```





**Parameters:**


* `Width` The new width of the window in pixels. 
* `Height` The new height of the window in pixels.

This function is used to handle the window resize event. It sets the viewport size based on the provided width and height parameters. 

**Parameters:**


* `Width` The new width of the window. 
* `Height` The new height of the window. 




        

<hr>



### function SetAPI 

```C++
static inline void AGE::Renderer::SetAPI (
    RendererAPI::API Renderer
) 
```




<hr>



### function Shutdown 

_Shuts down the renderer and its 2D component._ 
```C++
static void AGE::Renderer::Shutdown () 
```



This function is used to clean up resources held by the [**Renderer**](class_a_g_e_1_1_renderer.md) and its associated [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) component. It should be called when shutting down the application or before initializing a new scene.




**Returns:**

void


Shuts down the renderer and its 2D component.


This function is used to clean up resources held by the [**Renderer**](class_a_g_e_1_1_renderer.md) and its associated [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) component. It should be called when shutting down the application or before initializing a new scene.




**Returns:**

void 





        

<hr>



### function Submit 

_Submits a render command to the queue._ 
```C++
static void AGE::Renderer::Submit () 
```



This function submits a render command to the rendering system's queue, which will be processed and executed at some point in the future. The specific behavior of this function is not specified as it depends on the implementation details of the [**Renderer**](class_a_g_e_1_1_renderer.md) class and its associated [**RenderCommand**](class_a_g_e_1_1_render_command.md) classes.




**Returns:**

void


Submits the current render command to be processed by the renderer.


This function submits a render command for processing by the [**Renderer**](class_a_g_e_1_1_renderer.md) class. It uses the [**RenderCommand::Submit()**](class_a_g_e_1_1_render_command.md#function-submit) method, which is responsible for adding the command to the queue of commands that need to be processed.




**Returns:**

void No return value. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Renderer.h`

