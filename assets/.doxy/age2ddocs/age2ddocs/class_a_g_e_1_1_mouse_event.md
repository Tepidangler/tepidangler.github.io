

# Class AGE::MouseEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseEvent**](class_a_g_e_1_1_mouse_event.md)



_Represents a mouse event._ [More...](#detailed-description)

* `#include <MouseEvent.h>`



Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)


Inherited by the following classes: [AGE::MouseButtonPressedEvent](class_a_g_e_1_1_mouse_button_pressed_event.md),  [AGE::MouseButtonReleasedEvent](class_a_g_e_1_1_mouse_button_released_event.md),  [AGE::MouseMovedEvent](class_a_g_e_1_1_mouse_moved_event.md),  [AGE::MouseScrolledEvent](class_a_g_e_1_1_mouse_scrolled_event.md)






















## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  int | [**GetMouseButton**](#function-getmousebutton) () const<br> |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  int | [**m\_Button**](#variable-m_button)  <br> |
|  float | [**m\_MouseX**](#variable-m_mousex)  <br> |
|  float | [**m\_MouseY**](#variable-m_mousey)  <br> |
|  float | [**m\_XOffset**](#variable-m_xoffset)  <br> |
|  float | [**m\_YOffset**](#variable-m_yoffset)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**MouseEvent**](#function-mouseevent-13) (int Button) <br> |
|   | [**MouseEvent**](#function-mouseevent-23) (float x, float y) <br>_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with the given coordinates._ |
|   | [**MouseEvent**](#function-mouseevent-33) (float xOffset, float yOffset, bool Scrolled) <br>_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with given offsets._ |








## Detailed Description


This class is used to represent different types of mouse events, such as button presses or scrolls. It provides methods for getting the type and position of the mouse event. 


    
## Public Functions Documentation




### function GetMouseButton 

```C++
inline int AGE::MouseEvent::GetMouseButton () const
```




<hr>
## Protected Attributes Documentation




### variable m\_Button 

```C++
int AGE::MouseEvent::m_Button;
```




<hr>



### variable m\_MouseX 

```C++
float AGE::MouseEvent::m_MouseX;
```




<hr>



### variable m\_MouseY 

```C++
float AGE::MouseEvent::m_MouseY;
```




<hr>



### variable m\_XOffset 

```C++
float AGE::MouseEvent::m_XOffset;
```




<hr>



### variable m\_YOffset 

```C++
float AGE::MouseEvent::m_YOffset;
```




<hr>
## Protected Functions Documentation




### function MouseEvent [1/3]

```C++
inline AGE::MouseEvent::MouseEvent (
    int Button
) 
```




<hr>



### function MouseEvent [2/3]

_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with the given coordinates._
```C++
inline AGE::MouseEvent::MouseEvent (
    float x,
    float y
) 
```





**Parameters:**


* `x` The x-coordinate of the mouse event. 
* `y` The y-coordinate of the mouse event.

Constructs a [**MouseEvent**](class_a_g_e_1_1_mouse_event.md) object with the given coordinates.




**Parameters:**


* `x` The x-coordinate of the mouse event. 
* `y` The y-coordinate of the mouse event. 




        

<hr>



### function MouseEvent [3/3]

_Constructs a_ [_**MouseEvent**_](class_a_g_e_1_1_mouse_event.md) _object with given offsets._
```C++
inline AGE::MouseEvent::MouseEvent (
    float xOffset,
    float yOffset,
    bool Scrolled
) 
```



This function is used to create a new [**MouseEvent**](class_a_g_e_1_1_mouse_event.md) instance with the specified x and y offsets. The boolean Scrolled parameter is not actually utilized in this function, so it can be safely ignored for now.




**Parameters:**


* `xOffset` The horizontal scroll offset. 
* `yOffset` The vertical scroll offset. 
* `Scrolled` A boolean indicating whether the mouse scrolled or not (not used).

Constructs a [**MouseEvent**](class_a_g_e_1_1_mouse_event.md) object with given x and y offset values.


This constructor is used to create a new [**MouseEvent**](class_a_g_e_1_1_mouse_event.md) instance with the specified x and y offset values, which are then stored in member variables m\_XOffset and m\_YOffset respectively. The boolean Scrolled parameter is not utilized as it's not clear what its purpose would be without additional context or information about how this class is intended to be used.




**Parameters:**


* `xOffset` The horizontal offset value for the mouse event. 
* `yOffset` The vertical offset value for the mouse event. 
* `Scrolled` A boolean indicating whether the scroll wheel was moved (not currently utilized). 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

