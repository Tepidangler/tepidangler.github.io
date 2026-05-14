

# Class AGE::KeyReleasedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KeyReleasedEvent**](class_a_g_e_1_1_key_released_event.md)








Inherits the following classes: [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**KeyReleasedEvent**](#function-keyreleasedevent) (int KeyCode) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the event to a string representation._  |


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
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















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




### function KeyReleasedEvent 

```C++
inline AGE::KeyReleasedEvent::KeyReleasedEvent (
    int KeyCode
) 
```




<hr>



### function ToString 

_Converts the event to a string representation._ 
```C++
inline virtual std::string AGE::KeyReleasedEvent::ToString () override const
```



This function converts the [**KeyReleasedEvent**](class_a_g_e_1_1_key_released_event.md) into a string format that includes information about the key code of the released key. The resulting string is returned by this method.




**Returns:**

A string representing the [**KeyReleasedEvent**](class_a_g_e_1_1_key_released_event.md) in the format "KeyReleasedEvent: &lt;key\_code&gt;".


Converts the event to a string representation.


This function converts the [**KeyReleasedEvent**](class_a_g_e_1_1_key_released_event.md) into a string format that includes information about the key code of the released key. The resulting string is returned by this method.




**Returns:**

A string in the format "KeyReleasedEvent: &lt;key\_code&gt;". 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/KeyEvent.h`

