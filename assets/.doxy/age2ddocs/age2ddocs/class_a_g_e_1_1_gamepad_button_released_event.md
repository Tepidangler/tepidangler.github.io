

# Class AGE::GamepadButtonReleasedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GamepadButtonReleasedEvent**](class_a_g_e_1_1_gamepad_button_released_event.md)








Inherits the following classes: [AGE::InputEvent](class_a_g_e_1_1_input_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GamepadButtonReleasedEvent**](#function-gamepadbuttonreleasedevent) (int Button) <br>_Constructor for the_ [_**GamepadButtonReleasedEvent**_](class_a_g_e_1_1_gamepad_button_released_event.md) _class._ |
|  int | [**GetButton**](#function-getbutton) () <br>_Returns the current state of the button._  |




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




### function GamepadButtonReleasedEvent 

_Constructor for the_ [_**GamepadButtonReleasedEvent**_](class_a_g_e_1_1_gamepad_button_released_event.md) _class._
```C++
inline AGE::GamepadButtonReleasedEvent::GamepadButtonReleasedEvent (
    int Button
) 
```



This constructor is used to create a new instance of the [**GamepadButtonReleasedEvent**](class_a_g_e_1_1_gamepad_button_released_event.md) class, which represents an event signifying that a gamepad button has been released. The specific button associated with this event is passed as an argument during instantiation.




**Parameters:**


* `Button` An integer representing the ID of the gamepad button that was released.

Constructs a [**GamepadButtonReleasedEvent**](class_a_g_e_1_1_gamepad_button_released_event.md) object with the specified button number.


This constructor creates an instance of [**GamepadButtonReleasedEvent**](class_a_g_e_1_1_gamepad_button_released_event.md) that represents a gamepad button release event. The button number is passed as an argument to this function, which will be used by the [**InputEvent**](class_a_g_e_1_1_input_event.md) base class for processing the event.




**Parameters:**


* `Button` An integer representing the button number that was released. 




        

<hr>



### function GetButton 

_Returns the current state of the button._ 
```C++
inline int AGE::GamepadButtonReleasedEvent::GetButton () 
```



This function returns the current state of the button which can be either pressed or not pressed. The returned value is an integer where 0 represents the button being not pressed and any other number represents it being pressed.




**Returns:**

int - Current state of the button (0 for not pressed, non-zero for pressed).


Returns the current state of the button. 

**Returns:**

The current state of the button as an integer. If the button is pressed, it returns 1; if not, it returns 0. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

