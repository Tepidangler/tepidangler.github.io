

# Class AGE::Instrumentor



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Instrumentor**](class_a_g_e_1_1_instrumentor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginSession**](#function-beginsession) (const std::string & name, const std::string & filepath="results.json") <br>_Starts a new instrumentation session._  |
|  void | [**EndSession**](#function-endsession) () <br>_This function is used to end the session. It locks a mutex and then calls an internal function to actually end the session._  |
|   | [**Instrumentor**](#function-instrumentor-13) (const [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) &) = delete<br>_Deleted copy constructor for the_ [_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _class to prevent copying._ |
|   | [**Instrumentor**](#function-instrumentor-23) ([**Instrumentor**](class_a_g_e_1_1_instrumentor.md) &&) = delete<br>[_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _move constructor is deleted to prevent copying of the instrumentor object._ |
|  void | [**WriteProfile**](#function-writeprofile) (const [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) & result) <br>_Writes a profile result to an output stream in JSON format._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) & | [**Get**](#function-get) () <br>_Returns a reference to the singleton instance of the_ [_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _class._ |


























## Public Functions Documentation




### function BeginSession 

_Starts a new instrumentation session._ 
```C++
inline void AGE::Instrumentor::BeginSession (
    const std::string & name,
    const std::string & filepath="results.json"
) 
```



This function starts a new session with the given name and writes the header to the output stream. If there is an existing session, it will be closed before starting the new one. The results of profiling meant for the original session will end up in the newly opened session instead. 

**Parameters:**


* `name` The name of the new session. 
* `filepath` The path to the output JSON file. Defaults to "results.json".



**Returns:**

void


Starts a new profiling session.


This function starts a new profiling session with the given name and writes the header to the output stream. If there is already an active session, it will be closed before starting the new one. The results of any profiling data meant for the original session will instead go into the newly started session.




**Parameters:**


* `name` The name of the new session. This should ideally represent what the session is measuring or recording. 
* `filepath` Optional parameter specifying where to write the profiling data. Defaults to "results.json". 




        

<hr>



### function EndSession 

_This function is used to end the session. It locks a mutex and then calls an internal function to actually end the session._ 
```C++
inline void AGE::Instrumentor::EndSession () 
```





**Returns:**

void


This function is used to end the session. It ensures thread safety by using a std::lock\_guard on m\_Mutex. The actual work of ending the session is done by calling InternalEndSession(). 

**Returns:**

void 





        

<hr>



### function Instrumentor [1/3]

_Deleted copy constructor for the_ [_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _class to prevent copying._
```C++
AGE::Instrumentor::Instrumentor (
    const Instrumentor &
) = delete
```



This function is marked as deleted because we do not want any copies of an instance of this class. It's a good practice to avoid unnecessary copying and duplication in our code, which can lead to performance issues or memory leaks. The copy constructor for the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class has been set to private to prevent its use.


Deleted copy constructor for the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class.


This function is marked as deleted to prevent copying of an instance of this class, which would not make sense in the context of our application. 


        

<hr>



### function Instrumentor [2/3]

[_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _move constructor is deleted to prevent copying of the instrumentor object._
```C++
AGE::Instrumentor::Instrumentor (
    Instrumentor &&
) = delete
```



This function is marked as deleted in C++, which means that it cannot be used for creating a copy of an existing object. It's useful when we want to ensure that objects are not copied unintentionally and can only be moved.




**Returns:**

The move constructor is implicitly declared as deleted by the compiler if any non-static data member or base class has a user-declared destructor, copy assignment operator, or move assignment operator.


Move constructor for the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class. Deleted to prevent copying of objects. 

**Parameters:**


* `other` The object to be moved from. 




        

<hr>



### function WriteProfile 

_Writes a profile result to an output stream in JSON format._ 
```C++
inline void AGE::Instrumentor::WriteProfile (
    const ProfileResult & result
) 
```



This function takes a [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) object and writes it as a JSON string to the output stream. The JSON string includes details about the elapsed time, name of the operation, thread ID, and start timestamp. It also locks the mutex for thread safety. If the current session is active (m\_CurrentSession == true), the function writes the JSON string to the output stream and flushes it.




**Parameters:**


* `result` The [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) object to be written.

Writes a profile result to the output stream in JSON format.


This function takes a [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) object and writes its data into an output stream in JSON format. The data includes the category, duration, name, phase (X for unknown), process ID (0 as it's not applicable here), thread ID, and timestamp. It also locks a mutex to ensure thread safety when writing to the output stream. If the current session is active, the function writes the JSON string into the output stream and flushes it.




**Parameters:**


* `result` The [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) object containing data about the profile. 




        

<hr>
## Public Static Functions Documentation




### function Get 

_Returns a reference to the singleton instance of the_ [_**Instrumentor**_](class_a_g_e_1_1_instrumentor.md) _class._
```C++
static inline Instrumentor & AGE::Instrumentor::Get () 
```



This function creates and returns a reference to an instance of the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class, which is a part of the profiling system used in this application. The instance is created using the 'static' keyword, ensuring that it is only initialized once and reused across multiple calls.




**Returns:**

A reference to the singleton instance of the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class.


Returns a reference to the singleton instance of the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class.


This function creates and returns a static instance of the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class, ensuring that only one instance exists throughout the program's execution. The instance is returned as a reference, allowing for easy access and manipulation of its properties or methods.




**Returns:**

A reference to the singleton instance of the [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) class. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Debug/Public/Instrumentor.h`

