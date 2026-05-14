

# Class AGE::GamepadButtonPressedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GamepadButtonPressedEvent**](class_a_g_e_1_1_gamepad_button_pressed_event.md)








Inherits the following classes: [AGE::InputEvent](class_a_g_e_1_1_input_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GamepadButtonPressedEvent**](#function-gamepadbuttonpressedevent) (int Button) <br>_Constructor for the_ [_**GamepadButtonPressedEvent**_](class_a_g_e_1_1_gamepad_button_pressed_event.md) _class._ |
|  int | [**GetButton**](#function-getbutton) () <br>_Returns the value of member variable 'm\_Button'._  |




## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















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
|   | [**InputEvent**](class_a_g_e_1_1_input_event.md#function-inputevent-23) (int Axis, float Position) <br>_Constructs an_ [_**InputEvent**_](class_a_g_e_1_1_input_event.md) _object with the specified axis and position._ |
|   | [**InputEvent**](class_a_g_e_1_1_input_event.md#function-inputevent-33) (int Button) <br>_Constructor for the_ [_**InputEvent**_](class_a_g_e_1_1_input_event.md) _class._ |










## Public Functions Documentation




### function GamepadButtonPressedEvent 

_Constructor for the_ [_**GamepadButtonPressedEvent**_](class_a_g_e_1_1_gamepad_button_pressed_event.md) _class._
```C++
inline AGE::GamepadButtonPressedEvent::GamepadButtonPressedEvent (
    int Button
) 
```



This constructor creates a new instance of the [**GamepadButtonPressedEvent**](class_a_g_e_1_1_gamepad_button_pressed_event.md) class with the specified button number. It inherits from the [**InputEvent**](class_a_g_e_1_1_input_event.md) base class.




**Parameters:**


* `Button` The button number that was pressed on the gamepad.

Constructs a [**GamepadButtonPressedEvent**](class_a_g_e_1_1_gamepad_button_pressed_event.md) object with the specified button number.


This constructor creates an instance of [**GamepadButtonPressedEvent**](class_a_g_e_1_1_gamepad_button_pressed_event.md) that represents a button press event on a gamepad device. The button parameter specifies which button was pressed.




**Parameters:**


* `Button` An integer representing the button number that was pressed. 




        

<hr>



### function GetButton 

_Returns the value of member variable 'm\_Button'._ 
```C++
inline int AGE::GamepadButtonPressedEvent::GetButton () 
```





**Returns:**

The current state of button represented by integer.


Returns the current state of the button. 

**Returns:**

The current state of the button as an integer. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

