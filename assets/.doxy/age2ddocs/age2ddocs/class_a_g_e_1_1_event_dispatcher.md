

# Class AGE::EventDispatcher



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**Dispatch**](#function-dispatch) (EventFn&lt; T &gt; func) <br>_Dispatches an event of type T to the provided function if its type matches the static type of T._  |
|   | [**EventDispatcher**](#function-eventdispatcher) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br>_Constructor for the_ [_**EventDispatcher**_](class_a_g_e_1_1_event_dispatcher.md) _class._ |




























## Public Functions Documentation




### function Dispatch 

_Dispatches an event of type T to the provided function if its type matches the static type of T._ 
```C++
template<typename T>
inline bool AGE::EventDispatcher::Dispatch (
    EventFn< T > func
) 
```



This function takes a function object (or lambda) that accepts an argument of type T and returns void. It checks if the event's type is equal to the static type of T, then it calls the function with the event casted to type T. The function sets the 'Handled' member variable of the event to true if the event was handled by the provided function.




**Parameters:**


* `func` A function object (or lambda) that accepts an argument of type T and returns void. 



**Returns:**

True if the event was dispatched, false otherwise.


Dispatches an event of type T to the provided function if its type matches the static type of T.


This function takes a function object (func) as input and checks if the event's type is equal to the static type of T. If it is, the function object is invoked with the event casted to type T. The result of this operation is stored in the 'Handled' member of the event.




**Parameters:**


* `func` Function object (event handler) that will be called if the event matches the static type of T. 



**Returns:**

True if the event was dispatched, false otherwise. 





        

<hr>



### function EventDispatcher 

_Constructor for the_ [_**EventDispatcher**_](class_a_g_e_1_1_event_dispatcher.md) _class._
```C++
inline AGE::EventDispatcher::EventDispatcher (
    Event & Event
) 
```





**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event to be dispatched.

Constructs an instance of the [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md) class with a reference to an event object. 

**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event object that this dispatcher will handle. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/Event.h`

