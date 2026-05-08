

# Class AGE::GraphicsContext



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md)










Inherited by the following classes: [AGE::OpenGLContext](class_a_g_e_1_1_open_g_l_context.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br> |
|  [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) \* | [**As**](#function-as-22) () <br> |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual void | [**SwapBuffers**](#function-swapbuffers) () = 0<br> |
| virtual  | [**~GraphicsContext**](#function-graphicscontext) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) &gt; | [**Create**](#function-create) (void \* Window) <br> |


























## Public Functions Documentation




### function As [1/2]

```C++
template<typename T>
T * AGE::GraphicsContext::As () 
```




<hr>



### function As [2/2]

```C++
template<>
OpenGLContext * AGE::GraphicsContext::As () 
```




<hr>



### function Init 

```C++
virtual void AGE::GraphicsContext::Init () = 0
```




<hr>



### function SwapBuffers 

```C++
virtual void AGE::GraphicsContext::SwapBuffers () = 0
```




<hr>



### function ~GraphicsContext 

```C++
inline virtual AGE::GraphicsContext::~GraphicsContext () 
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Scope< GraphicsContext > AGE::GraphicsContext::Create (
    void * Window
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/GraphicsContext.h`

