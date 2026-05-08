

# Class AGE::InputEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**InputEvent**](class_a_g_e_1_1_input_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)


Inherited by the following classes: [AGE::AxisEvent](class_a_g_e_1_1_axis_event.md),  [AGE::GamepadButtonPressedEvent](class_a_g_e_1_1_gamepad_button_pressed_event.md),  [AGE::GamepadButtonReleasedEvent](class_a_g_e_1_1_gamepad_button_released_event.md)






















## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |
































## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_Axis**](#variable-m_axis)  <br> |
|  int | [**m\_Button**](#variable-m_button)  <br> |
|  float | [**m\_Position**](#variable-m_position)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**InputEvent**](#function-inputevent-13) () <br> |
|   | [**InputEvent**](#function-inputevent-23) (int Axis, float Position) <br> |
|   | [**InputEvent**](#function-inputevent-33) (int Button) <br> |








## Protected Attributes Documentation




### variable m\_Axis 

```C++
int AGE::InputEvent::m_Axis;
```




<hr>



### variable m\_Button 

```C++
int AGE::InputEvent::m_Button;
```




<hr>



### variable m\_Position 

```C++
float AGE::InputEvent::m_Position;
```




<hr>
## Protected Functions Documentation




### function InputEvent [1/3]

```C++
AGE::InputEvent::InputEvent () 
```




<hr>



### function InputEvent [2/3]

```C++
inline AGE::InputEvent::InputEvent (
    int Axis,
    float Position
) 
```




<hr>



### function InputEvent [3/3]

```C++
inline AGE::InputEvent::InputEvent (
    int Button
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

