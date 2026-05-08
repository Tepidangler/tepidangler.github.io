

# Class AGE::AxisEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AxisEvent**](class_a_g_e_1_1_axis_event.md)








Inherits the following classes: [AGE::InputEvent](class_a_g_e_1_1_input_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AxisEvent**](#function-axisevent) (int Axis, float Position) <br> |
|  int | [**GetAxis**](#function-getaxis) () <br> |
|  float | [**GetPosition**](#function-getposition) () <br> |




## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















## Protected Attributes inherited from AGE::InputEvent

See [AGE::InputEvent](class_a_g_e_1_1_input_event.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_Axis**](class_a_g_e_1_1_input_event.md#variable-m_axis)  <br> |
|  int | [**m\_Button**](class_a_g_e_1_1_input_event.md#variable-m_button)  <br> |
|  float | [**m\_Position**](class_a_g_e_1_1_input_event.md#variable-m_position)  <br> |
















































## Protected Functions inherited from AGE::InputEvent

See [AGE::InputEvent](class_a_g_e_1_1_input_event.md)

| Type | Name |
| ---: | :--- |
|   | [**InputEvent**](class_a_g_e_1_1_input_event.md#function-inputevent-13) () <br> |
|   | [**InputEvent**](class_a_g_e_1_1_input_event.md#function-inputevent-23) (int Axis, float Position) <br> |
|   | [**InputEvent**](class_a_g_e_1_1_input_event.md#function-inputevent-33) (int Button) <br> |










## Public Functions Documentation




### function AxisEvent 

```C++
inline AGE::AxisEvent::AxisEvent (
    int Axis,
    float Position
) 
```




<hr>



### function GetAxis 

```C++
inline int AGE::AxisEvent::GetAxis () 
```




<hr>



### function GetPosition 

```C++
inline float AGE::AxisEvent::GetPosition () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

