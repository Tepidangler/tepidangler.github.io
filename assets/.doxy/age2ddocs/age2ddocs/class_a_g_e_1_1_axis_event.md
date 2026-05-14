

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
|   | [**AxisEvent**](#function-axisevent) (int Axis, float Position) <br>_Constructs an instance of the_ [_**AxisEvent**_](class_a_g_e_1_1_axis_event.md) _class with specified axis and position._ |
|  int | [**GetAxis**](#function-getaxis) () <br>_This function returns the value of the member variable 'm\_Axis'._  |
|  float | [**GetPosition**](#function-getposition) () <br>_This function returns the current position value._  |




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




### function AxisEvent 

_Constructs an instance of the_ [_**AxisEvent**_](class_a_g_e_1_1_axis_event.md) _class with specified axis and position._
```C++
inline AGE::AxisEvent::AxisEvent (
    int Axis,
    float Position
) 
```



This constructor creates a new instance of the [**AxisEvent**](class_a_g_e_1_1_axis_event.md) class by initializing its base class ([**InputEvent**](class_a_g_e_1_1_input_event.md)) with the provided axis and position values.




**Parameters:**


* `Axis` The identifier for the input event's associated physical axis. 
* `Position` The current position of the physical axis in relation to its origin point.

Constructs an instance of the [**AxisEvent**](class_a_g_e_1_1_axis_event.md) class with specified axis and position.


This constructor creates a new instance of the [**AxisEvent**](class_a_g_e_1_1_axis_event.md) class by initializing its base class ([**InputEvent**](class_a_g_e_1_1_input_event.md)) with the provided axis and position values.




**Parameters:**


* `Axis` The identifier for the input event's associated physical axis, such as an x-axis or y-axis. 
* `Position` The current position on the specified axis. This could be a value between -1.0 and 1.0, representing full left to right movement.



**Returns:**

An instance of [**AxisEvent**](class_a_g_e_1_1_axis_event.md) with the provided axis and position values. 





        

<hr>



### function GetAxis 

_This function returns the value of the member variable 'm\_Axis'._ 
```C++
inline int AGE::AxisEvent::GetAxis () 
```





**Returns:**

The integer value stored in 'm\_Axis'


This function returns the current axis value.




**Returns:**

The integer value of the current axis. 





        

<hr>



### function GetPosition 

_This function returns the current position value._ 
```C++
inline float AGE::AxisEvent::GetPosition () 
```





**Returns:**

A floating-point number representing the current position.


Returns the current position value.


This function retrieves and returns the current position value stored in the member variable 'm\_Position'. The returned value represents a float representing the position of an object or entity.




**Returns:**

A floating-point number representing the current position. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

