

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
| virtual void | [**Clear**](#function-clear) () override<br> |
| virtual void | [**DrawArrays**](#function-drawarrays) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) override<br> |
| virtual void | [**DrawIndexed**](#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) override<br> |
| virtual void | [**DrawIndexed**](#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) override<br> |
| virtual void | [**DrawLines**](#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount) override<br> |
| virtual void | [**DrawStrips**](#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) override<br> |
| virtual void | [**Flush**](#function-flush) () override<br> |
| virtual void | [**Init**](#function-init) () override<br> |
| virtual void | [**Present**](#function-present) () override<br> |
| virtual void | [**SetClearColor**](#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) override<br> |
| virtual void | [**SetLineWidth**](#function-setlinewidth) (float Width) override<br> |
| virtual void | [**SetViewport**](#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) override<br> |
| virtual void | [**Submit**](#function-submit) () override<br> |
|   | [**~OpenGLRendererAPI**](#function-openglrendererapi) () = default<br> |


## Public Functions inherited from AGE::RendererAPI

See [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**Clear**](class_a_g_e_1_1_renderer_a_p_i.md#function-clear) () = 0<br> |
| virtual void | [**DrawArrays**](class_a_g_e_1_1_renderer_a_p_i.md#function-drawarrays) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount) = 0<br> |
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
| virtual  | [**~RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-rendererapi) () = default<br> |




## Public Static Functions inherited from AGE::RendererAPI

See [AGE::RendererAPI](class_a_g_e_1_1_renderer_a_p_i.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) &gt; | [**Create**](class_a_g_e_1_1_renderer_a_p_i.md#function-create) () <br> |
|  API | [**GetAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-getapi) () <br> |
|  void | [**SetAPI**](class_a_g_e_1_1_renderer_a_p_i.md#function-setapi) (RendererAPI::API Type) <br> |


















































## Public Functions Documentation




### function Clear 

```C++
virtual void AGE::OpenGLRendererAPI::Clear () override
```



Implements [*AGE::RendererAPI::Clear*](class_a_g_e_1_1_renderer_a_p_i.md#function-clear)


<hr>



### function DrawArrays 

```C++
virtual void AGE::OpenGLRendererAPI::DrawArrays (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) override
```



Implements [*AGE::RendererAPI::DrawArrays*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawarrays)


<hr>



### function DrawIndexed [1/2]

```C++
inline virtual void AGE::OpenGLRendererAPI::DrawIndexed (
    uint32_t IndexCount,
    uint32_t IndexStart,
    int VertexStart
) override
```



Implements [*AGE::RendererAPI::DrawIndexed*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-12)


<hr>



### function DrawIndexed [2/2]

```C++
virtual void AGE::OpenGLRendererAPI::DrawIndexed (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) override
```



Implements [*AGE::RendererAPI::DrawIndexed*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawindexed-22)


<hr>



### function DrawLines 

```C++
virtual void AGE::OpenGLRendererAPI::DrawLines (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount
) override
```



Implements [*AGE::RendererAPI::DrawLines*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawlines)


<hr>



### function DrawStrips 

```C++
virtual void AGE::OpenGLRendererAPI::DrawStrips (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount
) override
```



Implements [*AGE::RendererAPI::DrawStrips*](class_a_g_e_1_1_renderer_a_p_i.md#function-drawstrips)


<hr>



### function Flush 

```C++
virtual void AGE::OpenGLRendererAPI::Flush () override
```



Implements [*AGE::RendererAPI::Flush*](class_a_g_e_1_1_renderer_a_p_i.md#function-flush)


<hr>



### function Init 

```C++
virtual void AGE::OpenGLRendererAPI::Init () override
```



Implements [*AGE::RendererAPI::Init*](class_a_g_e_1_1_renderer_a_p_i.md#function-init)


<hr>



### function Present 

```C++
virtual void AGE::OpenGLRendererAPI::Present () override
```



This Function Currently Fails silently since there is really no use for them however because of how pure virtual classes work it has to be here to compile 


        
Implements [*AGE::RendererAPI::Present*](class_a_g_e_1_1_renderer_a_p_i.md#function-present)


<hr>



### function SetClearColor 

```C++
virtual void AGE::OpenGLRendererAPI::SetClearColor (
    const Vector4 Color
) override
```



Implements [*AGE::RendererAPI::SetClearColor*](class_a_g_e_1_1_renderer_a_p_i.md#function-setclearcolor)


<hr>



### function SetLineWidth 

```C++
virtual void AGE::OpenGLRendererAPI::SetLineWidth (
    float Width
) override
```



Implements [*AGE::RendererAPI::SetLineWidth*](class_a_g_e_1_1_renderer_a_p_i.md#function-setlinewidth)


<hr>



### function SetViewport 

```C++
virtual void AGE::OpenGLRendererAPI::SetViewport (
    uint32_t x,
    uint32_t y,
    uint32_t Width,
    uint32_t Height
) override
```



Implements [*AGE::RendererAPI::SetViewport*](class_a_g_e_1_1_renderer_a_p_i.md#function-setviewport)


<hr>



### function Submit 

```C++
virtual void AGE::OpenGLRendererAPI::Submit () override
```



This Function Currently Fails silently since there is really no use for them however because of how pure virtual classes work it has to be here to compile 


        
Implements [*AGE::RendererAPI::Submit*](class_a_g_e_1_1_renderer_a_p_i.md#function-submit)


<hr>



### function ~OpenGLRendererAPI 

```C++
AGE::OpenGLRendererAPI::~OpenGLRendererAPI () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLRendererAPI.h`

