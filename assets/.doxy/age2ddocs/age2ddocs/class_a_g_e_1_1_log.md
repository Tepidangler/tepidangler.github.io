

# Class AGE::Log



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Log**](class_a_g_e_1_1_log.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; spdlog::logger &gt; & | [**GetCoreLogger**](#function-getcorelogger) () <br>_This function returns a reference to the core logger used by the application._  |
|  Ref&lt; spdlog::logger &gt; & | [**GetGameLogger**](#function-getgamelogger) () <br>_This function returns a reference to the game logger object._  |
|  std::vector&lt; char &gt; & | [**GetLogs**](#function-getlogs) () <br>_This function returns a reference to the vector 's\_Logs'. The purpose of this function is to provide access to the logs for other parts of the program._  |
|  std::vector&lt; size\_t &gt; & | [**GetOffsets**](#function-getoffsets) () <br>_This function returns a reference to the vector_ `s_Offsets` _which is used for storing offset values._ |
|  std::vector&lt; LogType &gt; & | [**GetTypes**](#function-gettypes) () <br>_Returns a reference to the internal vector of LogTypes._  |
|  void | [**Init**](#function-init) () <br>_Initializes the logging system with specific formatting and log levels for two different logger instances, "AGECORE" and "AGEGAME". The pattern used is "[TIME] NAME: MESSAGE", where TIME represents the time at which the message was logged, NAME is the name of the logger instance that produced the message, and MESSAGE is the actual log message._  |


























## Public Static Functions Documentation




### function GetCoreLogger 

_This function returns a reference to the core logger used by the application._ 
```C++
static inline Ref< spdlog::logger > & AGE::Log::GetCoreLogger () 
```





**Returns:**

A reference to the core logger.


This function returns a reference to the core logger of the application. The core logger is used for logging messages that are important and should be visible in all parts of the application. It's implemented as an inline static member function of the Application class, so it can be accessed directly from anywhere within the code without needing to create a new instance every time. 

**Returns:**

A reference to the core logger object. 





        

<hr>



### function GetGameLogger 

_This function returns a reference to the game logger object._ 
```C++
static inline Ref< spdlog::logger > & AGE::Log::GetGameLogger () 
```



The game logger is used for logging messages related to the gameplay. It provides detailed information about what's happening in the game, which can be useful for debugging and performance tuning.




**Returns:**

A reference to the game logger object.


This function returns a reference to the game logger object. 

**Returns:**

A reference to the game logger object. 





        

<hr>



### function GetLogs 

_This function returns a reference to the vector 's\_Logs'. The purpose of this function is to provide access to the logs for other parts of the program._ 
```C++
static inline std::vector< char > & AGE::Log::GetLogs () 
```





**Returns:**

A reference to the vector 's\_Logs'


This function returns a reference to the vector 's\_Logs'. The purpose of this function is to provide access to the logs for other parts of the program. 

**Returns:**

A reference to the vector 's\_Logs' 





        

<hr>



### function GetOffsets 

_This function returns a reference to the vector_ `s_Offsets` _which is used for storing offset values._
```C++
static inline std::vector< size_t > & AGE::Log::GetOffsets () 
```





**Returns:**

A reference to the vector `s_Offsets`.


This function returns a reference to the vector 's\_Offsets'. It is used for storing offset values. 

**Returns:**

A reference to the vector 's\_Offsets' 





        

<hr>



### function GetTypes 

_Returns a reference to the internal vector of LogTypes._ 
```C++
static inline std::vector< LogType > & AGE::Log::GetTypes () 
```





**Returns:**

Reference to the internal vector of LogTypes.


This function returns a reference to the vector `s_Type` which holds all possible log types. 

**Returns:**

A reference to the vector of LogTypes. 





        

<hr>



### function Init 

_Initializes the logging system with specific formatting and log levels for two different logger instances, "AGECORE" and "AGEGAME". The pattern used is "[TIME] NAME: MESSAGE", where TIME represents the time at which the message was logged, NAME is the name of the logger instance that produced the message, and MESSAGE is the actual log message._ 
```C++
static void AGE::Log::Init () 
```





**Returns:**

void


Initializes the logging system with specific format and log levels for two different logger instances, "AGECORE" and "AGEGAME". The pattern set is "%^[%T] %n: %v%$", which includes timestamp, logger name, and message in color. Both loggers are set to trace level. 

**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Log.h`

