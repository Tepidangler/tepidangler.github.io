

# Class AGE::InstrumentationTimer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**InstrumentationTimer**](class_a_g_e_1_1_instrumentation_timer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**InstrumentationTimer**](#function-instrumentationtimer) (const char \* name) <br>_Constructs an_ [_**InstrumentationTimer**_](class_a_g_e_1_1_instrumentation_timer.md) _object with a given name._ |
|  void | [**Stop**](#function-stop) () <br>_Stops the timer and writes a profile to the instrumentor._  |
|   | [**~InstrumentationTimer**](#function-instrumentationtimer) () <br>_Destructor for the_ [_**InstrumentationTimer**_](class_a_g_e_1_1_instrumentation_timer.md) _class. Stops the timer if it has not been stopped already._ |




























## Public Functions Documentation




### function InstrumentationTimer 

_Constructs an_ [_**InstrumentationTimer**_](class_a_g_e_1_1_instrumentation_timer.md) _object with a given name._
```C++
inline AGE::InstrumentationTimer::InstrumentationTimer (
    const char * name
) 
```



The constructor initializes the timer with the provided name and sets m\_Stopped to false. It also records the current time point using std::chrono::steady\_clock::now() and stores it in m\_StartTimepoint. 

**Parameters:**


* `name` A string representing the name of the instrumentation timer.

Constructs an [**InstrumentationTimer**](class_a_g_e_1_1_instrumentation_timer.md) object with a given name. 

**Parameters:**


* `name` The name to be associated with the timer.

This constructor initializes the timer with the provided name and sets m\_Stopped to false, indicating that the timer is not stopped yet. It also records the current time point using std::chrono::steady\_clock::now() and stores it in m\_StartTimepoint. 


        

<hr>



### function Stop 

_Stops the timer and writes a profile to the instrumentor._ 
```C++
inline void AGE::InstrumentationTimer::Stop () 
```



This function stops the timer by capturing the current time point using `std::chrono::steady_clock::now()`, calculates the elapsed time since the start timepoint was set in microseconds, then writes this information along with other details such as the name of the timer and the ID of the thread to the instrumentor.




**Returns:**

void


Stops the timer and writes a profile to the instrumentor.


This function measures the time elapsed since the start of the timer, writes this information to the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md), and then resets the timer. The profile includes the name of the timer, the start time, the elapsed time, and the ID of the thread that executed the code.




**Returns:**

void 





        

<hr>



### function ~InstrumentationTimer 

_Destructor for the_ [_**InstrumentationTimer**_](class_a_g_e_1_1_instrumentation_timer.md) _class. Stops the timer if it has not been stopped already._
```C++
inline AGE::InstrumentationTimer::~InstrumentationTimer () 
```



Destructor for the [**InstrumentationTimer**](class_a_g_e_1_1_instrumentation_timer.md) class. Stops the timer if it hasn't been stopped already. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Debug/Public/Instrumentor.h`

