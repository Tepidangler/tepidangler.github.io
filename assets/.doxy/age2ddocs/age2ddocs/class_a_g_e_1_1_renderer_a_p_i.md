

# Class AGE::RendererAPI



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md)










Inherited by the following classes: [AGE::OpenGLRendererAPI](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md)












## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**API**](#enum-api)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Clear**](#function-clear) () = 0<br> |
| virtual void | [**DrawIndexed**](#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) = 0<br> |
| virtual void | [**DrawIndexed**](#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
| virtual void | [**DrawLines**](#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount) = 0<br> |
| virtual void | [**DrawStrips**](#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
| virtual void | [**Flush**](#function-flush) () = 0<br> |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual void | [**Present**](#function-present) () = 0<br> |
| virtual void | [**SetClearColor**](#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) = 0<br> |
| virtual void | [**SetLineWidth**](#function-setlinewidth) (float Width) = 0<br> |
| virtual void | [**SetViewport**](#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) = 0<br> |
| virtual void | [**Submit**](#function-submit) () = 0<br> |
| virtual  | [**~RendererAPI**](#function-rendererapi) () = default<br>_Virtual destructor for_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) &gt; | [**Create**](#function-create) () <br>_Creates a new instance of the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _based on the current setting._ |
|  API | [**GetAPI**](#function-getapi) () <br>_This function returns the current API object used by the application._  |
|  void | [**SetAPI**](#function-setapi) (RendererAPI::API Type) <br>_This function sets the API type for the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._ |


























## Public Types Documentation




### enum API 

```C++
enum AGE::RendererAPI::API {
    Headless = 0,
    OpenGL = 1
};
```




<hr>
## Public Functions Documentation




### function Clear 

```C++
virtual void AGE::RendererAPI::Clear () = 0
```




<hr>



### function DrawIndexed [1/2]

```C++
virtual void AGE::RendererAPI::DrawIndexed (
    uint32_t IndexCount,
    uint32_t IndexStart,
    int VertexStart
) = 0
```




<hr>



### function DrawIndexed [2/2]

```C++
virtual void AGE::RendererAPI::DrawIndexed (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) = 0
```




<hr>



### function DrawLines 

```C++
virtual void AGE::RendererAPI::DrawLines (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount
) = 0
```




<hr>



### function DrawStrips 

```C++
virtual void AGE::RendererAPI::DrawStrips (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) = 0
```




<hr>



### function Flush 

```C++
virtual void AGE::RendererAPI::Flush () = 0
```




<hr>



### function Init 

```C++
virtual void AGE::RendererAPI::Init () = 0
```




<hr>



### function Present 

```C++
virtual void AGE::RendererAPI::Present () = 0
```




<hr>



### function SetClearColor 

```C++
virtual void AGE::RendererAPI::SetClearColor (
    const Vector4 Color
) = 0
```




<hr>



### function SetLineWidth 

```C++
virtual void AGE::RendererAPI::SetLineWidth (
    float Width
) = 0
```




<hr>



### function SetViewport 

```C++
virtual void AGE::RendererAPI::SetViewport (
    uint32_t x,
    uint32_t y,
    uint32_t Width,
    uint32_t Height
) = 0
```




<hr>



### function Submit 

```C++
virtual void AGE::RendererAPI::Submit () = 0
```




<hr>



### function ~RendererAPI 

_Virtual destructor for_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._
```C++
virtual AGE::RendererAPI::~RendererAPI () = default
```



This function is responsible for freeing any resources that the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) object may have acquired during its lifetime, such as memory or graphics resources. It does not return a value and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new instance of the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _based on the current setting._
```C++
static Scope< RendererAPI > AGE::RendererAPI::Create () 
```



This function creates and returns an instance of the appropriate [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) class, depending on the currently set API. If no API is set (i.e., s\_API is None), it asserts false with a message "RendererAPI::API::None is currently not supported!". For OpenGL, it returns a new instance of [**OpenGLRendererAPI**](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md). In all other cases, it asserts false with the message "Unknown Renderer API!" and returns nullptr.




**Returns:**

Scope&lt;RendererAPI&gt; - The newly created [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) instance or nullptr if an invalid API is set.


Creates a new instance of the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) based on the current setting.


This function creates and returns an instance of either [**OpenGLRendererAPI**](class_a_g_e_1_1_open_g_l_renderer_a_p_i.md) or another type of [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md), depending on what is currently set as the API. If no valid API is set (i.e., s\_API is None), it asserts false with a message indicating that this case is not supported.




**Returns:**

Scope&lt;RendererAPI&gt; A new instance of the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md), or nullptr if an invalid API is detected. 





        

<hr>



### function GetAPI 

_This function returns the current API object used by the application._ 
```C++
static inline API AGE::RendererAPI::GetAPI () 
```





**Returns:**

The currently active API object, or "Unknown" if no API is set. 





        

<hr>



### function SetAPI 

_This function sets the API type for the_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _class._
```C++
static inline void AGE::RendererAPI::SetAPI (
    RendererAPI::API Type
) 
```





**Parameters:**


* `Type` The API type to be set, which can be one of the values defined in the RendererAPI::API enum. 



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderAPI.h`

