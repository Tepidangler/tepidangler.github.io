

# Class AGE::FramebufferResizeEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FramebufferResizeEvent**](class_a_g_e_1_1_framebuffer_resize_event.md)



_Represents a framebuffer resize event._ [More...](#detailed-description)

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
|   | [**FramebufferResizeEvent**](#function-framebufferresizeevent) (unsigned int Width, unsigned int Height) <br> |
|  unsigned int | [**GetHeight**](#function-getheight) () const<br>_Returns the height of an object._  |
|  unsigned int | [**GetWidth**](#function-getwidth) () const<br>_Returns the width of the object._  |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the_ [_**FramebufferResizeEvent**_](class_a_g_e_1_1_framebuffer_resize_event.md) _into a string format._ |


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


This class is used to represent a framebuffer resize event, which occurs when the size of the framebuffer changes. It contains two parameters - width and height that specify the new dimensions of the framebuffer. 


    
## Public Functions Documentation




### function FramebufferResizeEvent 

```C++
inline AGE::FramebufferResizeEvent::FramebufferResizeEvent (
    unsigned int Width,
    unsigned int Height
) 
```




<hr>



### function GetHeight 

_Returns the height of an object._ 
```C++
inline unsigned int AGE::FramebufferResizeEvent::GetHeight () const
```



This function is used to get the current height value of an object. It returns an unsigned integer representing the height.




**Returns:**

The current height of the object as an unsigned int.


Returns the height of an object.


This function returns the current value of the member variable 'm\_Height'. It is a getter method for this variable.




**Returns:**

The current height as an unsigned integer. 





        

<hr>



### function GetWidth 

_Returns the width of the object._ 
```C++
inline unsigned int AGE::FramebufferResizeEvent::GetWidth () const
```





**Returns:**

The width as an unsigned integer.


Returns the width of the object. 

**Returns:**

The width as an unsigned integer. 





        

<hr>



### function ToString 

_Converts the_ [_**FramebufferResizeEvent**_](class_a_g_e_1_1_framebuffer_resize_event.md) _into a string format._
```C++
inline virtual std::string AGE::FramebufferResizeEvent::ToString () override const
```



This function converts the [**FramebufferResizeEvent**](class_a_g_e_1_1_framebuffer_resize_event.md) object into a string representation, which includes the width and height of the framebuffer that was resized.




**Returns:**

A string containing the details about the event.


This function returns a string representation of the [**FramebufferResizeEvent**](class_a_g_e_1_1_framebuffer_resize_event.md) object. The returned string includes the width and height of the framebuffer that was resized.




**Returns:**

A string containing the details about the event, in the format "FramebufferResizeEvent: &lt;width&gt;, &lt;height&gt;". 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/ApplicationEvent.h`

