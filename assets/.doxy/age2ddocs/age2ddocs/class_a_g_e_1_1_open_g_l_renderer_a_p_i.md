

# Class AGE::OpenGLRendererAPI



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLRendererAPI**](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md)








Inherits the following classes: [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)
















## Public Types inherited from AGE::RendererAPI

See [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)

| Type | Name |
| ---: | :--- |
| enum  | [**API**](class_a_g_e_1_1_renderer_a_p_i.md#enum-api)  <br> |






































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Clear**](#function-clear) () override<br>_Clears the color and depth buffers of the OpenGL context._  |
| virtual void | [**DrawIndexed**](#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) override<br>_This function is used to draw indexed elements in a graphics context._  |
| virtual void | [**DrawIndexed**](#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) override<br>_Draws an indexed element array._  |
| virtual void | [**DrawLines**](#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount) override<br>_Draws a series of lines defined by the given vertex array._  |
| virtual void | [**DrawStrips**](#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) override<br>_DrawStrips is a function that draws triangle strips using OpenGL._  |
| virtual void | [**Flush**](#function-flush) () override<br>_This function flushes the OpenGL command buffer. It ensures that all commands issued up to this point are executed immediately, without buffering them for later execution._  |
| virtual void | [**Init**](#function-init) () override<br>_Initializes the OpenGL_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API with various settings for rendering._ |
| virtual void | [**Present**](#function-present) () override<br>_This function is used to present the rendered scene to the screen. It does not take any parameters and returns void, indicating that it has completed its operation without returning a value._  |
| virtual void | [**SetClearColor**](#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) override<br>_This function sets the clear color for the OpenGL context._  |
| virtual void | [**SetLineWidth**](#function-setlinewidth) (float Width) override<br>_Set the line width for subsequent drawing operations._  |
| virtual void | [**SetViewport**](#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) override<br>_Set the viewport for OpenGL rendering._  |
| virtual void | [**Submit**](#function-submit) () override<br>_Submits the current frame for rendering._  |
|   | [**~OpenGLRendererAPI**](#function-openglrendererapi) () = default<br>_Default destructor for the_ [_**OpenGLRendererAPI**_](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md) _class._ |


## Public Functions inherited from AGE::RendererAPI

See [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**Clear**](class_a_g_e_1_1_renderer_a_p_i.md#function-clear) () = 0<br> |
| virtual void | [**DrawIndexed**](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) = 0<br> |
| virtual void | [**DrawIndexed**](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
| virtual void | [**DrawLines**](class_a_g_e_1_1_renderer_a_p_i.md#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount) = 0<br> |
| virtual void | [**DrawStrips**](class_a_g_e_1_1_renderer_a_p_i.md#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
| virtual void | [**Flush**](class_a_g_e_1_1_renderer_a_p_i.md#function-flush) () = 0<br> |
| virtual void | [**Init**](class_a_g_e_1_1_renderer_a_p_i.md#function-init) () = 0<br> |
| virtual void | [**Present**](class_a_g_e_1_1_renderer_a_p_i.md#function-present) () = 0<br> |
| virtual void | [**SetClearColor**](class_a_g_e_1_1_renderer_a_p_i.md#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) = 0<br> |
| virtual void | [**SetLineWidth**](class_a_g_e_1_1_renderer_a_p_i.md#function-setlinewidth) (float Width) = 0<br> |
| virtual void | [**SetViewport**](class_a_g_e_1_1_renderer_a_p_i.md#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) = 0<br> |
| virtual void | [**Submit**](class_a_g_e_1_1_renderer_a_p_i.md#function-submit) () = 0<br> |
| virtual  | [**~RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-rendererapi) () = default<br>_Virtual destructor for_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._ |




## Public Static Functions inherited from AGE::RendererAPI

See [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) &gt; | [**Create**](class_a_g_e_1_1_renderer_a_p_i.md#function-create) () <br>_Creates a new instance of the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _based on the current setting._ |
|  API | [**GetAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-getapi) () <br>_This function returns the current API object used by the application._  |
|  void | [**SetAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-setapi) (RendererAPI::API Type) <br>_This function sets the API type for the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._ |


















































## Public Functions Documentation




### function Clear 

_Clears the color and depth buffers of the OpenGL context._ 
```C++
virtual void AGE::OpenGLRendererAPI::Clear () override
```



This function uses glClear to clear both the color and depth buffer bits, indicating that all pixels in these buffers should be cleared. The color buffer is typically filled with black (0, 0, 0), while the depth buffer is set to maximum value.




**Returns:**

void


Clears the color and depth buffer.


This function uses OpenGL's glClear() function to clear both the color and depth buffers. The GL\_COLOR\_BUFFER\_BIT and GL\_DEPTH\_BUFFER\_BIT flags are used to specify which buffers should be cleared. 


        
Implements [*AGE::RendererAPI::Clear*](class_a_g_e_1_1_renderer_a_p_i.md#function-clear)


<hr>



### function DrawIndexed [1/2]

_This function is used to draw indexed elements in a graphics context._ 
```C++
inline virtual void AGE::OpenGLRendererAPI::DrawIndexed (
    uint32_t IndexCount,
    uint32_t IndexStart,
    int VertexStart
) override
```



The function takes three parameters: the number of indices (IndexCount), the starting index (IndexStart), and the starting vertex position (VertexStart). It does not return anything, hence void return type.




**Parameters:**


* `IndexCount` Number of indices to be drawn. 
* `IndexStart` Starting index for drawing elements. 
* `VertexStart` The starting vertex position.



**Returns:**

Nothing is returned as the function is declared with 'override' keyword, indicating it overrides a virtual function in base class.


This function draws a set of vertices using index buffers. 

**Parameters:**


* `IndexCount` The number of indices to draw from the index buffer. 
* `IndexStart` The starting index in the index buffer. 
* `VertexStart` The vertex offset within the vertex buffer. 



**Returns:**

void 





        
Implements [*AGE::RendererAPI::DrawIndexed*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-12)


<hr>



### function DrawIndexed [2/2]

_Draws an indexed element array._ 
```C++
virtual void AGE::OpenGLRendererAPI::DrawIndexed (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) override
```



This function binds the given vertex array and then draws its elements using OpenGL's glDrawElements function. The number of indices to draw is determined by either the provided IndexCount parameter or, if no such count was provided, by the count in the bound index buffer. After drawing, it unbinds any texture for safety.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a vertex array object that contains the data to be drawn. 
* `IndexCount` The number of indices to draw from the element array. If this is zero, the count in the index buffer will be used instead.



**Returns:**

void


This function is used to draw an indexed element array. It binds the vertex array and then uses OpenGL's glDrawElements function to render a set number of elements from the index buffer. 

**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object which represents the data for rendering. 
* `IndexCount` The number of indices to be drawn. If this is 0, it defaults to the count in the index buffer of the vertex array. 



**Returns:**

void 





        
Implements [*AGE::RendererAPI::DrawIndexed*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-22)


<hr>



### function DrawLines 

_Draws a series of lines defined by the given vertex array._ 
```C++
virtual void AGE::OpenGLRendererAPI::DrawLines (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount
) override
```



This function binds the provided [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object and then uses OpenGL's glDrawArrays to draw an array of vertices as line segments. The number of vertices drawn is specified by the 'VertexCount' parameter.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object that contains the vertex data for the lines to be drawn. 
* `VertexCount` The number of vertices in the [**VertexArray**](class_a_g_e_1_1_vertex_array.md) to draw.

Draws a series of lines defined by the given vertex array.


This function binds the provided [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object and then uses OpenGL's glDrawArrays to draw a series of lines, starting from the first element (index 0) and drawing 'VertexCount' number of vertices. The type of primitives drawn is specified as GL\_LINES.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object that contains the vertex data for the lines to be drawn. 
* `VertexCount` The number of vertices in the line strip or loop, i.e., the number of elements to draw.



**Returns:**

void 





        
Implements [*AGE::RendererAPI::DrawLines*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawlines)


<hr>



### function DrawStrips 

_DrawStrips is a function that draws triangle strips using OpenGL._ 
```C++
virtual void AGE::OpenGLRendererAPI::DrawStrips (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) override
```



It binds the given [**VertexArray**](class_a_g_e_1_1_vertex_array.md) and then uses glDrawElements to draw elements with GL\_TRIANGLE\_STRIP mode. If IndexCount is not provided, it will use the count from the index buffer of the [**VertexArray**](class_a_g_e_1_1_vertex_array.md). After drawing, it unbinds the texture for safety.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object that represents the vertex data to be drawn. 
* `IndexCount` The number of indices to draw. If not provided, it will use the count from the index buffer of the [**VertexArray**](class_a_g_e_1_1_vertex_array.md).

DrawStrips is a function that draws triangle strips using the OpenGL API.




**Parameters:**


* [**VertexArray**](class_a_g_e_1_1_vertex_array.md) A reference to a constant [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object which represents the vertex array data. 
* `IndexCount` An unsigned integer representing the number of indices to be drawn. If this value is zero, it defaults to the count in the index buffer of the [**VertexArray**](class_a_g_e_1_1_vertex_array.md). 




        
Implements [*AGE::RendererAPI::DrawStrips*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawstrips)


<hr>



### function Flush 

_This function flushes the OpenGL command buffer. It ensures that all commands issued up to this point are executed immediately, without buffering them for later execution._ 
```C++
virtual void AGE::OpenGLRendererAPI::Flush () override
```





**Returns:**

void


Flushes the OpenGL command queue.


This function calls glFlush(), which forces all pending commands to be executed as quickly as possible. It is useful for ensuring that certain operations are completed before proceeding with other tasks.




**Returns:**

void 





        
Implements [*AGE::RendererAPI::Flush*](class_a_g_e_1_1_renderer_a_p_i.md#function-flush)


<hr>



### function Init 

_Initializes the OpenGL_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API with various settings for rendering._
```C++
virtual void AGE::OpenGLRendererAPI::Init () override
```



This function sets up several important OpenGL states such as blending, depth testing, line smoothing and front face winding order. It enables features like blending (for transparency), depth testing (for occlusion culling) and line smoothing (for smoother lines). The blend equation is set to GL\_FUNC\_ADD for the source and destination colors, the blend function is set to use GL\_SRC\_ALPHA as the source color and GL\_ONE\_MINUS\_SRC\_ALPHA as the destination color. Depth testing is enabled with a depth function of GL\_LEQUAL which means pixels that are closer to the camera will be drawn over those that are further away. The clear depth value is set to 1.0f. [**Line**](struct_a_g_e_1_1_line.md) smoothing is enabled, and front face winding order is set to GL\_CW (counter-clockwise).




**Returns:**

void


Initializes the OpenGL [**Renderer**](class_a_g_e_1_1_renderer.md) API with various settings for rendering.


This function sets up several important OpenGL states such as blending, depth testing, line smoothing and front face winding order. It enables blending by setting the source blend factor to GL\_SRC\_ALPHA and the destination blend factor to GL\_ONE\_MINUS\_SRC\_ALPHA. Depth testing is enabled with a depth function of GL\_LEQUAL, clearing the depth buffer with glClearDepth(1.0f), and enabling line smoothing with glEnable(GL\_LINE\_SMOOTH). The front face winding order is set to GL\_CW using glFrontFace(GL\_CW).




**Returns:**

void 





        
Implements [*AGE::RendererAPI::Init*](class_a_g_e_1_1_renderer_a_p_i.md#function-init)


<hr>



### function Present 

_This function is used to present the rendered scene to the screen. It does not take any parameters and returns void, indicating that it has completed its operation without returning a value._ 
```C++
virtual void AGE::OpenGLRendererAPI::Present () override
```



This Function Currently Fails silently since there is really no use for them however because of how pure virtual classes work it has to be here to compile


This function is used to present the rendered scene to the screen. It does not take any parameters and returns void, indicating that it has completed its task without returning a value. 


        
Implements [*AGE::RendererAPI::Present*](class_a_g_e_1_1_renderer_a_p_i.md#function-present)


<hr>



### function SetClearColor 

_This function sets the clear color for the OpenGL context._ 
```C++
virtual void AGE::OpenGLRendererAPI::SetClearColor (
    const Vector4 Color
) override
```





**Parameters:**


* `Color` A [**Vector4**](struct_a_g_e_1_1_vector4.md) object representing the RGBA values of the clear color.

Set the clear color for OpenGL rendering context.


This function sets the clear color for the current OpenGL rendering context. The color is specified as a [**Vector4**](struct_a_g_e_1_1_vector4.md) with each component ranging from 0 to 1.




**Parameters:**


* `Color` A [**Vector4**](struct_a_g_e_1_1_vector4.md) specifying the red, green, blue and alpha components of the color. 




        
Implements [*AGE::RendererAPI::SetClearColor*](class_a_g_e_1_1_renderer_a_p_i.md#function-setclearcolor)


<hr>



### function SetLineWidth 

_Set the line width for subsequent drawing operations._ 
```C++
virtual void AGE::OpenGLRendererAPI::SetLineWidth (
    float Width
) override
```



This function sets the current line width to a value in pixels. The actual effect of this setting depends on the specific rendering mode and transformation matrices currently active.




**Parameters:**


* `Width` The new line width, in pixels. Must be greater than zero.

This function sets the width of lines used for rendering. 

**Parameters:**


* `Width` The new line width to be set. Must be greater than zero. 




        
Implements [*AGE::RendererAPI::SetLineWidth*](class_a_g_e_1_1_renderer_a_p_i.md#function-setlinewidth)


<hr>



### function SetViewport 

_Set the viewport for OpenGL rendering._ 
```C++
virtual void AGE::OpenGLRendererAPI::SetViewport (
    uint32_t x,
    uint32_t y,
    uint32_t Width,
    uint32_t Height
) override
```



This function sets the viewport in OpenGL to a specified width and height at a given x and y position. The coordinates are defined as integers, with (0,0) being the bottom-left corner of the window/viewport. 

**Parameters:**


* `x` The x coordinate of the lower left corner of the viewport rectangle. 
* `y` The y coordinate of the lower left corner of the viewport rectangle. 
* `Width` The width of the viewport, in pixels. 
* `Height` The height of the viewport, in pixels.



**Returns:**

void No return value is expected as this function only sets OpenGL state variables.


Set the viewport for OpenGL rendering.


This function sets the viewport in OpenGL to a specified width and height starting at coordinates (x, y). The viewport is defined as the rectangular area of the window where rendering takes place.




**Parameters:**


* `x` The x-coordinate of the lower left corner of the viewport rectangle. 
* `y` The y-coordinate of the lower left corner of the viewport rectangle. 
* `Width` The width of the viewport rectangle. 
* `Height` The height of the viewport rectangle. 




        
Implements [*AGE::RendererAPI::SetViewport*](class_a_g_e_1_1_renderer_a_p_i.md#function-setviewport)


<hr>



### function Submit 

_Submits the current frame for rendering._ 
```C++
virtual void AGE::OpenGLRendererAPI::Submit () override
```



This Function Currently Fails silently since there is really no use for them however because of how pure virtual classes work it has to be here to compile


This function submits the current frame to be rendered by the OpenGL [**Renderer**](class_a_g_e_1_1_renderer.md) API. It does not actually render anything, it just prepares everything for drawing. The actual rendering is done in the `OpenGLRendererAPI::EndScene()` function.




**Returns:**

void


Submits the current frame for rendering.


This function submits the current frame to be rendered by the OpenGL [**Renderer**](class_a_g_e_1_1_renderer.md) API. It does not actually render anything, it just prepares everything for rendering.




**Returns:**

void 





        
Implements [*AGE::RendererAPI::Submit*](class_a_g_e_1_1_renderer_a_p_i.md#function-submit)


<hr>



### function ~OpenGLRendererAPI 

_Default destructor for the_ [_**OpenGLRendererAPI**_](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md) _class._
```C++
AGE::OpenGLRendererAPI::~OpenGLRendererAPI () = default
```



This function is responsible for releasing any resources that were acquired during the lifetime of an instance of this class. It does not perform any operations on the actual objects being rendered, but rather cleans up any internal data structures or handles used by the renderer.




**Returns:**

void


Default destructor for the [**OpenGLRendererAPI**](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md) class.


This function is responsible for freeing any resources that were allocated during the lifetime of an instance of this class. It does not perform any operations on the state of the renderer itself, but rather cleans up any associated memory or other resources.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLRendererAPI.h`

