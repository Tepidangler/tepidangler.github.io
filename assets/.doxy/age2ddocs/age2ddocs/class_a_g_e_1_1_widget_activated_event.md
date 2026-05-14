

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
|  uint8\_t | [**GetStack**](#function-getstack) () const<br>_This function returns the current value of the stack variable._  |
|  Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; | [**GetWidget**](#function-getwidget) () const<br>_Returns the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _instance associated with this object._ |
|   | [**WidgetActivatedEvent**](#function-widgetactivatedevent) (const Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; UIWidget, uint8\_t Stack) <br>_Constructs a new instance of_ [_**WidgetActivatedEvent**_](class_a_g_e_1_1_widget_activated_event.md) _._ |


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




### function GetStack 

_This function returns the current value of the stack variable._ 
```C++
inline uint8_t AGE::WidgetActivatedEvent::GetStack () const
```





**Returns:**

The current value of the stack as a uint8\_t.


This function returns the value of member variable 'm\_Stack'. 

**Returns:**

uint8\_t Returns the current value of 'm\_Stack' as a uint8\_t. 





        

<hr>



### function GetWidget 

_Returns the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _instance associated with this object._
```C++
inline Ref< ScriptableWidget > AGE::WidgetActivatedEvent::GetWidget () const
```





**Returns:**

A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) instance. If no such instance exists, a default-constructed one is returned.


Returns the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) object associated with this instance. 

**Returns:**

A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) object. If no such object exists, an empty Ref&lt;ScriptableWidget&gt; is returned. 





        

<hr>



### function WidgetActivatedEvent 

_Constructs a new instance of_ [_**WidgetActivatedEvent**_](class_a_g_e_1_1_widget_activated_event.md) _._
```C++
inline AGE::WidgetActivatedEvent::WidgetActivatedEvent (
    const Ref< ScriptableWidget > UIWidget,
    uint8_t Stack
) 
```





**Parameters:**


* `UIWidget` A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) that triggered this event. 
* `Stack` The stack depth at which the widget was activated. 



**Returns:**

An instance of [**WidgetActivatedEvent**](class_a_g_e_1_1_widget_activated_event.md) with the provided parameters.


Constructs a new instance of [**WidgetActivatedEvent**](class_a_g_e_1_1_widget_activated_event.md).


This constructor initializes the object with a reference to a [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) and a stack index. The [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) is used for interacting with the UI, while the stack index is used to track which widget in the stack this event corresponds to. 

**Parameters:**


* `UIWidget` A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) that this event pertains to. 
* `Stack` The index of the widget in the stack that this event corresponds to. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/UIEvent.h`

