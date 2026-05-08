

# Class AGE::RenderUIEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RenderUIEvent**](class_a_g_e_1_1_render_u_i_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**TimeStep**](class_a_g_e_1_1_time_step.md) | [**m\_DeltaTime**](#variable-m_deltatime)  <br> |


## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  [**TimeStep**](class_a_g_e_1_1_time_step.md) | [**GetDeltaTime**](#function-getdeltatime) () const<br> |
|   | [**RenderUIEvent**](#function-renderuievent) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















































## Public Attributes Documentation




### variable m\_DeltaTime 

```C++
TimeStep AGE::RenderUIEvent::m_DeltaTime;
```




<hr>
## Public Functions Documentation




### function GetDeltaTime 

```C++
inline TimeStep AGE::RenderUIEvent::GetDeltaTime () const
```




<hr>



### function RenderUIEvent 

```C++
inline AGE::RenderUIEvent::RenderUIEvent (
    TimeStep DeltaTime
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/RendererEvent.h`

