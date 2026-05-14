

# Namespace AGE::CoreLogger



[**Namespace List**](namespaces.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**CoreLogger**](namespace_a_g_e_1_1_core_logger.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Assert**](#function-assert) (bool Condition, std::string\_view fmt, Args &&... args) <br>_This function is used for asserting conditions in the code. If the condition is false, it throws an exception with a formatted message._  |
|  void | [**Critical**](#function-critical) (std::string\_view fmt, Args &&... args) <br>_This function logs a critical message to the system. The message is formatted using fmt::format and includes the prefix "[AGECORE] ". It also pushes each character of the logged string into_ [_**Log::GetLogs()**_](class_a_g_e_1_1_log.md#function-getlogs) _for later analysis, increments the offset by the size of the logged string, and sets the log type to Critical. The function supports both Windows and Linux platforms via preprocessor directives._ |
|  void | [**Error**](#function-error) (std::string\_view fmt, Args &&... args) <br>_This function logs an error message to the core logger and various other logging systems. The error message is formatted using a variadic template, allowing for flexible formatting of the error message._  |
|  void | [**Info**](#function-info) (std::string\_view fmt, Args &&... args) <br>_This function logs informational messages to the console and a debug log file._  |
|  void | [**Trace**](#function-trace) (std::string\_view fmt, Args &&... args) <br>_This function logs a trace message with the specified format and arguments. The formatted string is prefixed with "[AGECORE] ". It also adds each character of the log line to_ [_**Log::GetLogs()**_](class_a_g_e_1_1_log.md#function-getlogs) _and updates_[_**Log::GetOffsets()**_](class_a_g_e_1_1_log.md#function-getoffsets) _._ |
|  void | [**Warn**](#function-warn) (std::string\_view fmt, Args &&... args) <br>_This function logs a warning message to the console and stores it in the log buffer for later retrieval._  |




























## Public Functions Documentation




### function Assert 

_This function is used for asserting conditions in the code. If the condition is false, it throws an exception with a formatted message._ 
```C++
template<typename ... Args>
void AGE::CoreLogger::Assert (
    bool Condition,
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `Condition` The condition to be checked. It should evaluate to true if the program state is valid and false otherwise. 
* `fmt` A format string that describes how the arguments should be formatted when included into the error message. 
* `args` Variadic arguments representing values to include in the error message. 



**Returns:**

void This function does not return a value. It throws an exception if the condition is false.


This function is used for asserting a condition in the code. If the condition is not met, it throws an exception with a formatted message. 

**Parameters:**


* `Condition` The boolean condition to be checked. 
* `fmt` A format string that will be used to create the error message if the condition is false. 
* `args` Arguments for the format string. 




        

<hr>



### function Critical 

_This function logs a critical message to the system. The message is formatted using fmt::format and includes the prefix "[AGECORE] ". It also pushes each character of the logged string into_ [_**Log::GetLogs()**_](class_a_g_e_1_1_log.md#function-getlogs) _for later analysis, increments the offset by the size of the logged string, and sets the log type to Critical. The function supports both Windows and Linux platforms via preprocessor directives._
```C++
template<typename ... Args>
void AGE::CoreLogger::Critical (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A std::string\_view representing the format string for the message. 
* `args` Variadic arguments representing the values to be formatted into the message. 



**Returns:**

void


This function logs a critical message to the system. The log includes the formatted string and arguments, along with additional information such as timestamp and log level. It also pushes each character of the log line into [**Log::GetLogs()**](class_a_g_e_1_1_log.md#function-getlogs).




**Parameters:**


* `fmt` A std::string\_view representing the format string for the message to be logged. 
* `args` Variadic arguments representing the values to be formatted into the message.



**Returns:**

void 





        

<hr>



### function Error 

_This function logs an error message to the core logger and various other logging systems. The error message is formatted using a variadic template, allowing for flexible formatting of the error message._ 
```C++
template<typename ... Args>
void AGE::CoreLogger::Error (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A string\_view representing the format string for the error message. 
* `args` Variadic arguments representing the values to be inserted into the format string.



**Returns:**

void This function does not return a value.


This function logs an error message to the core logger, appending "[AGECORE]" before it. It also pushes each character of the logged string into [**Log::GetLogs()**](class_a_g_e_1_1_log.md#function-getlogs) and updates [**Log::GetOffsets()**](class_a_g_e_1_1_log.md#function-getoffsets). The log type is set as Error using LogType::Error. If AG\_PLATFORM\_WINDOWS is defined, it uses OutputDebugString to output the error message; if not, printf is used instead. 

**Parameters:**


* `fmt` A string\_view representing the format of the error message. 
* `args` Variadic arguments for the format string. 




        

<hr>



### function Info 

_This function logs informational messages to the console and a debug log file._ 
```C++
template<typename ... Args>
void AGE::CoreLogger::Info (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A format string that specifies how subsequent arguments are converted for output. 
* `args` Arguments referenced by the format specifiers in the format string.



**Returns:**

void 





        

<hr>



### function Trace 

_This function logs a trace message with the specified format and arguments. The formatted string is prefixed with "[AGECORE] ". It also adds each character of the log line to_ [_**Log::GetLogs()**_](class_a_g_e_1_1_log.md#function-getlogs) _and updates_[_**Log::GetOffsets()**_](class_a_g_e_1_1_log.md#function-getoffsets) _._
```C++
template<typename ... Args>
void AGE::CoreLogger::Trace (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A std::string\_view representing the format string for the trace message. 
* `args` Variadic arguments representing the values to be formatted into the trace message.



**Returns:**

void


This function logs a trace message to the system's debug output and also stores it in the log buffer for later retrieval.




**Parameters:**


* `fmt` The format string used to create the logged message. It should follow the same syntax as printf/scanf functions. 
* `args` Variadic arguments that correspond to the placeholders in the format string.



**Returns:**

void 





        

<hr>



### function Warn 

_This function logs a warning message to the console and stores it in the log buffer for later retrieval._ 
```C++
template<typename ... Args>
void AGE::CoreLogger::Warn (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` The format string used to create the warning message. It should follow the same syntax as printf or std::format. 
* `args` The arguments that will be substituted into the format string.



**Returns:**

None


This function logs a warning message to the console and stores it for later retrieval.




**Parameters:**


* `fmt` The format string used to create the warning message. It should follow the same syntax as printf/scanf functions in C++. 
* `args` Variadic arguments that correspond to the placeholders in the format string.



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Log.h`

