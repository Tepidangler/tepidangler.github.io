

# Class AGE::StringPasteEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**StringPasteEvent**](class_a_g_e_1_1_string_paste_event.md)



_Represents a string paste event. This event is triggered when a string is pasted from the clipboard._ [More...](#detailed-description)

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
|   | [**StringPasteEvent**](#function-stringpasteevent) (const char \* String) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_This function returns a string representation of the event. The returned string includes details about what string was pasted and from where (clipboard)._  |


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


* `String` The string that was pasted.

This class represents a string paste event. It is an application event that includes details about what string was pasted and from where (clipboard). 


    
## Public Functions Documentation




### function GetString 

_This function returns a pointer to the string stored in the object._ 
```C++
inline const char * AGE::StringPasteEvent::GetString () 
```





**Returns:**

A constant character pointer pointing to the internal string of the object. If no string is set, it will return nullptr.


This function returns a pointer to the string stored in the object. 

**Returns:**

A pointer to the internal string of this object. 





        

<hr>



### function StringPasteEvent 

```C++
inline AGE::StringPasteEvent::StringPasteEvent (
    const char * String
) 
```




<hr>



### function ToString 

_This function returns a string representation of the event. The returned string includes details about what string was pasted and from where (clipboard)._ 
```C++
inline virtual std::string AGE::StringPasteEvent::ToString () override const
```





**Returns:**

std::string A string containing information about the paste event.


This function returns a string representation of the event. The returned string includes details about what string was pasted and where it came from (clipboard).




**Returns:**

A string containing information about the paste event. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/ApplicationEvent.h`

