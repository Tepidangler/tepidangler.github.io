

# Class AGE::Timer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Timer**](class_a_g_e_1_1_timer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**Elapsed**](#function-elapsed) () <br>_This function returns the elapsed time in milliseconds since the start time 'm\_Start'._  |
|  float | [**ElapsedMillis**](#function-elapsedmillis) () <br>_This function returns the elapsed time in milliseconds since the last reset._  |
|  void | [**Reset**](#function-reset) () <br>_This function resets the start time to the current time._  |
|   | [**Timer**](#function-timer) () <br>_Constructor for the_ [_**Timer**_](class_a_g_e_1_1_timer.md) _class. It initializes a new instance of the_[_**Timer**_](class_a_g_e_1_1_timer.md) _and resets it._ |




























## Public Functions Documentation




### function Elapsed 

_This function returns the elapsed time in milliseconds since the start time 'm\_Start'._ 
```C++
inline float AGE::Timer::Elapsed () 
```



The function uses std::chrono to measure the duration between the current time and the start time. It then converts this duration from nanoseconds to milliseconds by dividing by 1,000,000 (since there are 1,000,000 nanoseconds in a millisecond). The result is returned as a float.




**Returns:**

A float representing the elapsed time in milliseconds.


This function returns the elapsed time in milliseconds since the start time 'm\_Start'.


The function uses a high resolution clock to measure the elapsed time and then converts it into milliseconds. It does this by first converting the duration into nanoseconds, then dividing by 1 million (to convert from nanoseconds to microseconds) and finally again by 1000 (to convert from microseconds to milliseconds). The result is a float representing the elapsed time in milliseconds.




**Returns:**

A float representing the elapsed time in milliseconds since 'm\_Start'. 





        

<hr>



### function ElapsedMillis 

_This function returns the elapsed time in milliseconds since the last reset._ 
```C++
inline float AGE::Timer::ElapsedMillis () 
```





**Returns:**

A float representing the elapsed time in milliseconds. If no timer has been set, it will return 0.0f.


This function returns the elapsed time in milliseconds.


The function multiplies the result of `Elapsed()` by 1000 to convert seconds into milliseconds. It assumes that `Elapsed()` is a function returning the elapsed time in seconds.




**Returns:**

A float representing the elapsed time in milliseconds. 





        

<hr>



### function Reset 

_This function resets the start time to the current time._ 
```C++
inline void AGE::Timer::Reset () 
```



The function uses `std::chrono` library to get the current time and store it in m\_Start variable. It is typically used at the beginning of a performance measurement session, setting the starting point for timing measurements.




**Returns:**

void


This function resets the start time to the current time.


The function uses `std::chrono` library to get the current time and assigns it to m\_Start variable. It is typically used in timing operations where you want to measure how much time has passed since a certain point.




**Returns:**

void 





        

<hr>



### function Timer 

_Constructor for the_ [_**Timer**_](class_a_g_e_1_1_timer.md) _class. It initializes a new instance of the_[_**Timer**_](class_a_g_e_1_1_timer.md) _and resets it._
```C++
inline AGE::Timer::Timer () 
```



Constructor for the [**Timer**](class_a_g_e_1_1_timer.md) class. Initializes a new instance of the timer and resets it to 0. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Timer.h`

