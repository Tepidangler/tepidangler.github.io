

# Class AGE::WindowResizeEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)
























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  unsigned int | [**GetHeight**](#function-getheight) () const<br> |
|  unsigned int | [**GetWidth**](#function-getwidth) () const<br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br> |
|   | [**WindowResizeEvent**](#function-windowresizeevent) (unsigned int Width, unsigned int Height) <br> |


## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















































## Public Functions Documentation




### function GetHeight 

```C++
inline unsigned int AGE::WindowResizeEvent::GetHeight () const
```




<hr>



### function GetWidth 

```C++
inline unsigned int AGE::WindowResizeEvent::GetWidth () const
```




<hr>



### function ToString 

```C++
inline virtual std::string AGE::WindowResizeEvent::ToString () override const
```



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

