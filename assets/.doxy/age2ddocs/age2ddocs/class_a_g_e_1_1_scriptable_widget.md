

# Class AGE::ScriptableWidget



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md)








Inherits the following classes: std::enable_shared_from_this< ScriptableWidget >


































## Public Functions

| Type | Name |
| ---: | :--- |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br> |
|  T & | [**GetComponent**](#function-getcomponent) () <br> |
| virtual [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetID**](#function-getid) () <br> |
| virtual std::string | [**GetName**](#function-getname) () <br> |
| virtual bool | [**IsVisible**](#function-isvisible) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
| virtual void | [**SetVisibility**](#function-setvisibility) (bool Visibility) <br> |
| virtual  | [**~ScriptableWidget**](#function-scriptablewidget) () <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**bIsVisible**](#variable-bisvisible)   = `true`<br> |
|  std::string | [**m\_Name**](#variable-m_name)   = `""`<br> |
|  [**ScreenResolution**](struct_a_g_e_1_1_screen_resolution.md) | [**m\_Resolution**](#variable-m_resolution)  <br> |
|  EWidgetStack | [**m\_Stack**](#variable-m_stack)   = `EWidgetStack::INVALID`<br> |
|  std::vector&lt; Ref&lt; [**UIComponent**](class_a_g_e_1_1_u_i_component.md) &gt; &gt; | [**m\_UIComponents**](#variable-m_uicomponents)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual [**Entity**](class_a_g_e_1_1_entity.md) & | [**GetEntityHandle**](#function-getentityhandle) () <br> |
| virtual void | [**OnConstruct**](#function-onconstruct) () <br> |
| virtual void | [**OnDestroy**](#function-ondestroy) () <br> |
| virtual void | [**OnInit**](#function-oninit) () <br> |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**Reset**](#function-reset) () <br> |




## Public Functions Documentation




### function AddComponent 

```C++
template<typename T, typename ... Args>
inline T & AGE::ScriptableWidget::AddComponent (
    Args &&... args
) 
```




<hr>



### function GetComponent 

```C++
template<typename T>
inline T & AGE::ScriptableWidget::GetComponent () 
```




<hr>



### function GetID 

```C++
inline virtual UUID AGE::ScriptableWidget::GetID () 
```




<hr>



### function GetName 

```C++
inline virtual std::string AGE::ScriptableWidget::GetName () 
```




<hr>



### function IsVisible 

```C++
inline virtual bool AGE::ScriptableWidget::IsVisible () 
```




<hr>



### function OnEvent 

```C++
inline virtual void AGE::ScriptableWidget::OnEvent (
    Event & E
) 
```




<hr>



### function SetVisibility 

```C++
inline virtual void AGE::ScriptableWidget::SetVisibility (
    bool Visibility
) 
```




<hr>



### function ~ScriptableWidget 

```C++
inline virtual AGE::ScriptableWidget::~ScriptableWidget () 
```




<hr>
## Protected Attributes Documentation




### variable bIsVisible 

```C++
bool AGE::ScriptableWidget::bIsVisible;
```




<hr>



### variable m\_Name 

```C++
std::string AGE::ScriptableWidget::m_Name;
```




<hr>



### variable m\_Resolution 

```C++
ScreenResolution AGE::ScriptableWidget::m_Resolution;
```




<hr>



### variable m\_Stack 

```C++
EWidgetStack AGE::ScriptableWidget::m_Stack;
```




<hr>



### variable m\_UIComponents 

```C++
std::vector<Ref<UIComponent> > AGE::ScriptableWidget::m_UIComponents;
```




<hr>
## Protected Functions Documentation




### function GetEntityHandle 

```C++
inline virtual Entity & AGE::ScriptableWidget::GetEntityHandle () 
```




<hr>



### function OnConstruct 

```C++
inline virtual void AGE::ScriptableWidget::OnConstruct () 
```




<hr>



### function OnDestroy 

```C++
inline virtual void AGE::ScriptableWidget::OnDestroy () 
```




<hr>



### function OnInit 

```C++
inline virtual void AGE::ScriptableWidget::OnInit () 
```




<hr>



### function OnUpdate 

```C++
inline virtual void AGE::ScriptableWidget::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function Reset 

```C++
inline virtual void AGE::ScriptableWidget::Reset () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/ScriptableWidget.h`

