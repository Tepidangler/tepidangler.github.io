

# Class AGE::MouseEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MouseEvent**](class_a_g_e_1_1_mouse_event.md)








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
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |














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
|   | [**MouseEvent**](#function-mouseevent-23) (float x, float y) <br> |
|   | [**MouseEvent**](#function-mouseevent-33) (float xOffset, float yOffset, bool Scrolled) <br> |








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

```C++
inline AGE::MouseEvent::MouseEvent (
    float x,
    float y
) 
```




<hr>



### function MouseEvent [3/3]

```C++
inline AGE::MouseEvent::MouseEvent (
    float xOffset,
    float yOffset,
    bool Scrolled
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/MouseEvent.h`

