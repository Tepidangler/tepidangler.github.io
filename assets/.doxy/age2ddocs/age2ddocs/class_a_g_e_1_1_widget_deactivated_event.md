

# Class AGE::WidgetDeactivatedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WidgetDeactivatedEvent**](class_a_g_e_1_1_widget_deactivated_event.md)








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
|  Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; | [**GetWidget**](#function-getwidget) () const<br>_Returns the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _object associated with this instance._ |
|   | [**WidgetDeactivatedEvent**](#function-widgetdeactivatedevent) (const Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; UIWidget, uint8\_t Stack) <br>_Constructs a new instance of_ [_**WidgetDeactivatedEvent**_](class_a_g_e_1_1_widget_deactivated_event.md) _._ |


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
inline uint8_t AGE::WidgetDeactivatedEvent::GetStack () const
```





**Returns:**

uint8\_t Returns the current value of the stack variable as a uint8\_t type.


This function returns the current value of the stack variable. 

**Returns:**

uint8\_t The current value of the stack variable. 





        

<hr>



### function GetWidget 

_Returns the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _object associated with this instance._
```C++
inline Ref< ScriptableWidget > AGE::WidgetDeactivatedEvent::GetWidget () const
```





**Returns:**

A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) object. If no such object exists, returns an empty Ref&lt;ScriptableWidget&gt;.


Returns the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) object associated with this instance. 

**Returns:**

A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) object. If no such object exists, an empty Ref will be returned. 





        

<hr>



### function WidgetDeactivatedEvent 

_Constructs a new instance of_ [_**WidgetDeactivatedEvent**_](class_a_g_e_1_1_widget_deactivated_event.md) _._
```C++
inline AGE::WidgetDeactivatedEvent::WidgetDeactivatedEvent (
    const Ref< ScriptableWidget > UIWidget,
    uint8_t Stack
) 
```



This constructor initializes the object with the given parameters. It sets the stack level and the scriptable widget reference.




**Parameters:**


* `UIWidget` A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) that is deactivating. 
* `Stack` The stack level of the deactivated widget.

Constructs a new instance of [**Widget**](struct_a_g_e_1_1_widget.md) Deactivated [**Event**](class_a_g_e_1_1_event.md).


This constructor initializes the event with a reference to the Scriptable [**Widget**](struct_a_g_e_1_1_widget.md) and the stack number.




**Parameters:**


* `UIWidget` A const reference to the Scriptable [**Widget**](struct_a_g_e_1_1_widget.md) that is deactivating. 
* `Stack` The stack number of the widget being deactivated. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/UIEvent.h`

