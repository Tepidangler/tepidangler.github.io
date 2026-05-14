

# Class AGE::MouseMovedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseMovedEvent**](class_a_g_e_1_1_mouse_moved_event.md)








Inherits the following classes: [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetX**](#function-getx) () const<br>_Returns the current x-coordinate of the mouse cursor._  |
|  float | [**GetY**](#function-gety) () const<br>_This function returns the current value of member variable 'm\_MouseY'._  |
|   | [**MouseMovedEvent**](#function-mousemovedevent) (float x, float y) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the event data into a string format._  |


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




### function GetX 

_Returns the current x-coordinate of the mouse cursor._ 
```C++
inline float AGE::MouseMovedEvent::GetX () const
```





**Returns:**

A floating point number representing the current x-coordinate of the mouse cursor.


Returns the current x-coordinate of the mouse cursor. 

**Returns:**

The x-coordinate value as a floating point number. If there is an error in retrieving the data, it returns -1.0. 





        

<hr>



### function GetY 

_This function returns the current value of member variable 'm\_MouseY'._ 
```C++
inline float AGE::MouseMovedEvent::GetY () const
```





**Returns:**

A floating-point number representing the y-coordinate.


This function returns the value of member variable 'm\_MouseY'. 

**Returns:**

A floating-point number representing the current y-coordinate. 





        

<hr>



### function MouseMovedEvent 

```C++
inline AGE::MouseMovedEvent::MouseMovedEvent (
    float x,
    float y
) 
```




<hr>



### function ToString 

_Converts the event data into a string format._ 
```C++
inline virtual std::string AGE::MouseMovedEvent::ToString () override const
```



This function converts the mouse movement event data into a human-readable string format. The string includes the x and y coordinates of the mouse cursor at the time of the event.




**Returns:**

A string containing the details of the mouse movement event.


This function returns a string representation of the [**MouseMovedEvent**](class_a_g_e_1_1_mouse_moved_event.md) object. The returned string includes the x and y coordinates of the mouse cursor at the time of the event.




**Returns:**

A string in the format "MouseMovedEvent: &lt;m\_MouseX&gt;, &lt;m\_MouseY&gt;". 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

