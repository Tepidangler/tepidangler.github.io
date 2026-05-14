

# Class AGE::RendererChangeEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RendererChangeEvent**](class_a_g_e_1_1_renderer_change_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)
























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) \* | [**GetWindow**](#function-getwindow) () const<br>_Returns the window object associated with this class instance._  |
|   | [**RendererChangeEvent**](#function-rendererchangeevent) ([**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) \* Window) <br>_Constructor for_ [_**RendererChangeEvent**_](class_a_g_e_1_1_renderer_change_event.md) _class._ |
| virtual std::string | [**ToString**](#function-tostring) () override const<br>_Converts the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _object to a string representation._ |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















































## Public Functions Documentation




### function GetWindow 

_Returns the window object associated with this class instance._ 
```C++
inline AGEWindow * AGE::RendererChangeEvent::GetWindow () const
```





**Returns:**

Pointer to an [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) object representing the current window. 





        

<hr>



### function RendererChangeEvent 

_Constructor for_ [_**RendererChangeEvent**_](class_a_g_e_1_1_renderer_change_event.md) _class._
```C++
inline AGE::RendererChangeEvent::RendererChangeEvent (
    AGEWindow * Window
) 
```



This constructor initializes the [**RendererChangeEvent**](class_a_g_e_1_1_renderer_change_event.md) object with a reference to an [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) instance. It is used to handle changes in the renderer of the provided window.




**Parameters:**


* `Window` Pointer to an [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) instance representing the window whose renderer will be changed. 




        

<hr>



### function ToString 

_Converts the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _object to a string representation._
```C++
inline virtual std::string AGE::RendererChangeEvent::ToString () override const
```



This function returns a string that represents the current state of the [**Renderer**](class_a_g_e_1_1_renderer.md) object, including its type and any relevant details. The returned string is formatted as "Renderer Changed: [Utils::ConvertAPIToString()]", where [Utils::ConvertAPIToString()] represents the result of Utils::ConvertAPIToString().




**Returns:**

A string representation of the [**Renderer**](class_a_g_e_1_1_renderer.md) object. 





        
Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/RendererEvent.h`

