

# Class AGE::KeyPressedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KeyPressedEvent**](class_a_g_e_1_1_key_pressed_event.md)



_Returns the repeat count of a certain process or operation._ [More...](#detailed-description)

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
|  int | [**GetRepeatCount**](#function-getrepeatcount) () const<br>_Returns the repeat count of a certain process or operation._  |
|   | [**KeyPressedEvent**](#function-keypressedevent) (int KeyCode, int RepeatCount) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the event into a string representation._  |


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


This function returns the number of times a specific process or operation is repeated, as an integer value. If it fails to retrieve the data, it will return -1.




**Returns:**

The repeat count as an integer. 





    
## Public Functions Documentation




### function GetRepeatCount 

_Returns the repeat count of a certain process or operation._ 
```C++
inline int AGE::KeyPressedEvent::GetRepeatCount () const
```





**Returns:**

The number of times the process or operation is repeated, as an integer value. If the function fails to retrieve the data, it returns -1.


Returns the repeat count of a sequence.


This function retrieves the current value of the member variable `m_RepeatCount`, which represents the number of times a sequence should be repeated.




**Returns:**

The current repeat count as an integer. If no sequence is set or if the sequence has not been processed yet, this will return 0. 





        

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

_Converts the event into a string representation._ 
```C++
inline virtual std::string AGE::KeyPressedEvent::ToString () override const
```



This function converts the [**KeyPressedEvent**](class_a_g_e_1_1_key_pressed_event.md) object into a string format that includes the key code and repeat count of the event. The resulting string is returned by this method.




**Returns:**

A string in the format "KeyPressedEvent: [keycode] ([repeatcount] repeats)".


Converts the event into a string representation.


This function converts the [**KeyPressedEvent**](class_a_g_e_1_1_key_pressed_event.md) object into a human-readable string format. It includes details about the key code and repeat count of the event.




**Returns:**

A string containing the details of the event in a readable format. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/KeyEvent.h`

