

# Class AGE::KeyTypedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md)



_Represents a Key Typed_ [_**Event**_](class_a_g_e_1_1_event.md) _in the system._[More...](#detailed-description)

* `#include <KeyEvent.h>`



Inherits the following classes: [AGE::KeyEvent](class_a_g_e_1_1_key_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**KeyTypedEvent**](#function-keytypedevent) (int KeyCode) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the event into a string format._  |


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










## Detailed Description


This class extends the base [**KeyEvent**](class_a_g_e_1_1_key_event.md) class and represents an event where a key has been typed into the system. It provides a method to convert this event into a string representation.


Converts the event into a string format.


This function converts the [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md) object into a string format that includes the key code of the event. The resulting string is returned by this method.




**Returns:**

A string representation of the [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md) object, including the key code. 





    
## Public Functions Documentation




### function KeyTypedEvent 

```C++
inline AGE::KeyTypedEvent::KeyTypedEvent (
    int KeyCode
) 
```




<hr>



### function ToString 

_Converts the event into a string format._ 
```C++
inline virtual std::string AGE::KeyTypedEvent::ToString () override const
```



This function converts the [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md) object into a string format that includes the key code of the event. The resulting string is returned by this method.




**Returns:**

A string representation of the [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md) object, including the key code.


Converts the event to a string representation.


This function converts the [**KeyTypedEvent**](class_a_g_e_1_1_key_typed_event.md) into a string format that includes the key code of the event. The resulting string is returned by this method.




**Returns:**

A string in the format "KeyTypedEvent: &lt;key\_code&gt;". 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/KeyEvent.h`

