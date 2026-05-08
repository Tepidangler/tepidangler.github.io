

# Class AGE::AGEWindow



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; void([**Event**](class_a_g_e_1_1_event.md) &)&gt; | [**EventCallbackFn**](#typedef-eventcallbackfn)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
| virtual [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) \* | [**GetGraphicsContext**](#function-getgraphicscontext) () = 0<br> |
| virtual unsigned int | [**GetHeight**](#function-getheight) () const = 0<br> |
| virtual [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetMousePos**](#function-getmousepos) () = 0<br> |
| virtual void \* | [**GetNativeWindow**](#function-getnativewindow) () const = 0<br> |
| virtual unsigned int | [**GetWidth**](#function-getwidth) () const = 0<br> |
| virtual bool | [**IsVSync**](#function-isvsync) () const = 0<br> |
| virtual void | [**OnUpdate**](#function-onupdate) () = 0<br> |
| virtual void | [**RebuildWindow**](#function-rebuildwindow) () = 0<br> |
| virtual void | [**SetEventCallback**](#function-seteventcallback) (const EventCallbackFn & Callback) = 0<br> |
| virtual void | [**SetVSync**](#function-setvsync) (bool Enabled) = 0<br> |
| virtual void | [**SetWindowIcon**](#function-setwindowicon) (const std::filesystem::path & Path) = 0<br> |
| virtual void | [**SwitchRenderer**](#function-switchrenderer) () = 0<br> |
| virtual  | [**~AGEWindow**](#function-agewindow) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) &gt; | [**Create**](#function-create) (const [**WindowProps**](struct_a_g_e_1_1_window_props.md) & props=[**WindowProps**](struct_a_g_e_1_1_window_props.md)()) <br> |


























## Public Types Documentation




### typedef EventCallbackFn 

```C++
using AGE::AGEWindow::EventCallbackFn =  std::function<void(Event&)>;
```




<hr>
## Public Functions Documentation




### function GetGraphicsContext 

```C++
virtual GraphicsContext * AGE::AGEWindow::GetGraphicsContext () = 0
```




<hr>



### function GetHeight 

```C++
virtual unsigned int AGE::AGEWindow::GetHeight () const = 0
```




<hr>



### function GetMousePos 

```C++
virtual Vector2 AGE::AGEWindow::GetMousePos () = 0
```




<hr>



### function GetNativeWindow 

```C++
virtual void * AGE::AGEWindow::GetNativeWindow () const = 0
```




<hr>



### function GetWidth 

```C++
virtual unsigned int AGE::AGEWindow::GetWidth () const = 0
```




<hr>



### function IsVSync 

```C++
virtual bool AGE::AGEWindow::IsVSync () const = 0
```




<hr>



### function OnUpdate 

```C++
virtual void AGE::AGEWindow::OnUpdate () = 0
```




<hr>



### function RebuildWindow 

```C++
virtual void AGE::AGEWindow::RebuildWindow () = 0
```




<hr>



### function SetEventCallback 

```C++
virtual void AGE::AGEWindow::SetEventCallback (
    const EventCallbackFn & Callback
) = 0
```




<hr>



### function SetVSync 

```C++
virtual void AGE::AGEWindow::SetVSync (
    bool Enabled
) = 0
```




<hr>



### function SetWindowIcon 

```C++
virtual void AGE::AGEWindow::SetWindowIcon (
    const std::filesystem::path & Path
) = 0
```




<hr>



### function SwitchRenderer 

```C++
virtual void AGE::AGEWindow::SwitchRenderer () = 0
```




<hr>



### function ~AGEWindow 

```C++
inline virtual AGE::AGEWindow::~AGEWindow () 
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Scope< AGEWindow > AGE::AGEWindow::Create (
    const WindowProps & props=WindowProps ()
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Window.h`

