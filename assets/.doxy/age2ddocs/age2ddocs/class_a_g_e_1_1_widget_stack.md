

# Class AGE::WidgetStack



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WidgetStack**](class_a_g_e_1_1_widget_stack.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ActivateWidget**](#function-activatewidget) () <br> |
|  void | [**DeactivateWidget**](#function-deactivatewidget) () <br> |
|  Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; | [**GetActiveWidget**](#function-getactivewidget) () <br> |
|  void | [**OnTopUpdate**](#function-ontopupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**PopWidgetFromStack**](#function-popwidgetfromstack) () <br> |
|  void | [**PushWidgetToStack**](#function-pushwidgettostack) (Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; Widget) <br> |
|   | [**WidgetStack**](#function-widgetstack) () = default<br> |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::iterator | [**begin**](#function-begin-12) () <br> |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br> |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::iterator | [**end**](#function-end-12) () <br> |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::const\_iterator | [**end**](#function-end-22) () const<br> |
|   | [**~WidgetStack**](#function-widgetstack) () = default<br> |




























## Public Functions Documentation




### function ActivateWidget 

```C++
void AGE::WidgetStack::ActivateWidget () 
```




<hr>



### function DeactivateWidget 

```C++
void AGE::WidgetStack::DeactivateWidget () 
```




<hr>



### function GetActiveWidget 

```C++
inline Ref< ScriptableWidget > AGE::WidgetStack::GetActiveWidget () 
```




<hr>



### function OnTopUpdate 

```C++
void AGE::WidgetStack::OnTopUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function PopWidgetFromStack 

```C++
void AGE::WidgetStack::PopWidgetFromStack () 
```




<hr>



### function PushWidgetToStack 

```C++
void AGE::WidgetStack::PushWidgetToStack (
    Ref< ScriptableWidget > Widget
) 
```




<hr>



### function WidgetStack 

```C++
AGE::WidgetStack::WidgetStack () = default
```




<hr>



### function begin [1/2]

```C++
inline std::deque< Ref< ScriptableWidget > >::iterator AGE::WidgetStack::begin () 
```




<hr>



### function begin [2/2]

```C++
inline std::deque< Ref< ScriptableWidget > >::const_iterator AGE::WidgetStack::begin () const
```




<hr>



### function end [1/2]

```C++
inline std::deque< Ref< ScriptableWidget > >::iterator AGE::WidgetStack::end () 
```




<hr>



### function end [2/2]

```C++
inline std::deque< Ref< ScriptableWidget > >::const_iterator AGE::WidgetStack::end () const
```




<hr>



### function ~WidgetStack 

```C++
AGE::WidgetStack::~WidgetStack () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/WidgetStack.h`

