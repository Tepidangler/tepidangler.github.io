

# Class AGE::TimeStep



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TimeStep**](class_a_g_e_1_1_time_step.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetMilliseconds**](#function-getmilliseconds) () const<br>_This function returns the time value in milliseconds._  |
|  float | [**GetSeconds**](#function-getseconds) () const<br>_This function returns the time value in seconds._  |
|   | [**TimeStep**](#function-timestep) (float time=0.f) <br>_Constructs a_ [_**TimeStep**_](class_a_g_e_1_1_time_step.md) _object with the given time value. If no argument is provided, it defaults to 0._ |
|   | [**operator float**](#function-operator-float) () const<br>_Converts the object into a floating-point number representing time._  |




























## Public Functions Documentation




### function GetMilliseconds 

_This function returns the time value in milliseconds._ 
```C++
inline float AGE::TimeStep::GetMilliseconds () const
```





**Returns:**

The time value multiplied by 1000 to convert it into milliseconds.


This function returns the time value in milliseconds. 

**Returns:**

The time value multiplied by 1000 to convert it into milliseconds. 





        

<hr>



### function GetSeconds 

_This function returns the time value in seconds._ 
```C++
inline float AGE::TimeStep::GetSeconds () const
```





**Returns:**

A float representing the time in seconds.


This function returns the time value in seconds. 

**Returns:**

A float representing the time in seconds. 





        

<hr>



### function TimeStep 

_Constructs a_ [_**TimeStep**_](class_a_g_e_1_1_time_step.md) _object with the given time value. If no argument is provided, it defaults to 0._
```C++
inline AGE::TimeStep::TimeStep (
    float time=0.f
) 
```





**Parameters:**


* `time` The time value for this [**TimeStep**](class_a_g_e_1_1_time_step.md). Defaults to 0 if not specified.

Constructs a [**TimeStep**](class_a_g_e_1_1_time_step.md) object with the given time value. If no argument is provided, it defaults to 0. 

**Parameters:**


* `time` The time value for this [**TimeStep**](class_a_g_e_1_1_time_step.md). Defaults to 0 if not specified. 




        

<hr>



### function operator float 

_Converts the object into a floating-point number representing time._ 
```C++
inline AGE::TimeStep::operator float () const
```



This function returns the value of 'm\_Time' which is a private member variable of this class. It provides an implicit conversion to float, allowing it to be used in arithmetic expressions where a float is expected.




**Returns:**

A floating-point number representing the time stored in 'm\_Time'.


Converts the object to a floating-point number representing time.


This function returns the value of the 'm\_Time' member variable, which represents time in some unit. The exact meaning and interpretation of this value is not specified here.




**Returns:**

A float representing the current time value. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/DeltaTime.h`

