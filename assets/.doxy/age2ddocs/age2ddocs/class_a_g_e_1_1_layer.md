

# Class AGE::Layer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Layer**](class_a_g_e_1_1_layer.md)










Inherited by the following classes: [AGE::ImGuiLayer](class_a_g_e_1_1_im_gui_layer.md),  [AGE::NodeEditorWindow](class_a_g_e_1_1_node_editor_window.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetName**](#function-getname) () const<br> |
|  float | [**GetTime**](#function-gettime) () <br> |
| virtual void | [**Init**](#function-init) () <br> |
|   | [**Layer**](#function-layer) (const std::string & name="Layer") <br> |
| virtual void | [**OnAttach**](#function-onattach) () <br> |
| virtual void | [**OnDetach**](#function-ondetach) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br> |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual  | [**~Layer**](#function-layer) () <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](#variable-m_debugname)  <br> |




















## Public Functions Documentation




### function GetName 

```C++
inline const std::string & AGE::Layer::GetName () const
```




<hr>



### function GetTime 

```C++
float AGE::Layer::GetTime () 
```




<hr>



### function Init 

```C++
inline virtual void AGE::Layer::Init () 
```




<hr>



### function Layer 

```C++
AGE::Layer::Layer (
    const std::string & name="Layer"
) 
```




<hr>



### function OnAttach 

```C++
inline virtual void AGE::Layer::OnAttach () 
```




<hr>



### function OnDetach 

```C++
inline virtual void AGE::Layer::OnDetach () 
```




<hr>



### function OnEvent 

```C++
inline virtual void AGE::Layer::OnEvent (
    Event & Event
) 
```




<hr>



### function OnImGuiRender 

```C++
inline virtual void AGE::Layer::OnImGuiRender (
    TimeStep DeltaTime
) 
```




<hr>



### function OnUpdate 

```C++
inline virtual void AGE::Layer::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function ~Layer 

```C++
virtual AGE::Layer::~Layer () 
```




<hr>
## Protected Attributes Documentation




### variable m\_DebugName 

```C++
std::string AGE::Layer::m_DebugName;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Layer.h`

