

# Namespace AGE::GameLogger



[**Namespace List**](namespaces.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GameLogger**](namespace_a_g_e_1_1_game_logger.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Assert**](#function-assert) (bool Condition, std::string\_view fmt, Args &&... args) <br>_This function is used to assert a condition. If the condition is not met, it throws an exception with a formatted message._  |
|  void | [**Critical**](#function-critical) (std::string\_view fmt, Args &&... args) <br>_This function logs a critical message to the game logger and various other logging systems._  |
|  void | [**Error**](#function-error) (std::string\_view fmt, Args &&... args) <br>_This function is used for logging errors in the game. It takes a format string and variable arguments, formats them into a line of text, logs it to various outputs (game log, debug output on Windows, standard output on Linux), and stores it for later retrieval._  |
|  void | [**Info**](#function-info) (std::string\_view fmt, Args &&... args) <br>_This function logs informational messages to the game logger and various other logging systems._  |
|  void | [**Trace**](#function-trace) (std::string\_view fmt, Args &&... args) <br>_This function traces a message to the game logger and various other logging systems._  |
|  void | [**Warn**](#function-warn) (std::string\_view fmt, Args &&... args) <br>_This function is used for logging warnings in the game. It takes a format string and variable arguments, formats them into a string, then logs this string as a warning along with other information such as log type and offsets. The formatted string is also added to the game's logs. If the platform is Windows, it uses OutputDebugString for logging; if it's Linux, printf is used instead._  |




























## Public Functions Documentation




### function Assert 

_This function is used to assert a condition. If the condition is not met, it throws an exception with a formatted message._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Assert (
    bool Condition,
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `Condition` The condition that needs to be checked. 
* `fmt` A format string for the error message. 
* `args` Arguments for the format string.

This function is used for asserting a condition in the code. If the condition is not met, it throws an exception with a formatted message. 

**Parameters:**


* `Condition` The boolean condition to be checked. 
* `fmt` A format string that describes what happened. 
* `args` Variadic arguments providing additional information about the event. 



**Returns:**

void This function does not return any value. It only throws exceptions in case of failure. 





        

<hr>



### function Critical 

_This function logs a critical message to the game logger and various other logging systems._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Critical (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` The format string for the log message. 
* `args` Variadic arguments used to fill in placeholders in the format string.



**Returns:**

None 





        

<hr>



### function Error 

_This function is used for logging errors in the game. It takes a format string and variable arguments, formats them into a line of text, logs it to various outputs (game log, debug output on Windows, standard output on Linux), and stores it for later retrieval._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Error (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` The format string used to generate the error message. This should be a printf-style format string. 
* `args` The variable arguments that will replace placeholders in the format string.



**Returns:**

void No return value is expected as this function only logs errors and does not handle them.


This function logs an error message to the game logger and various other logging systems.




**Parameters:**


* `fmt` A format string for the error message, which can include placeholders for variable arguments. 
* `args` The variable arguments that will be substituted into the format string.



**Returns:**

void 





        

<hr>



### function Info 

_This function logs informational messages to the game logger and various other logging systems._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Info (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A format string that specifies how subsequent arguments are converted for output. 
* `args` Arguments following the format string.



**Returns:**

None


This function logs informational messages to the game logger and various other logging systems.




**Parameters:**


* `fmt` A format string that specifies how subsequent arguments are converted for output. 
* `args` Arguments referenced by the format specifiers in the format string.



**Returns:**

void 





        

<hr>



### function Trace 

_This function traces a message to the game logger and various other logging systems._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Trace (
    std::string_view fmt,
    Args &&... args
) 
```



The function takes in a format string and variable arguments, formats them into a line of text, then logs this line both to the game logger and any number of additional loggers. It also records the offsets at which each character was logged for later retrieval.




**Parameters:**


* `fmt` A std::string\_view representing the format string. 
* `args` Variable arguments representing values to be inserted into the format string.



**Returns:**

void


This function traces a message to the game logger and various other logging systems.


The function takes a format string and variable arguments, formats them into a string with prefix "[AGEGAME] ", then logs this string to the game logger and various other logging systems. It also pushes each character of the logged string onto another log for later analysis. The offsets are updated accordingly.




**Parameters:**


* `fmt` A std::string\_view representing the format string. 
* `args` Variable arguments representing values to be formatted into the format string.



**Returns:**

void 





        

<hr>



### function Warn 

_This function is used for logging warnings in the game. It takes a format string and variable arguments, formats them into a string, then logs this string as a warning along with other information such as log type and offsets. The formatted string is also added to the game's logs. If the platform is Windows, it uses OutputDebugString for logging; if it's Linux, printf is used instead._ 
```C++
template<typename ... Args>
void AGE::GameLogger::Warn (
    std::string_view fmt,
    Args &&... args
) 
```





**Parameters:**


* `fmt` A format string that specifies how the remaining arguments are converted to strings. 
* `...args` Variable number of arguments, which will be formatted according to the provided format string. 



**Returns:**

void


This function logs a warning message with the given format string and arguments.


The formatted message is prefixed with "[AGEGAME] " and logged to various outputs based on the platform.




**Parameters:**


* `fmt` A std::string\_view representing the format string for the warning message. 
* `args` Variadic parameters representing the arguments for the format string.



**Returns:**

void This function does not return a value. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Log.h`

