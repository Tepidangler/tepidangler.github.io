

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
|  float | [**GetXOffset**](#function-getxoffset) () const<br> |
|  float | [**GetYOffset**](#function-getyoffset) () const<br> |
|   | [**MouseScrolledEvent**](#function-mousescrolledevent) (float xOffset, float yOffset) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br> |


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
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















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
|   | [**MouseEvent**](class_a_g_e_1_1_mouse_event.md#function-mouseevent-23) (float x, float y) <br> |
|   | [**MouseEvent**](class_a_g_e_1_1_mouse_event.md#function-mouseevent-33) (float xOffset, float yOffset, bool Scrolled) <br> |










## Public Functions Documentation




### function GetXOffset 

```C++
inline float AGE::MouseScrolledEvent::GetXOffset () const
```




<hr>



### function GetYOffset 

```C++
inline float AGE::MouseScrolledEvent::GetYOffset () const
```




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

```C++
inline virtual std::string AGE::MouseScrolledEvent::ToString () override const
```



Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

