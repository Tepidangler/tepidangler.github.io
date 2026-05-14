

# Class AGE::KeyEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KeyEvent**](class_a_g_e_1_1_key_event.md)



_Represents a keyboard event._ [More...](#detailed-description)

* `#include <KeyEvent.h>`



Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)


Inherited by the following classes: [AGE::KeyPressedEvent](class_a_g_e_1_1_key_pressed_event.md),  [AGE::KeyReleasedEvent](class_a_g_e_1_1_key_released_event.md),  [AGE::KeyTypedEvent](class_a_g_e_1_1_key_typed_event.md)






















## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  int | [**GetKeyCode**](#function-getkeycode) () const<br> |


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
|  int | [**m\_KeyCode**](#variable-m_keycode)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**KeyEvent**](#function-keyevent) (int KeyCode) <br> |








## Detailed Description


This class is used to represent a keyboard event, which includes the key code associated with the event.


Represents a keyboard event.


This class is used to represent a keyboard event, which includes the key code of the pressed key. 


    
## Public Functions Documentation




### function GetKeyCode 

```C++
inline int AGE::KeyEvent::GetKeyCode () const
```




<hr>
## Protected Attributes Documentation




### variable m\_KeyCode 

```C++
int AGE::KeyEvent::m_KeyCode;
```




<hr>
## Protected Functions Documentation




### function KeyEvent 

```C++
inline AGE::KeyEvent::KeyEvent (
    int KeyCode
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/KeyEvent.h`

