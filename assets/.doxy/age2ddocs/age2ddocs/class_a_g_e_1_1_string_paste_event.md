

# Class AGE::StringPasteEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**StringPasteEvent**](class_a_g_e_1_1_string_paste_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)
























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  const char \* | [**GetString**](#function-getstring) () <br> |
|   | [**StringPasteEvent**](#function-stringpasteevent) (const char \* String) <br> |
| virtual std::string | [**ToString**](#function-tostring) () override const<br> |


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




### function GetString 

```C++
inline const char * AGE::StringPasteEvent::GetString () 
```




<hr>



### function StringPasteEvent 

```C++
inline AGE::StringPasteEvent::StringPasteEvent (
    const char * String
) 
```




<hr>



### function ToString 

```C++
inline virtual std::string AGE::StringPasteEvent::ToString () override const
```



Implements [*AGE::Event::ToString*](class_a_g_e_1_1_event.md#function-tostring)


<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/ApplicationEvent.h`

