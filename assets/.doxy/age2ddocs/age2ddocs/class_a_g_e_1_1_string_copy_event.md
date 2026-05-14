

# Class AGE::StringCopyEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**StringCopyEvent**](class_a_g_e_1_1_string_copy_event.md)



_Represents a string copy event. This event is triggered when a string is copied to the clipboard._ [More...](#detailed-description)

* `#include <ApplicationEvent.h>`



Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)
























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  const char \* | [**GetString**](#function-getstring) () <br>_This function returns a pointer to the string stored in the object._  |
|   | [**StringCopyEvent**](#function-stringcopyevent) (const char \* String) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_This function returns a string representation of the event. The returned string includes details about what string was copied to the clipboard, and is formatted as such._  |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















































## Detailed Description




**Parameters:**


* `String` The string that was copied.

This class represents an event that occurs when a string is copied.


It contains the string that was copied and provides methods to access this string and get a string representation of the event. 


    
## Public Functions Documentation




### function GetString 

_This function returns a pointer to the string stored in the object._ 
```C++
inline const char * AGE::StringCopyEvent::GetString () 
```





**Returns:**

A constant character pointer to the internal string of this object.


This function returns a pointer to the string stored in member variable `m_String`. 

**Returns:**

A constant pointer to the string stored in `m_String`. If no such string exists, it will return nullptr. 





        

<hr>



### function StringCopyEvent 

```C++
inline AGE::StringCopyEvent::StringCopyEvent (
    const char * String
) 
```




<hr>



### function ToString 

_This function returns a string representation of the event. The returned string includes details about what string was copied to the clipboard, and is formatted as such._ 
```C++
inline virtual std::string AGE::StringCopyEvent::ToString () override const
```





**Returns:**

A string containing information about the copy event.


Converts the event into a string format.


This function converts the event into a human-readable string format, which includes details about what string was copied to the clipboard and when it happened.




**Returns:**

A string containing information about the copy event. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/ApplicationEvent.h`

