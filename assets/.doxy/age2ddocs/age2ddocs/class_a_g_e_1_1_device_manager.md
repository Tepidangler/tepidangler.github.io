

# Class AGE::DeviceManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**DeviceManager**](class_a_g_e_1_1_device_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**DeviceManager**](#function-devicemanager) (AudioEngineType AudioEngine, bool UseXInput=false) <br>_Constructs a_ [_**DeviceManager**_](class_a_g_e_1_1_device_manager.md) _object._ |
|  [**AudioManager**](class_a_g_e_1_1_audio_manager.md) & | [**GetAudioManager**](#function-getaudiomanager) () <br>_Returns a reference to the global instance of the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _class._ |
|  [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md) & | [**GetWindow**](#function-getwindow) () <br>_Returns a reference to the main application window._  |
|  void | [**UpdateWindow**](#function-updatewindow) () <br>_This function updates the window by calling OnUpdate method of m\_Window object._  |
| virtual  | [**~DeviceManager**](#function-devicemanager) () = default<br>_Virtual destructor for the_ [_**DeviceManager**_](class_a_g_e_1_1_device_manager.md) _class._ |




























## Public Functions Documentation




### function DeviceManager 

_Constructs a_ [_**DeviceManager**_](class_a_g_e_1_1_device_manager.md) _object._
```C++
AGE::DeviceManager::DeviceManager (
    AudioEngineType AudioEngine,
    bool UseXInput=false
) 
```



This constructor initializes the device manager with an audio engine type and a boolean flag indicating whether to use XInput or not. It creates an [**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md), [**AudioManager**](class_a_g_e_1_1_audio_manager.md), and optionally an XInput instance based on the input parameters. The initialization is logged using CoreLogger::Info().




**Parameters:**


* [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) The type of audio engine to be used by the device manager. 
* `UseXInput` A boolean flag indicating whether or not to use XInput. 




        

<hr>



### function GetAudioManager 

_Returns a reference to the global instance of the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _class._
```C++
inline AudioManager & AGE::DeviceManager::GetAudioManager () 
```



This function returns a reference to the globally accessible instance of the [**AudioManager**](class_a_g_e_1_1_audio_manager.md) class, which is used for managing audio in the application. The returned object can be used to interact with the audio system.




**Returns:**

Reference to the global [**AudioManager**](class_a_g_e_1_1_audio_manager.md) instance. 





        

<hr>



### function GetWindow 

_Returns a reference to the main application window._ 
```C++
inline AGEWindow & AGE::DeviceManager::GetWindow () 
```



This function returns a reference to the main application window, which is used throughout the program for various operations such as rendering and user input handling.




**Returns:**

A reference to the main application window ([**AGEWindow**](class_a_g_e_1_1_a_g_e_window.md)&). 





        

<hr>



### function UpdateWindow 

_This function updates the window by calling OnUpdate method of m\_Window object._ 
```C++
inline void AGE::DeviceManager::UpdateWindow () 
```



The function does not take any parameters and returns nothing. It directly calls the OnUpdate() method on the m\_Window object, which presumably handles updating the window's content or properties based on some internal state. 


        

<hr>



### function ~DeviceManager 

_Virtual destructor for the_ [_**DeviceManager**_](class_a_g_e_1_1_device_manager.md) _class._
```C++
virtual AGE::DeviceManager::~DeviceManager () = default
```



This function is responsible for releasing any resources that were acquired by the [**DeviceManager**](class_a_g_e_1_1_device_manager.md) instance, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/DeviceManager.h`

