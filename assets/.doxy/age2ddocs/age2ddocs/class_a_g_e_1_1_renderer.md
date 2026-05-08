

# Class AGE::Renderer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Renderer**](class_a_g_e_1_1_renderer.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginScene**](#function-beginscene-12) (const [**Camera**](class_a_g_e_1_1_camera.md) & Camera, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform) <br> |
|  void | [**BeginScene**](#function-beginscene-22) (const [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br> |
|  void | [**EndScene**](#function-endscene) () <br> |
|  void | [**Flush**](#function-flush) () <br> |
|  RendererAPI::API | [**GetAPI**](#function-getapi) () <br> |
|  void | [**Init**](#function-init) () <br> |
|  void | [**OnFramebufferResize**](#function-onframebufferresize) (uint32\_t Width, uint32\_t Height) <br> |
|  void | [**OnWindowResize**](#function-onwindowresize) (uint32\_t Width, uint32\_t Height) <br> |
|  void | [**SetAPI**](#function-setapi) (RendererAPI::API Renderer) <br> |
|  void | [**Shutdown**](#function-shutdown) () <br> |
|  void | [**Submit**](#function-submit) () <br> |


























## Public Static Functions Documentation




### function BeginScene [1/2]

```C++
static void AGE::Renderer::BeginScene (
    const Camera & Camera,
    const Matrix4D & Transform
) 
```




<hr>



### function BeginScene [2/2]

```C++
static void AGE::Renderer::BeginScene (
    const EditorCamera & Camera
) 
```




<hr>



### function EndScene 

```C++
static void AGE::Renderer::EndScene () 
```




<hr>



### function Flush 

```C++
static void AGE::Renderer::Flush () 
```




<hr>



### function GetAPI 

```C++
static inline RendererAPI::API AGE::Renderer::GetAPI () 
```




<hr>



### function Init 

```C++
static void AGE::Renderer::Init () 
```




<hr>



### function OnFramebufferResize 

```C++
static void AGE::Renderer::OnFramebufferResize (
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function OnWindowResize 

```C++
static void AGE::Renderer::OnWindowResize (
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function SetAPI 

```C++
static inline void AGE::Renderer::SetAPI (
    RendererAPI::API Renderer
) 
```




<hr>



### function Shutdown 

```C++
static void AGE::Renderer::Shutdown () 
```




<hr>



### function Submit 

```C++
static void AGE::Renderer::Submit () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Renderer.h`

