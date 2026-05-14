

# Class AGE::MouseScrolledEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseScrolledEvent**](class_a_g_e_1_1_mouse_scrolled_event.md)








Inherits the following classes: [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetXOffset**](#function-getxoffset) () const<br>_Returns the X offset value._  |
|  float | [**GetYOffset**](#function-getyoffset) () const<br>_This function returns the Y offset value._  |
|   | [**MouseScrolledEvent**](#function-mousescrolledevent) (float xOffset, float yOffset) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_This function returns a string representation of the_ [_**MouseScrolledEvent**_](class_a_g_e_1_1_mouse_scrolled_event.md) _object. The returned string includes the x and y offsets that represent the scroll event._ |


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




### function GetXOffset 

_Returns the X offset value._ 
```C++
inline float AGE::MouseScrolledEvent::GetXOffset () const
```



This function returns the current X offset value stored in the object. The X offset is used to adjust the position of objects on the x-axis.




**Returns:**

A float representing the current X offset value.


This function returns the X offset value. 

**Returns:**

A floating-point number representing the X offset. 





        

<hr>



### function GetYOffset 

_This function returns the Y offset value._ 
```C++
inline float AGE::MouseScrolledEvent::GetYOffset () const
```





**Returns:**

A floating-point number representing the Y offset.


This function returns the Y offset value. 

**Returns:**

A constant float representing the current Y offset value. 





        

<hr>



### function MouseScrolledEvent 

```C++
inline AGE::MouseScrolledEvent::MouseScrolledEvent (
    float xOffset,
    float yOffset
) 
```




<hr>



### function ToString 

_This function returns a string representation of the_ [_**MouseScrolledEvent**_](class_a_g_e_1_1_mouse_scrolled_event.md) _object. The returned string includes the x and y offsets that represent the scroll event._
```C++
inline virtual std::string AGE::MouseScrolledEvent::ToString () override const
```





**Returns:**

A string containing the details about the mouse scrolling event.


Converts the [**MouseScrolledEvent**](class_a_g_e_1_1_mouse_scrolled_event.md) into a string format.


The function constructs and returns a string representation of the [**MouseScrolledEvent**](class_a_g_e_1_1_mouse_scrolled_event.md) object, which includes the x-offset and y-offset values.




**Returns:**

A string containing the details about the [**MouseScrolledEvent**](class_a_g_e_1_1_mouse_scrolled_event.md). 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

