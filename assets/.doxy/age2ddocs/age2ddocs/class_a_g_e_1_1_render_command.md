

# Class AGE::RenderCommand



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RenderCommand**](class_a_g_e_1_1_render_command.md)




























## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Pipeline**](class_a_g_e_1_1_pipeline.md) &gt; | [**s\_GraphicsPipeline**](#variable-s_graphicspipeline)   = `nullptr`<br> |
















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Clear**](#function-clear) () <br> |
|  void | [**DrawArray**](#function-drawarray) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount=0) <br> |
|  void | [**DrawIndexed**](#function-drawindexed-12) (uint32\_t IndexCount, uint32\_t IndexStart, int VertexStart) <br> |
|  void | [**DrawIndexed**](#function-drawindexed-22) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t IndexCount=0) <br> |
|  void | [**DrawLines**](#function-drawlines) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount=0) <br> |
|  void | [**DrawStrips**](#function-drawstrips) (const Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; & VertexArray, uint32\_t VertexCount=0) <br> |
|  void | [**Flush**](#function-flush) () <br> |
|  RendererAPI::API & | [**GetCurrentRendererAPI**](#function-getcurrentrendererapi) () <br> |
|  void | [**Init**](#function-init) () <br> |
|  void | [**Present**](#function-present) () <br> |
|  void | [**ResetStats**](#function-resetstats) () <br> |
|  void | [**SetClearColor**](#function-setclearcolor) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) Color) <br> |
|  void | [**SetLineWidth**](#function-setlinewidth) (float Width) <br> |
|  void | [**SetViewport**](#function-setviewport) (uint32\_t x, uint32\_t y, uint32\_t Width, uint32\_t Height) <br> |
|  void | [**Submit**](#function-submit) () <br> |


























## Public Static Attributes Documentation




### variable s\_GraphicsPipeline 

```C++
Ref< Pipeline > AGE::RenderCommand::s_GraphicsPipeline;
```




<hr>
## Public Static Functions Documentation




### function Clear 

```C++
static void AGE::RenderCommand::Clear () 
```




<hr>



### function DrawArray 

```C++
static inline void AGE::RenderCommand::DrawArray (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount=0
) 
```




<hr>



### function DrawIndexed [1/2]

```C++
static inline void AGE::RenderCommand::DrawIndexed (
    uint32_t IndexCount,
    uint32_t IndexStart,
    int VertexStart
) 
```




<hr>



### function DrawIndexed [2/2]

```C++
static inline void AGE::RenderCommand::DrawIndexed (
    const Ref< VertexArray > & VertexArray,
    uint32_t IndexCount=0
) 
```




<hr>



### function DrawLines 

```C++
static inline void AGE::RenderCommand::DrawLines (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount=0
) 
```




<hr>



### function DrawStrips 

```C++
static inline void AGE::RenderCommand::DrawStrips (
    const Ref< VertexArray > & VertexArray,
    uint32_t VertexCount=0
) 
```




<hr>



### function Flush 

```C++
static void AGE::RenderCommand::Flush () 
```




<hr>



### function GetCurrentRendererAPI 

```C++
static inline RendererAPI::API & AGE::RenderCommand::GetCurrentRendererAPI () 
```




<hr>



### function Init 

```C++
static void AGE::RenderCommand::Init () 
```




<hr>



### function Present 

```C++
static void AGE::RenderCommand::Present () 
```




<hr>



### function ResetStats 

```C++
static void AGE::RenderCommand::ResetStats () 
```




<hr>



### function SetClearColor 

```C++
static void AGE::RenderCommand::SetClearColor (
    const Vector4 Color
) 
```




<hr>



### function SetLineWidth 

```C++
static inline void AGE::RenderCommand::SetLineWidth (
    float Width
) 
```




<hr>



### function SetViewport 

```C++
static void AGE::RenderCommand::SetViewport (
    uint32_t x,
    uint32_t y,
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function Submit 

```C++
static void AGE::RenderCommand::Submit () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderCommand.h`

