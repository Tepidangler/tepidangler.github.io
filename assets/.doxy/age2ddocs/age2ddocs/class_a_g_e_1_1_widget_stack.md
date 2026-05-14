

# Class AGE::WidgetStack



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WidgetStack**](class_a_g_e_1_1_widget_stack.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ActivateWidget**](#function-activatewidget) () <br>_Activates the widget at the front of the stack by setting its visibility to true._  |
|  void | [**DeactivateWidget**](#function-deactivatewidget) () <br>_Deactivates the widget at the front of the stack by setting its visibility to false._  |
|  Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; | [**GetActiveWidget**](#function-getactivewidget) () <br>_This function returns the active widget from the list of widgets._  |
|  void | [**OnTopUpdate**](#function-ontopupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function updates the topmost widget in the stack based on a given time step._  |
|  void | [**PopWidgetFromStack**](#function-popwidgetfromstack) () <br>_Removes the first widget from the stack._  |
|  void | [**PushWidgetToStack**](#function-pushwidgettostack) (Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; Widget) <br>_Pushes a_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _to the front of the stack._ |
|   | [**WidgetStack**](#function-widgetstack) () = default<br>_Default constructor for the_ [_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class. This function initializes an instance of the_[_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class with its members set to their default values._ |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::iterator | [**begin**](#function-begin-12) () <br>_Returns an iterator pointing to the beginning of the deque container storing_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _objects._ |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br>_Returns a constant iterator pointing to the beginning of the deque of_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _objects._ |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::iterator | [**end**](#function-end-12) () <br>_Returns an iterator pointing to the past-the-end element in the deque container._  |
|  std::deque&lt; Ref&lt; [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) &gt; &gt;::const\_iterator | [**end**](#function-end-22) () const<br>_Returns a constant iterator pointing to the past-the-end element of the deque container._  |
|   | [**~WidgetStack**](#function-widgetstack) () = default<br>_Destructor for the_ [_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class._ |




























## Public Functions Documentation




### function ActivateWidget 

_Activates the widget at the front of the stack by setting its visibility to true._ 
```C++
void AGE::WidgetStack::ActivateWidget () 
```



This function uses a member variable `m_Widgets`, which is assumed to be a container storing pointers to [**Widget**](struct_a_g_e_1_1_widget.md) objects. The front element of this container (i.e., the first added widget) is activated by calling the SetVisibility method on it with an argument of true.




**Returns:**

void


Activates the widget at the front of the stack by setting its visibility to true.


This function uses a member variable `m_Widgets`, which is assumed to be a container storing pointers to [**Widget**](struct_a_g_e_1_1_widget.md) objects. The front element of this container (i.e., the first added widget) will have its visibility set to true using the `SetVisibility(true)` method.




**Returns:**

void 





        

<hr>



### function DeactivateWidget 

_Deactivates the widget at the front of the stack by setting its visibility to false._ 
```C++
void AGE::WidgetStack::DeactivateWidget () 
```



This function removes the first element from the m\_Widgets vector and sets its visibility to false, effectively deactivating it. If the stack is empty, this function does nothing.


Deactivates the widget at the front of the stack by setting its visibility to false.


This function removes the first widget from the stack and sets its visibility to false, effectively deactivating it. If there are no widgets in the stack, this function does nothing. 


        

<hr>



### function GetActiveWidget 

_This function returns the active widget from the list of widgets._ 
```C++
inline Ref< ScriptableWidget > AGE::WidgetStack::GetActiveWidget () 
```





**Returns:**

A reference to the first element in the m\_Widgets vector, which is the active widget. If the vector is empty, it will return a default-constructed Ref&lt;ScriptableWidget&gt; object.


Retrieves the active widget from the list of widgets. 

**Returns:**

A reference to the frontmost widget in the list. If there are no widgets, a default-constructed Ref&lt;ScriptableWidget&gt; is returned. 





        

<hr>



### function OnTopUpdate 

_This function updates the topmost widget in the stack based on a given time step._ 
```C++
void AGE::WidgetStack::OnTopUpdate (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The amount of time that has passed since the last update.



**Returns:**

void


This function updates the top widget in the stack based on a given time step.


The function checks if there are any widgets in the stack (i.e., m\_Widgets size is greater than 0). If so, it calls the OnUpdate() method for the frontmost widget with the provided DeltaTime. This allows the top widget to be updated based on time elapsed since the last frame.




**Parameters:**


* `DeltaTime` The time step representing the amount of time that has passed since the last update.



**Returns:**

void 





        

<hr>



### function PopWidgetFromStack 

_Removes the first widget from the stack._ 
```C++
void AGE::WidgetStack::PopWidgetFromStack () 
```



This function removes the front element of the m\_Widgets list, effectively popping the topmost widget off the stack. If there are no widgets in the stack, this function does nothing and has no effect.


Removes the first widget from the stack.


This function removes the frontmost element of the m\_Widgets list, effectively "popping" the top-most widget off the stack. If the stack is empty, this operation has no effect. 


        

<hr>



### function PushWidgetToStack 

_Pushes a_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _to the front of the stack._
```C++
void AGE::WidgetStack::PushWidgetToStack (
    Ref< ScriptableWidget > Widget
) 
```



This function takes a reference to a [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) and pushes it onto the front of the m\_Widgets list. The widget is added at the beginning of the list, so it will be the next one to be popped off the stack. 

**Parameters:**


* [**Widget**](struct_a_g_e_1_1_widget.md) A reference to the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) that should be pushed onto the stack.

Pushes a [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) to the front of the stack.


This function takes in a reference to a [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) and pushes it to the front of the m\_Widgets list. The widget is added at the beginning of the list, so it will be the next one to be popped off the stack if PopNextWidgetFromStack() is called.




**Parameters:**


* [**Widget**](struct_a_g_e_1_1_widget.md) A reference to a [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) that you want to push onto the stack. 



**Returns:**

void No return value. 





        

<hr>



### function WidgetStack 

_Default constructor for the_ [_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class. This function initializes an instance of the_[_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class with its members set to their default values._
```C++
AGE::WidgetStack::WidgetStack () = default
```





**Returns:**

An instance of the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class with all member variables initialized to their default values.


Default constructor for the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class. This function initializes a new instance of the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class with an empty stack.




**Returns:**

A new instance of the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class. 





        

<hr>



### function begin [1/2]

_Returns an iterator pointing to the beginning of the deque container storing_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _objects._
```C++
inline std::deque< Ref< ScriptableWidget > >::iterator AGE::WidgetStack::begin () 
```





**Returns:**

An iterator that points to the start of the deque.


Returns an iterator pointing to the beginning of the deque container storing [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) objects. 

**Returns:**

An iterator pointing to the first element in the deque. If the deque is empty, the returned iterator will be equal to [**end()**](class_a_g_e_1_1_widget_stack.md#function-end-12). 





        

<hr>



### function begin [2/2]

_Returns a constant iterator pointing to the beginning of the deque of_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _objects._
```C++
inline std::deque< Ref< ScriptableWidget > >::const_iterator AGE::WidgetStack::begin () const
```





**Returns:**

A constant iterator pointing to the first element in the deque, or [**end()**](class_a_g_e_1_1_widget_stack.md#function-end-12) if the deque is empty.


Returns a constant iterator pointing to the beginning of the deque.


This function returns a constant iterator that points to the first element in the deque 'm\_Widgets'. The returned iterator can be used to access and traverse all elements from the start of the deque. 

**Returns:**

A constant iterator pointing to the beginning of the deque. 





        

<hr>



### function end [1/2]

_Returns an iterator pointing to the past-the-end element in the deque container._ 
```C++
inline std::deque< Ref< ScriptableWidget > >::iterator AGE::WidgetStack::end () 
```





**Returns:**

An iterator pointing to the past-the-end element of the sequence controlled by the deque object.


Returns an iterator pointing to the past-the-end element in the deque container. 

**Returns:**

An iterator to the past-the-end of the sequence controlled by the deque object. 





        

<hr>



### function end [2/2]

_Returns a constant iterator pointing to the past-the-end element of the deque container._ 
```C++
inline std::deque< Ref< ScriptableWidget > >::const_iterator AGE::WidgetStack::end () const
```





**Returns:**

A constant iterator pointing to the past-the-end element in the container.


Returns a constant iterator pointing to the past-the-end element of the deque container. 

**Returns:**

A constant iterator pointing to the past-the-end element in the container. 





        

<hr>



### function ~WidgetStack 

_Destructor for the_ [_**WidgetStack**_](class_a_g_e_1_1_widget_stack.md) _class._
```C++
AGE::WidgetStack::~WidgetStack () = default
```



This destructor is used to clean up any resources that were allocated during the lifetime of an object of this class. It does not perform any specific actions related to the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class, but serves as a standard way to define and document such a destructor in Doxygen.




**Returns:**

Nothing is returned as it's a destructor.


Destructor for the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class.


This destructor is used to clean up any resources that were allocated during the lifetime of an object of this class. It does not perform any specific operations related to the [**WidgetStack**](class_a_g_e_1_1_widget_stack.md) class itself, but serves as a standard way to define and document such a destructor in Doxygen.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/WidgetStack.h`

