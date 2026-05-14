

# Class AGE::AGESound



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md)








Inherits the following classes: [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGESound**](#function-agesound) () <br>_Constructor for the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _class. Initializes the sound object with default values._ |
| virtual std::string & | [**GetCurrentEventName**](#function-getcurrenteventname) () override<br>_Get the name of the current event._  |
| virtual void | [**Init**](#function-init) () override<br> |
| virtual bool | [**IsEventValid**](#function-iseventvalid) (const std::string & EventName) override<br>_Checks whether the given event name is valid or not._  |
| virtual void | [**LoadBank**](#function-loadbank) (Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; Bank) override<br>_Loads a sound bank into the system._  |
| virtual void | [**LoadBanks**](#function-loadbanks) (const std::vector&lt; Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & Banks) override<br>_Loads a list of Sound Banks into the system._  |
| virtual void | [**LoadEvents**](#function-loadevents) () override<br> |
|  void | [**Play**](#function-play) (const Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & Source) <br>_Plays an audio source._  |
| virtual void | [**Set3DAttributes**](#function-set3dattributes) (void \* Attributes) override<br>_Sets the 3D attributes for the sound object._  |
| virtual void | [**SetCurrentEventName**](#function-setcurrenteventname) (const std::string & Name) override<br>_Set the name of the current event._  |
| virtual void | [**SetParameterByName**](#function-setparameterbyname) (const std::string & Name, float Value) override<br>_This function sets a parameter by its name._  |
| virtual void | [**Shutdown**](#function-shutdown) () override<br>_Shuts down the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._ |
| virtual void | [**Start**](#function-start) () override<br>_Starts the sound playback._  |
| virtual void | [**Stop**](#function-stop-13) () override<br>_Stops the sound from playing._  |
|  void | [**Stop**](#function-stop-23) (const Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & Source) <br>_Stops the audio source from playing._  |
|  void | [**Stop**](#function-stop-33) (const std::vector&lt; Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; & Sources) <br>_Stops all the audio sources in a given vector._  |
| virtual void | [**Update**](#function-update) () override<br>_Updates the sound object._  |
|   | [**~AGESound**](#function-agesound) () override<br>_Destructor for_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _class._ |


## Public Functions inherited from AGE::AudioEngine

See [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_audio_engine.md#function-as-12) () <br>_This function is a placeholder and will always fail an assertion. It's used as a stub for future development._  |
|  [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) \* | [**As**](class_a_g_e_1_1_audio_engine.md#function-as-22) () <br>_This function returns a pointer to the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._ |
| virtual std::string & | [**GetCurrentEventName**](class_a_g_e_1_1_audio_engine.md#function-getcurrenteventname) () = 0<br> |
| virtual void | [**Init**](class_a_g_e_1_1_audio_engine.md#function-init) () = 0<br> |
| virtual bool | [**IsEventValid**](class_a_g_e_1_1_audio_engine.md#function-iseventvalid) (const std::string & EventName) = 0<br> |
| virtual void | [**LoadBank**](class_a_g_e_1_1_audio_engine.md#function-loadbank) (Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; Bank) = 0<br> |
| virtual void | [**LoadBanks**](class_a_g_e_1_1_audio_engine.md#function-loadbanks) (const std::vector&lt; Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & Banks) = 0<br> |
| virtual void | [**LoadEvents**](class_a_g_e_1_1_audio_engine.md#function-loadevents) () = 0<br> |
| virtual void | [**Set3DAttributes**](class_a_g_e_1_1_audio_engine.md#function-set3dattributes) (void \* Attributes) = 0<br> |
| virtual void | [**SetCurrentEventName**](class_a_g_e_1_1_audio_engine.md#function-setcurrenteventname) (const std::string & Name) = 0<br> |
| virtual void | [**SetParameterByName**](class_a_g_e_1_1_audio_engine.md#function-setparameterbyname) (const std::string & Name, float Value) = 0<br> |
| virtual void | [**Shutdown**](class_a_g_e_1_1_audio_engine.md#function-shutdown) () = 0<br> |
| virtual void | [**Start**](class_a_g_e_1_1_audio_engine.md#function-start) () = 0<br> |
| virtual void | [**Stop**](class_a_g_e_1_1_audio_engine.md#function-stop) () = 0<br> |
| virtual void | [**Update**](class_a_g_e_1_1_audio_engine.md#function-update) () = 0<br> |
| virtual  | [**~AudioEngine**](class_a_g_e_1_1_audio_engine.md#function-audioengine) () = default<br>_Virtual destructor for the_ [_**AudioEngine**_](class_a_g_e_1_1_audio_engine.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AudioSource**](class_a_g_e_1_1_audio_source.md) | [**LoadAudioSource**](#function-loadaudiosource) (const std::string & FileName) <br>_Loads an audio source from a file._  |
|  void | [**SetDebugLogging**](#function-setdebuglogging) (bool Log) <br>_Set the debug logging state for the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._ |


## Public Static Functions inherited from AGE::AudioEngine

See [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; | [**Create**](class_a_g_e_1_1_audio_engine.md#function-create) (AudioEngineType Type) <br> |


















































## Public Functions Documentation




### function AGESound 

_Constructor for the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _class. Initializes the sound object with default values._
```C++
AGE::AGESound::AGESound () 
```



This constructor initializes an instance of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) class by calling the Init() function, which sets up any necessary resources or defaults for a sound object.




**Returns:**

void


Constructor for the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) class. Initializes a new instance of the sound object with default values. 


        

<hr>



### function GetCurrentEventName 

_Get the name of the current event._ 
```C++
virtual std::string & AGE::AGESound::GetCurrentEventName () override
```



This function returns a reference to the string that holds the name of the currently playing sound event. The returned value is not const, meaning it can be modified.




**Returns:**

A reference to the string holding the name of the current event


Get the name of the current event 

**Returns:**

A reference to a string containing the name of the current event 





        
Implements [*AGE::AudioEngine::GetCurrentEventName*](class_a_g_e_1_1_audio_engine.md#function-getcurrenteventname)


<hr>



### function Init 

```C++
virtual void AGE::AGESound::Init () override
```



Implements [*AGE::AudioEngine::Init*](class_a_g_e_1_1_audio_engine.md#function-init)


<hr>



### function IsEventValid 

_Checks whether the given event name is valid or not._ 
```C++
virtual bool AGE::AGESound::IsEventValid (
    const std::string & EventName
) override
```



This function takes an event name as input and checks if it's a valid event. The validity of the event can be based on various factors such as its length, format etc.




**Parameters:**


* `EventName` A string representing the name of the event to validate. 



**Returns:**

Returns true if the event is valid, false otherwise.


Checks whether the given event name is valid or not.


This function takes an event name as input and checks if it's a valid event by comparing it with a list of known events. If the event name matches any of these, the function returns true; otherwise, it returns false.




**Parameters:**


* `EventName` The name of the event to be checked. 



**Returns:**

True if the event is valid, False otherwise. 





        
Implements [*AGE::AudioEngine::IsEventValid*](class_a_g_e_1_1_audio_engine.md#function-iseventvalid)


<hr>



### function LoadBank 

_Loads a sound bank into the system._ 
```C++
virtual void AGE::AGESound::LoadBank (
    Ref< SoundBank > Bank
) override
```



This function takes in a reference to a [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object and loads it into the system. It does not return anything, so use void as the return type.




**Parameters:**


* `Bank` A reference to the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object that you want to load.

Loads a sound bank into the system.


This function takes in a reference to a [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object and loads it into the system for use by the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) class. The exact behavior of this function depends on its implementation, which is not provided here.




**Parameters:**


* `Bank` A reference to the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object to be loaded. 




        
Implements [*AGE::AudioEngine::LoadBank*](class_a_g_e_1_1_audio_engine.md#function-loadbank)


<hr>



### function LoadBanks 

_Loads a list of Sound Banks into the system._ 
```C++
virtual void AGE::AGESound::LoadBanks (
    const std::vector< Ref< SoundBank > > & Banks
) override
```



This function takes in a vector of references to Sound Bank objects and loads them into the sound system. The Sound Banks are expected to be properly initialized before being passed to this function.




**Parameters:**


* `Banks` A vector of references to Sound Bank objects.

Loads a collection of Sound Banks into the system.


This function takes in a vector of references to Sound Bank objects and loads them into the system. It does not return anything, so it is void.




**Parameters:**


* `Banks` - A constant reference to a vector of [**SoundBank**](class_a_g_e_1_1_sound_bank.md) references. Each [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object represents a bank of sounds that can be played by the system. 




        
Implements [*AGE::AudioEngine::LoadBanks*](class_a_g_e_1_1_audio_engine.md#function-loadbanks)


<hr>



### function LoadEvents 

```C++
inline virtual void AGE::AGESound::LoadEvents () override
```



Implements [*AGE::AudioEngine::LoadEvents*](class_a_g_e_1_1_audio_engine.md#function-loadevents)


<hr>



### function Play 

_Plays an audio source._ 
```C++
void AGE::AGESound::Play (
    const Ref< AudioSource > & Source
) 
```



This function plays the provided [**AudioSource**](class_a_g_e_1_1_audio_source.md) using OpenAL's alSourcePlay function.




**Parameters:**


* `Source` A reference to the [**AudioSource**](class_a_g_e_1_1_audio_source.md) that is to be played.

Plays an audio source.


This function plays the provided [**AudioSource**](class_a_g_e_1_1_audio_source.md) using OpenAL's alSourcePlay function. The function takes a reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object which is played by this method.




**Parameters:**


* `Source` A const reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object that needs to be played. 




        

<hr>



### function Set3DAttributes 

_Sets the 3D attributes for the sound object._ 
```C++
virtual void AGE::AGESound::Set3DAttributes (
    void * Attributes
) override
```



This function sets the 3D attributes of the sound object using a void pointer to the Attributes structure. The exact nature and format of this data is not specified, as it depends on the specific implementation of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) class.




**Parameters:**


* `Attributes` A void pointer to the Attributes structure.

Sets the 3D attributes for the sound object.


This function sets the 3D attributes of the sound object using a void pointer to the Attributes structure. The exact nature and format of this data is not specified in the documentation, so it's assumed to be opaque to Doxygen.




**Parameters:**


* `Attributes` A void pointer to the Attributes structure. This parameter is expected to contain specific 3D attributes for the sound object but its content is not defined by this function. 




        
Implements [*AGE::AudioEngine::Set3DAttributes*](class_a_g_e_1_1_audio_engine.md#function-set3dattributes)


<hr>



### function SetCurrentEventName 

_Set the name of the current event._ 
```C++
virtual void AGE::AGESound::SetCurrentEventName (
    const std::string & Name
) override
```





**Parameters:**


* `Name` The new name for the current event

Sets the name of the current event.


This function sets the name of the current event in the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object. The new name is passed as a const reference to avoid unnecessary copying.




**Parameters:**


* `Name` A constant reference to the string that will be used as the new name for the current event. 




        
Implements [*AGE::AudioEngine::SetCurrentEventName*](class_a_g_e_1_1_audio_engine.md#function-setcurrenteventname)


<hr>



### function SetParameterByName 

_This function sets a parameter by its name._ 
```C++
virtual void AGE::AGESound::SetParameterByName (
    const std::string & Name,
    float Value
) override
```



The function takes two parameters - the name of the parameter and the value to set it to. It does not return anything. If the provided name corresponds to an existing parameter, this function will update that parameter's value. Otherwise, it will do nothing.




**Parameters:**


* `Name` A string representing the name of the parameter to be set. 
* `Value` The new float value for the parameter.



**Returns:**

None


Set the parameter value by its name 

**Parameters:**


* `Name` The name of the parameter to set 
* `Value` The new value for the parameter 




        
Implements [*AGE::AudioEngine::SetParameterByName*](class_a_g_e_1_1_audio_engine.md#function-setparameterbyname)


<hr>



### function Shutdown 

_Shuts down the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._
```C++
virtual void AGE::AGESound::Shutdown () override
```



This function is used to clean up any resources that were allocated during the initialization of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object, such as memory or file handles. It prepares the object for deletion by setting it into a safe state and cleaning up any remaining resources.




**Returns:**

void


Shuts down the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object.


This function is used to clean up any resources that were allocated during the initialization of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object, such as memory or file handles. It prepares the object for deletion or reuse. 


        
Implements [*AGE::AudioEngine::Shutdown*](class_a_g_e_1_1_audio_engine.md#function-shutdown)


<hr>



### function Start 

_Starts the sound playback._ 
```C++
virtual void AGE::AGESound::Start () override
```



This function initiates the sound playback by setting up any necessary resources and starting the audio engine. It does not start the actual playing of the sound, that is done in the [**Play()**](class_a_g_e_1_1_a_g_e_sound.md#function-play) method.




**Returns:**

void


Starts the sound playback.


This function initiates the sound playback by starting to play the audio data from the beginning of the buffer. It does not reset or rewind the sound, it simply starts playing from where it left off.




**Returns:**

void 





        
Implements [*AGE::AudioEngine::Start*](class_a_g_e_1_1_audio_engine.md#function-start)


<hr>



### function Stop [1/3]

_Stops the sound from playing._ 
```C++
virtual void AGE::AGESound::Stop () override
```



This function is used to stop the sound that was previously started using the [**Play()**](class_a_g_e_1_1_a_g_e_sound.md#function-play) method. It will halt any ongoing playback and reset the position of the sound source back to its initial state.




**Returns:**

void


Stops the sound from playing.


This function is used to stop the sound that was previously started using the [**Play()**](class_a_g_e_1_1_a_g_e_sound.md#function-play) method. It should be called when you want to halt the playback of the sound.




**Returns:**

void 





        
Implements [*AGE::AudioEngine::Stop*](class_a_g_e_1_1_audio_engine.md#function-stop)


<hr>



### function Stop [2/3]

_Stops the audio source from playing._ 
```C++
void AGE::AGESound::Stop (
    const Ref< AudioSource > & Source
) 
```



This function stops an audio source from playing by using the OpenAL library's alSourceStop() function. The audio source to be stopped is passed as a reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object.




**Parameters:**


* `Source` A reference to the [**AudioSource**](class_a_g_e_1_1_audio_source.md) object whose source should be stopped.

Stops an audio source from playing.


This function stops the audio source specified by the handle provided. It does not check if the source is actually playing, so it should be used with caution.




**Parameters:**


* `Source` A reference to the [**AudioSource**](class_a_g_e_1_1_audio_source.md) object that you want to stop. 




        

<hr>



### function Stop [3/3]

_Stops all the audio sources in a given vector._ 
```C++
void AGE::AGESound::Stop (
    const std::vector< Ref< AudioSource > > & Sources
) 
```



This function iterates over each element of the provided vector and calls the [**Stop()**](class_a_g_e_1_1_a_g_e_sound.md#function-stop-13) function on it, effectively stopping any ongoing sound playback for each [**AudioSource**](class_a_g_e_1_1_audio_source.md) object.




**Parameters:**


* `Sources` A constant reference to a vector of Ref&lt;AudioSource&gt; objects representing the audio sources to be stopped. 



**Returns:**

void No return value is expected as all operations are performed in-place.


Stops all audio sources in the given vector.


This function iterates over each element of the provided vector and calls the [**Stop()**](class_a_g_e_1_1_a_g_e_sound.md#function-stop-13) function on it, effectively stopping any ongoing sound playback for that source.




**Parameters:**


* `Sources` A constant reference to a vector of [**AudioSource**](class_a_g_e_1_1_audio_source.md) references. Each element represents an individual audio source which will have its playback stopped. 




        

<hr>



### function Update 

_Updates the sound object._ 
```C++
virtual void AGE::AGESound::Update () override
```



This function is responsible for updating the sound object's state based on its current configuration and any changes in the game world. It does not return a value as it operates by side effects, modifying internal states of the sound object.




**Returns:**

None


Updates the sound object.


This function is responsible for updating the state of the sound object. It may involve processing audio data, updating sound properties or triggering any other necessary actions based on its current state.




**Returns:**

void 





        
Implements [*AGE::AudioEngine::Update*](class_a_g_e_1_1_audio_engine.md#function-update)


<hr>



### function ~AGESound 

_Destructor for_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _class._
```C++
AGE::AGESound::~AGESound () override
```



This function is responsible for releasing any resources that the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object may have acquired during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function LoadAudioSource 

_Loads an audio source from a file._ 
```C++
static AudioSource AGE::AGESound::LoadAudioSource (
    const std::string & FileName
) 
```



This function loads an audio source based on the format of the provided filename. It supports WAV and MP3 formats. If the format is not supported, it logs an error message and returns an invalid [**AudioSource**](class_a_g_e_1_1_audio_source.md) object.




**Parameters:**


* `FileName` The name of the file to load from. 



**Returns:**

An [**AudioSource**](class_a_g_e_1_1_audio_source.md) object representing the loaded audio data.


Loads an audio source from a file.


This function loads an audio source based on the format of the provided filename. It supports WAV and MP3 formats. If the format is not supported, it logs an error message and returns an invalid [**AudioSource**](class_a_g_e_1_1_audio_source.md) object.




**Parameters:**


* `FileName` The name of the file to load from. 



**Returns:**

An [**AudioSource**](class_a_g_e_1_1_audio_source.md) object representing the loaded audio data. 





        

<hr>



### function SetDebugLogging 

_Set the debug logging state for the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._
```C++
static void AGE::AGESound::SetDebugLogging (
    bool Log
) 
```



This function sets the debug logging state of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object. When debug logging is enabled, it will provide detailed information about its internal operations.




**Parameters:**


* [**Log**](class_a_g_e_1_1_log.md) A boolean value indicating whether to enable (true) or disable (false) debug logging. 



**Returns:**

void


Set the Debug Logging flag for the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object


This function sets a boolean value that determines whether debug logging is enabled or disabled.




**Parameters:**


* [**Log**](class_a_g_e_1_1_log.md) A boolean indicating if debug logging should be enabled (true) or disabled (false). 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AGESound/Public/AGEAudio.h`

