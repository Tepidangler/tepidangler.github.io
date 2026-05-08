

# Class AGE::ImGuiLayer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md)








Inherits the following classes: [AGE::Layer](class_a_g_e_1_1_layer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Begin**](#function-begin) () <br> |
|  void | [**BlockEvents**](#function-blockevents) (bool block) <br> |
| virtual void | [**End**](#function-end) () <br> |
|   | [**ImGuiLayer**](#function-imguilayer) () <br> |
| virtual void | [**OnAttach**](#function-onattach) () override<br> |
| virtual void | [**OnDetach**](#function-ondetach) () override<br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) override<br> |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br> |
|   | [**~ImGuiLayer**](#function-imguilayer) () <br> |


## Public Functions inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetName**](class_a_g_e_1_1_layer.md#function-getname) () const<br> |
|  float | [**GetTime**](class_a_g_e_1_1_layer.md#function-gettime) () <br> |
| virtual void | [**Init**](class_a_g_e_1_1_layer.md#function-init) () <br> |
|   | [**Layer**](class_a_g_e_1_1_layer.md#function-layer) (const std::string & name="Layer") <br> |
| virtual void | [**OnAttach**](class_a_g_e_1_1_layer.md#function-onattach) () <br> |
| virtual void | [**OnDetach**](class_a_g_e_1_1_layer.md#function-ondetach) () <br> |
| virtual void | [**OnEvent**](class_a_g_e_1_1_layer.md#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br> |
| virtual void | [**OnImGuiRender**](class_a_g_e_1_1_layer.md#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**OnUpdate**](class_a_g_e_1_1_layer.md#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual  | [**~Layer**](class_a_g_e_1_1_layer.md#function-layer) () <br> |
















## Protected Attributes inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](class_a_g_e_1_1_layer.md#variable-m_debugname)  <br> |






































## Public Functions Documentation




### function Begin 

```C++
virtual void AGE::ImGuiLayer::Begin () 
```




<hr>



### function BlockEvents 

```C++
inline void AGE::ImGuiLayer::BlockEvents (
    bool block
) 
```




<hr>



### function End 

```C++
virtual void AGE::ImGuiLayer::End () 
```




<hr>



### function ImGuiLayer 

```C++
AGE::ImGuiLayer::ImGuiLayer () 
```




<hr>



### function OnAttach 

```C++
virtual void AGE::ImGuiLayer::OnAttach () override
```



Implements [*AGE::Layer::OnAttach*](class_a_g_e_1_1_layer.md#function-onattach)


<hr>



### function OnDetach 

```C++
virtual void AGE::ImGuiLayer::OnDetach () override
```



Implements [*AGE::Layer::OnDetach*](class_a_g_e_1_1_layer.md#function-ondetach)


<hr>



### function OnEvent 

```C++
virtual void AGE::ImGuiLayer::OnEvent (
    Event & E
) override
```



Implements [*AGE::Layer::OnEvent*](class_a_g_e_1_1_layer.md#function-onevent)


<hr>



### function OnImGuiRender 

```C++
virtual void AGE::ImGuiLayer::OnImGuiRender (
    TimeStep DeltaTime
) override
```



Implements [*AGE::Layer::OnImGuiRender*](class_a_g_e_1_1_layer.md#function-onimguirender)


<hr>



### function ~ImGuiLayer 

```C++
AGE::ImGuiLayer::~ImGuiLayer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/ImGui/Public/ImGuiLayer.h`

