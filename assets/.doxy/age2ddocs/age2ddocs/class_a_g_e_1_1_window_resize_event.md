

# Class AGE::WindowResizeEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md)



_Represents a window resize event._ [More...](#detailed-description)

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
|  unsigned int | [**GetHeight**](#function-getheight) () const<br>_Returns the height of an object._  |
|  unsigned int | [**GetWidth**](#function-getwidth) () const<br>_Returns the width of the object._  |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_This function returns a string representation of the_ [_**WindowResizeEvent**_](class_a_g_e_1_1_window_resize_event.md) _object. The returned string includes the width and height of the window that was resized._ |
|   | [**WindowResizeEvent**](#function-windowresizeevent) (unsigned int Width, unsigned int Height) <br> |


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


This class is used to represent a window resize event, which includes the width and height of the resized window.


This class represents a window resize event. It is triggered when the size of an application's window changes. 


    
## Public Functions Documentation




### function GetHeight 

_Returns the height of an object._ 
```C++
inline unsigned int AGE::WindowResizeEvent::GetHeight () const
```



This function is used to get the current height value of an object. It returns an unsigned integer representing the height.




**Returns:**

The current height of the object as an unsigned int. If no height has been set, it will return 0.


Returns the height of an object.


This function returns the current value of the member variable 'm\_Height'. It is a getter method for this variable.




**Returns:**

The current height as an unsigned integer. 





        

<hr>



### function GetWidth 

_Returns the width of the object._ 
```C++
inline unsigned int AGE::WindowResizeEvent::GetWidth () const
```



This function returns the current value of the private member variable 'm\_Width'. It provides a way to access and retrieve the width of an object.




**Returns:**

unsigned int The current width of the object. If no width is set, it will return 0.


Returns the width of the object. 

**Returns:**

The width as an unsigned integer value. 





        

<hr>



### function ToString 

_This function returns a string representation of the_ [_**WindowResizeEvent**_](class_a_g_e_1_1_window_resize_event.md) _object. The returned string includes the width and height of the window that was resized._
```C++
inline virtual std::string AGE::WindowResizeEvent::ToString () override const
```





**Returns:**

A string containing the details about the event, such as the new width and height of the window.


Converts the [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md) object into a string format.


The function constructs and returns a string that represents the current state of the [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md) object. This includes details about the width and height of the window.




**Returns:**

A string representation of the [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md) object, including its width and height. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>



### function WindowResizeEvent 

```C++
inline AGE::WindowResizeEvent::WindowResizeEvent (
    unsigned int Width,
    unsigned int Height
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/ApplicationEvent.h`

