

# Class AGE::WidgetActivatedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WidgetActivatedEvent**](class_a_g_e_1_1_widget_activated_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)
























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  uint8\_t | [**GetStack**](#function-getstack) () const<br> |
|  Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; | [**GetWidget**](#function-getwidget) () const<br> |
|   | [**WidgetActivatedEvent**](#function-widgetactivatedevent) (const Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; UIWidget, uint8\_t Stack) <br> |


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




### function GetStack 

```C++
inline uint8_t AGE::WidgetActivatedEvent::GetStack () const
```




<hr>



### function GetWidget 

```C++
inline Ref< ScriptableWidget > AGE::WidgetActivatedEvent::GetWidget () const
```




<hr>



### function WidgetActivatedEvent 

```C++
inline AGE::WidgetActivatedEvent::WidgetActivatedEvent (
    const Ref< ScriptableWidget > UIWidget,
    uint8_t Stack
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/UIEvent.h`

