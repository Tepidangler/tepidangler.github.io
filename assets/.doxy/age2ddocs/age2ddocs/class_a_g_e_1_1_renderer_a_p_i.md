

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
| virtual void | [**DrawArrays**](#function-drawarrays) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
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
| virtual  | [**~RendererAPI**](#function-rendererapi) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) &gt; | [**Create**](#function-create) () <br> |
|  API | [**GetAPI**](#function-getapi) () <br> |
|  void | [**SetAPI**](#function-setapi) (RendererAPI::API Type) <br> |


























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



### function DrawArrays 

```C++
virtual void AGE::RendererAPI::DrawArrays (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) = 0
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

```C++
virtual AGE::RendererAPI::~RendererAPI () = default
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Scope< RendererAPI > AGE::RendererAPI::Create () 
```




<hr>



### function GetAPI 

```C++
static inline API AGE::RendererAPI::GetAPI () 
```




<hr>



### function SetAPI 

```C++
static inline void AGE::RendererAPI::SetAPI (
    RendererAPI::API Type
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderAPI.h`

