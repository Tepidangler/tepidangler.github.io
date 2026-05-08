

# Class AGE::KeyPressedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KeyPressedEvent**](class_a_g_e_1_1_key_pressed_event.md)








Inherits the following classes: [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|  int | [**GetRepeatCount**](#function-getrepeatcount) () const<br> |
|   | [**KeyPressedEvent**](#function-keypressedevent) (int KeyCode, int RepeatCount) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br> |


## Public Functions inherited from AGE::KeyEvent

See [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)

| Type | Name |
| ---: | :--- |
|  int | [**GetKeyCode**](class_a_g_e_1_1_key_event.md#function-getkeycode) () const<br> |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















## Protected Attributes inherited from AGE::KeyEvent

See [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)

| Type | Name |
| ---: | :--- |
|  int | [**m\_KeyCode**](class_a_g_e_1_1_key_event.md#variable-m_keycode)  <br> |
















































## Protected Functions inherited from AGE::KeyEvent

See [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)

| Type | Name |
| ---: | :--- |
|   | [**KeyEvent**](class_a_g_e_1_1_key_event.md#function-keyevent) (int KeyCode) <br> |










## Public Functions Documentation




### function GetRepeatCount 

```C++
inline int AGE::KeyPressedEvent::GetRepeatCount () const
```




<hr>



### function KeyPressedEvent 

```C++
inline AGE::KeyPressedEvent::KeyPressedEvent (
    int KeyCode,
    int RepeatCount
) 
```




<hr>



### function ToString 

```C++
inline virtual std::string AGE::KeyPressedEvent::ToString () override const
```



Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/KeyEvent.h`

