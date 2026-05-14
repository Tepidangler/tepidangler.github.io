

# Class AGE::RenderCommand



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RenderCommand**](class_a_g_e_1_1_render_command.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Clear**](#function-clear) () <br>_Clears the rendering buffer._  |
|  void | [**DrawIndexed**](#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) <br>_Draw a set of indexed vertices._  |
|  void | [**DrawIndexed**](#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount=0) <br>_DrawIndexed is a function that renders the vertices of a_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) _Array using indices._ |
|  void | [**DrawLines**](#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount=0) <br>_Draw lines using the specified vertex array and count._  |
|  void | [**DrawStrips**](#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount=0) <br>_DrawStrips is a function that draws vertex strips using the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API._ |
|  void | [**Flush**](#function-flush) () <br>_This function is used to flush the rendering commands in the renderer API. It calls the Flush method of the s\_RendererAPI object, which should handle flushing all pending rendering commands._  |
|  RendererAPI::API & | [**GetCurrentRendererAPI**](#function-getcurrentrendererapi) () <br>_This function returns the current renderer API being used by the application._  |
|  void | [**Init**](#function-init) () <br>_Initializes the_ [_**RenderCommand**_](class_a_g_e_1_1_render_command.md) _. This includes setting up the renderer API, current API, and creating a graphics pipeline based on the type of API in use._ |
|  void | [**Present**](#function-present) () <br>_This function is used to present the current frame buffer on screen._  |
|  void | [**ResetStats**](#function-resetstats) () <br>_Resets the graphics pipeline statistics._  |
|  void | [**SetClearColor**](#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) <br>_Sets the clear color for the renderer._  |
|  void | [**SetLineWidth**](#function-setlinewidth) (float Width) <br>_This function sets the line width for rendering purposes._  |
|  void | [**SetViewport**](#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) <br>_Set the viewport dimensions._  |
|  void | [**Submit**](#function-submit) () <br>_Submits the command to be processed by the renderer API._  |


























## Public Static Functions Documentation




### function Clear 

_Clears the rendering buffer._ 
```C++
static void AGE::RenderCommand::Clear () 
```



This function calls the Clear method of the currently bound [**Renderer**](class_a_g_e_1_1_renderer.md) API, which is responsible for clearing the rendering buffer. It's typically used to prepare the framebuffer for a new render pass.




**Returns:**

void


Clears the rendering buffer.


This function calls the Clear method of the currently bound [**Renderer**](class_a_g_e_1_1_renderer.md) API, which is responsible for clearing the rendering buffer. The specifics of this operation are dependent on the concrete implementation of the [**Renderer**](class_a_g_e_1_1_renderer.md) API in use. 


        

<hr>



### function DrawIndexed [1/2]

_Draw a set of indexed vertices._ 
```C++
static inline void AGE::RenderCommand::DrawIndexed (
    uint32_t IndexCount,
    uint32_t IndexStart,
    int VertexStart
) 
```



This function is used to draw a subset of the vertices in the vertex buffer using indices from the index buffer. The number of indices to be drawn, starting index and starting vertex position are specified as parameters.




**Parameters:**


* `IndexCount` Number of indices to be drawn. 
* `IndexStart` Starting index location in the index buffer. 
* `VertexStart` Starting vertex position in the vertex buffer.

DrawIndexed is a function that draws indexed vertices.


This function uses the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) to draw indexed vertices on the screen. The number of indices to be drawn, their starting position and the starting vertex are provided as parameters.




**Parameters:**


* `IndexCount` The number of indices to be drawn. 
* `IndexStart` The starting position of the indices in the index buffer. 
* `VertexStart` The starting vertex for the draw call.



**Returns:**

void 





        

<hr>



### function DrawIndexed [2/2]

_DrawIndexed is a function that renders the vertices of a_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) _Array using indices._
```C++
static inline void AGE::RenderCommand::DrawIndexed (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount=0
) 
```





**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**Vertex**](struct_a_g_e_1_1_vertex.md) Array object. This represents the vertex data to be rendered. 
* `IndexCount` An unsigned integer value representing the number of indices to draw. If no index count is specified, it defaults to 0 and all vertices are drawn.

DrawIndexed function is used to render a set of vertices using indices.


This function takes in a constant reference to a [**VertexArray**](class_a_g_e_1_1_vertex_array.md) and an unsigned integer for the index count. If no index count is provided, it defaults to 0. The function uses the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md)'s DrawIndexed method to perform the rendering.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A constant reference to the [**VertexArray**](class_a_g_e_1_1_vertex_array.md) that contains the vertices to be rendered. 
* `IndexCount` An unsigned integer representing the number of indices in the index buffer. Default is 0. 




        

<hr>



### function DrawLines 

_Draw lines using the specified vertex array and count._ 
```C++
static inline void AGE::RenderCommand::DrawLines (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount=0
) 
```



This function uses the [**Renderer**](class_a_g_e_1_1_renderer.md) API to draw lines based on the provided vertex array and count. If no vertex count is provided (0), it defaults to drawing all vertices in the array.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**Vertex**](struct_a_g_e_1_1_vertex.md) Array object representing the data for the lines to be drawn. 
* `VertexCount` An unsigned integer value indicating the number of vertices to draw from the vertex array. If not provided, it defaults to drawing all vertices in the array.



**Returns:**

void


Draw lines using the specified vertex array and count.


This function uses the [**Renderer**](class_a_g_e_1_1_renderer.md) API to draw lines based on the provided vertex array and count. If no count is provided (0), it will default to drawing all vertices in the array.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**Vertex**](struct_a_g_e_1_1_vertex.md) Array object that contains the data for the lines to be drawn. 
* `VertexCount` The number of vertices to draw from the vertex array. If not provided (0), it will default to drawing all vertices in the array. 




        

<hr>



### function DrawStrips 

_DrawStrips is a function that draws vertex strips using the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API._
```C++
static inline void AGE::RenderCommand::DrawStrips (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount=0
) 
```





**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**Vertex**](struct_a_g_e_1_1_vertex.md) Array object which represents the data of the vertices to be drawn. 
* `VertexCount` An unsigned integer value representing the number of vertices to draw. If no value is provided, it defaults to 0.

DrawStrips is a function that draws vertex strips using the [**Renderer**](class_a_g_e_1_1_renderer.md) API.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object. This represents the vertex array to be drawn. 
* `VertexCount` An unsigned integer value representing the number of vertices in the vertex array. If no value is provided, it defaults to 0. 




        

<hr>



### function Flush 

_This function is used to flush the rendering commands in the renderer API. It calls the Flush method of the s\_RendererAPI object, which should handle flushing all pending rendering commands._ 
```C++
static void AGE::RenderCommand::Flush () 
```





**Returns:**

void No return value expected.


This function flushes the renderer API buffer.


The function calls the Flush method of the s\_RendererAPI object, which is presumably responsible for clearing or emptying any buffers that have been filled by rendering operations in previous frames. It does not take any parameters and returns void. 


        

<hr>



### function GetCurrentRendererAPI 

_This function returns the current renderer API being used by the application._ 
```C++
static inline RendererAPI::API & AGE::RenderCommand::GetCurrentRendererAPI () 
```





**Returns:**

A reference to the current renderer API (either RendererAPI::OpenGL, RendererAPI::Vulkan or RendererAPI::Unknown).


This function returns the current renderer API being used by the application. 

**Returns:**

A reference to the current renderer API (either OpenGL, DirectX or Vulkan). 





        

<hr>



### function Init 

_Initializes the_ [_**RenderCommand**_](class_a_g_e_1_1_render_command.md) _. This includes setting up the renderer API, current API, and creating a graphics pipeline based on the type of API in use._
```C++
static void AGE::RenderCommand::Init () 
```



The function uses a switch-case statement to determine which API is currently being used. If it's OpenGL (API value 1), it sets the pipeline for the OpenGL context and initializes the graphics pipeline. If an unsupported API is detected, an error message is logged.




**Returns:**

void 





        

<hr>



### function Present 

_This function is used to present the current frame buffer on screen._ 
```C++
static void AGE::RenderCommand::Present () 
```



The function calls the Present method of the s\_RendererAPI object, which should handle presenting the current frame buffer on screen.


This function is used to present the current frame buffer for display.


It calls the Present method of the s\_RendererAPI object, which should handle presenting the frame buffer on the target platform. 


        

<hr>



### function ResetStats 

_Resets the graphics pipeline statistics._ 
```C++
static void AGE::RenderCommand::ResetStats () 
```



This function is used to reset all the statistics related to the graphics pipeline. It calls the `ResetStats` method on the global instance of `GraphicsPipeline`, which resets any accumulated data or counters for rendering performance tracking.




**Returns:**

void


Resets the graphics pipeline statistics.


This function is used to reset all the statistics related to the graphics pipeline. It calls the `ResetStats` method on the global instance of `GraphicsPipeline`. 


        

<hr>



### function SetClearColor 

_Sets the clear color for the renderer._ 
```C++
static void AGE::RenderCommand::SetClearColor (
    const Vector4 Color
) 
```



This function sets the clear color used by the renderer to clear the frame buffer before rendering each new frame. The color is specified as a [**Vector4**](struct_a_g_e_1_1_vector4.md) with components in the range [0,1].




**Parameters:**


* `Color` The new clear color.

Sets the clear color for the renderer.


This function sets the clear color used by the renderer to clear the frame buffer before rendering a new frame. The color is specified as a [**Vector4**](struct_a_g_e_1_1_vector4.md) with components in the range [0,1].




**Parameters:**


* `Color` A [**Vector4**](struct_a_g_e_1_1_vector4.md) specifying the red, green, blue and alpha values of the clear color. Each component should be in the range [0,1].



**Returns:**

void 





        

<hr>



### function SetLineWidth 

_This function sets the line width for rendering purposes._ 
```C++
static inline void AGE::RenderCommand::SetLineWidth (
    float Width
) 
```





**Parameters:**


* `Width` The new line width to be set.

This function sets the line width for rendering purposes.




**Parameters:**


* `Width` The new line width to be set. 




        

<hr>



### function SetViewport 

_Set the viewport dimensions._ 
```C++
static void AGE::RenderCommand::SetViewport (
    uint32_t x,
    uint32_t y,
    uint32_t Width,
    uint32_t Height
) 
```



This function sets the dimensions of the viewport in pixels. The viewport is a rectangular area within which to render.




**Parameters:**


* `x` The x-coordinate of the lower left corner of the viewport. 
* `y` The y-coordinate of the lower left corner of the viewport. 
* `Width` The width of the viewport in pixels. 
* `Height` The height of the viewport in pixels.

Set the viewport for rendering.


This function sets the viewport dimensions for the renderer API. The viewport is a rectangle in the framebuffer that specifies what part of the framebuffer should be rendered to.




**Parameters:**


* `x` The x-coordinate, indicating the left side of the viewport. 
* `y` The y-coordinate, indicating the top side of the viewport. 
* `Width` The width of the viewport. 
* `Height` The height of the viewport. 




        

<hr>



### function Submit 

_Submits the command to be processed by the renderer API._ 
```C++
static void AGE::RenderCommand::Submit () 
```



This function submits a command for processing by the [**Renderer**](class_a_g_e_1_1_renderer.md) API, which is responsible for managing and executing all rendering operations. The specifics of this submission process are handled internally by the [**Renderer**](class_a_g_e_1_1_renderer.md) API, so it's not necessary to understand these details in order to use this function.




**Returns:**

void


Submits the command to be processed by the renderer API.


This function submits a command for processing by the [**Renderer**](class_a_g_e_1_1_renderer.md) API, which is responsible for rendering and managing graphics resources. The specifics of what this means will depend on the implementation of the [**Renderer**](class_a_g_e_1_1_renderer.md) API in use.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderCommand.h`

