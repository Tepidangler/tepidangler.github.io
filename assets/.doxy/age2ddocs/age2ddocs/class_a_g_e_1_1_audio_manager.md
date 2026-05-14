

# Class AGE::AudioManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AudioManager**](class_a_g_e_1_1_audio_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AudioManager**](#function-audiomanager) (AudioEngineType Type) <br>_Constructs an instance of the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _class._ |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; | [**GetAudioEngine**](#function-getaudioengine) () <br>_Returns the Audio Engine instance._  |
|  AudioEngineType | [**GetAudioEngineType**](#function-getaudioenginetype) () <br>_This function returns the type of audio engine being used by the application._  |
|  void | [**SwitchAudioEngine**](#function-switchaudioengine) (AudioEngineType Type) <br>_Switches the audio engine being used by the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _._ |




























## Public Functions Documentation




### function AudioManager 

_Constructs an instance of the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _class._
```C++
AGE::AudioManager::AudioManager (
    AudioEngineType Type
) 
```



This constructor initializes an instance of the [**AudioManager**](class_a_g_e_1_1_audio_manager.md) class with a specified audio engine type. It creates an instance of the appropriate audio engine based on the provided type and sets it as the current audio engine for the manager. The log message "Audio Manager Initialized!" is also printed to indicate successful initialization.




**Parameters:**


* `Type` - The type of audio engine that should be used by this [**AudioManager**](class_a_g_e_1_1_audio_manager.md) instance. This can be one of the values defined in the AudioEngineType enum, such as kOpenAL or kFMOD. 




        

<hr>



### function GetAudioEngine 

_Returns the Audio Engine instance._ 
```C++
inline Ref< AudioEngine > AGE::AudioManager::GetAudioEngine () 
```



This function returns a reference to an [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) object which is currently being used by the application. The returned object can be used for various audio processing tasks.




**Returns:**

Reference to the current [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) instance. 





        

<hr>



### function GetAudioEngineType 

_This function returns the type of audio engine being used by the application._ 
```C++
inline AudioEngineType AGE::AudioManager::GetAudioEngineType () 
```





**Returns:**

The type of [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) as an enumeration value (e.g., kAudioEngineType1, kAudioEngineType2). 





        

<hr>



### function SwitchAudioEngine 

_Switches the audio engine being used by the_ [_**AudioManager**_](class_a_g_e_1_1_audio_manager.md) _._
```C++
void AGE::AudioManager::SwitchAudioEngine (
    AudioEngineType Type
) 
```



This function resets the current audio engine and replaces it with a new one of the specified type. The new audio engine is initialized immediately after its creation.




**Parameters:**


* `Type` The type of the new audio engine to be created. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/DeviceManager.h`

