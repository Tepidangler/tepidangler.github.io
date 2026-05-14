

# Class AGE::MouseButtonPressedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseButtonPressedEvent**](class_a_g_e_1_1_mouse_button_pressed_event.md)








Inherits the following classes: [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MouseButtonPressedEvent**](#function-mousebuttonpressedevent) (int Button) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the event to a string representation._  |


## Public Functions inherited from AGE::MouseEvent

See [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)

| Type | Name |
| ---: | :--- |
|  int | [**GetMouseButton**](class_a_g_e_1_1_mouse_event.md#function-getmousebutton) () const<br> |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















## Protected Attributes inherited from AGE::MouseEvent

See [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_Button**](class_a_g_e_1_1_mouse_event.md#variable-m_button)  <br> |
|  float | [**m\_MouseX**](class_a_g_e_1_1_mouse_event.md#variable-m_mousex)  <br> |
|  float | [**m\_MouseY**](class_a_g_e_1_1_mouse_event.md#variable-m_mousey)  <br> |
|  float | [**m\_XOffset**](class_a_g_e_1_1_mouse_event.md#variable-m_xoffset)  <br> |
|  float | [**m\_YOffset**](class_a_g_e_1_1_mouse_event.md#variable-m_yoffset)  <br> |
















































## Protected Functions inherited from AGE::MouseEvent

See [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)

| Type | Name |
| ---: | :--- |
|   | [**MouseEvent**](class_a_g_e_1_1_mouse_event.md#function-mouseevent-13) (int Button) <br> |
|   | [**MouseEvent**](class_a_g_e_1_1_mouse_event.md#function-mouseevent-23) (float x, float y) <br>_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with the given coordinates._ |
|   | [**MouseEvent**](class_a_g_e_1_1_mouse_event.md#function-mouseevent-33) (float xOffset, float yOffset, bool Scrolled) <br>_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with given offsets._ |










## Public Functions Documentation




### function MouseButtonPressedEvent 

```C++
inline AGE::MouseButtonPressedEvent::MouseButtonPressedEvent (
    int Button
) 
```




<hr>



### function ToString 

_Converts the event to a string representation._ 
```C++
inline virtual std::string AGE::MouseButtonPressedEvent::ToString () override const
```



This function converts the event into a human-readable format by appending the button value of the event to a base string. The resulting string is returned as output.




**Returns:**

A string representing the event in the format "MouseButtonPressedEvent: &lt;button&gt;".


Converts the event to a string representation.


This function converts the [**MouseButtonPressedEvent**](class_a_g_e_1_1_mouse_button_pressed_event.md) into a human-readable string format. It includes information about the button that was pressed in the event.




**Returns:**

A string containing the details of the event, such as "MouseButtonPressedEvent: ButtonName". 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

