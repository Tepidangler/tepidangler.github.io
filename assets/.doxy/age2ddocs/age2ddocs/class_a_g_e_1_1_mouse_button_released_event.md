

# Class AGE::MouseButtonReleasedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseButtonReleasedEvent**](class_a_g_e_1_1_mouse_button_released_event.md)



_Represents a mouse button released event._ [More...](#detailed-description)

* `#include <MouseEvent.h>`



Inherits the following classes: [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MouseButtonReleasedEvent**](#function-mousebuttonreleasedevent) (int Button) <br> |
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










## Detailed Description


This class inherits from the [**MouseEvent**](class_a_g_e_1_1_mouse_event.md) base class and is used to represent a specific type of event, which is a mouse button being released. The constructor takes an integer parameter representing the button that was released. The [**ToString()**](class_a_g_e_1_1_mouse_button_released_event.md#function-tostring) method overrides the base class's pure virtual method and returns a string representation of this event.


Represents a mouse button release event.


This class represents a specific type of mouse event where a button is released. It includes details about the button that was released. 


    
## Public Functions Documentation




### function MouseButtonReleasedEvent 

```C++
inline AGE::MouseButtonReleasedEvent::MouseButtonReleasedEvent (
    int Button
) 
```




<hr>



### function ToString 

_Converts the event to a string representation._ 
```C++
inline virtual std::string AGE::MouseButtonReleasedEvent::ToString () override const
```



This function converts the [**MouseButtonReleasedEvent**](class_a_g_e_1_1_mouse_button_released_event.md) into a human-readable string format. It includes details about the button that was released.




**Returns:**

A string containing the event type and the button that was released.


Converts the event to a string representation.


This function converts the [**MouseButtonReleasedEvent**](class_a_g_e_1_1_mouse_button_released_event.md) into a human-readable format by appending the button that was released. The resulting string is returned as output of this method.




**Returns:**

A string containing the details about the mouse button release event. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

