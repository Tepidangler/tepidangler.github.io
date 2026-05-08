

# Class AGE::AGESound



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md)








Inherits the following classes: [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGESound**](#function-agesound) () <br> |
| virtual std::string & | [**GetCurrentEventName**](#function-getcurrenteventname) () override<br> |
| virtual void | [**Init**](#function-init) () override<br> |
| virtual bool | [**IsEventValid**](#function-iseventvalid) (const std::string & EventName) override<br> |
| virtual void | [**LoadBank**](#function-loadbank) (Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; Bank) override<br> |
| virtual void | [**LoadBanks**](#function-loadbanks) (const std::vector&lt; Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & Banks) override<br> |
| virtual void | [**LoadEvents**](#function-loadevents) () override<br> |
|  void | [**Play**](#function-play) (const Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & Source) <br> |
| virtual void | [**Set3DAttributes**](#function-set3dattributes) (void \* Attributes) override<br> |
| virtual void | [**SetCurrentEventName**](#function-setcurrenteventname) (const std::string & Name) override<br> |
| virtual void | [**SetParameterByName**](#function-setparameterbyname) (const std::string & Name, float Value) override<br> |
| virtual void | [**Shutdown**](#function-shutdown) () override<br> |
| virtual void | [**Start**](#function-start) () override<br> |
| virtual void | [**Stop**](#function-stop-13) () override<br> |
|  void | [**Stop**](#function-stop-23) (const Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & Source) <br> |
|  void | [**Stop**](#function-stop-33) (const std::vector&lt; Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; & Sources) <br> |
| virtual void | [**Update**](#function-update) () override<br> |
|   | [**~AGESound**](#function-agesound) () override<br> |


## Public Functions inherited from AGE::AudioEngine

See [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_audio_engine.md#function-as-12) () <br> |
|  [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) \* | [**As**](class_a_g_e_1_1_audio_engine.md#function-as-22) () <br> |
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
| virtual  | [**~AudioEngine**](class_a_g_e_1_1_audio_engine.md#function-audioengine) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AudioSource**](class_a_g_e_1_1_audio_source.md) | [**LoadAudioSource**](#function-loadaudiosource) (const std::string & FileName) <br> |
|  void | [**SetDebugLogging**](#function-setdebuglogging) (bool Log) <br> |


## Public Static Functions inherited from AGE::AudioEngine

See [AGE::AudioEngine](class_a_g_e_1_1_audio_engine.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; | [**Create**](class_a_g_e_1_1_audio_engine.md#function-create) (AudioEngineType Type) <br> |


















































## Public Functions Documentation




### function AGESound 

```C++
AGE::AGESound::AGESound () 
```




<hr>



### function GetCurrentEventName 

```C++
virtual std::string & AGE::AGESound::GetCurrentEventName () override
```



Implements [*AGE::AudioEngine::GetCurrentEventName*](class_a_g_e_1_1_audio_engine.md#function-getcurrenteventname)


<hr>



### function Init 

```C++
virtual void AGE::AGESound::Init () override
```



Implements [*AGE::AudioEngine::Init*](class_a_g_e_1_1_audio_engine.md#function-init)


<hr>



### function IsEventValid 

```C++
virtual bool AGE::AGESound::IsEventValid (
    const std::string & EventName
) override
```



Implements [*AGE::AudioEngine::IsEventValid*](class_a_g_e_1_1_audio_engine.md#function-iseventvalid)


<hr>



### function LoadBank 

```C++
virtual void AGE::AGESound::LoadBank (
    Ref< SoundBank > Bank
) override
```



Implements [*AGE::AudioEngine::LoadBank*](class_a_g_e_1_1_audio_engine.md#function-loadbank)


<hr>



### function LoadBanks 

```C++
virtual void AGE::AGESound::LoadBanks (
    const std::vector< Ref< SoundBank > > & Banks
) override
```



Implements [*AGE::AudioEngine::LoadBanks*](class_a_g_e_1_1_audio_engine.md#function-loadbanks)


<hr>



### function LoadEvents 

```C++
inline virtual void AGE::AGESound::LoadEvents () override
```



Implements [*AGE::AudioEngine::LoadEvents*](class_a_g_e_1_1_audio_engine.md#function-loadevents)


<hr>



### function Play 

```C++
void AGE::AGESound::Play (
    const Ref< AudioSource > & Source
) 
```




<hr>



### function Set3DAttributes 

```C++
virtual void AGE::AGESound::Set3DAttributes (
    void * Attributes
) override
```



Implements [*AGE::AudioEngine::Set3DAttributes*](class_a_g_e_1_1_audio_engine.md#function-set3dattributes)


<hr>



### function SetCurrentEventName 

```C++
virtual void AGE::AGESound::SetCurrentEventName (
    const std::string & Name
) override
```



Implements [*AGE::AudioEngine::SetCurrentEventName*](class_a_g_e_1_1_audio_engine.md#function-setcurrenteventname)


<hr>



### function SetParameterByName 

```C++
virtual void AGE::AGESound::SetParameterByName (
    const std::string & Name,
    float Value
) override
```



Implements [*AGE::AudioEngine::SetParameterByName*](class_a_g_e_1_1_audio_engine.md#function-setparameterbyname)


<hr>



### function Shutdown 

```C++
virtual void AGE::AGESound::Shutdown () override
```



Implements [*AGE::AudioEngine::Shutdown*](class_a_g_e_1_1_audio_engine.md#function-shutdown)


<hr>



### function Start 

```C++
virtual void AGE::AGESound::Start () override
```



Implements [*AGE::AudioEngine::Start*](class_a_g_e_1_1_audio_engine.md#function-start)


<hr>



### function Stop [1/3]

```C++
virtual void AGE::AGESound::Stop () override
```



Implements [*AGE::AudioEngine::Stop*](class_a_g_e_1_1_audio_engine.md#function-stop)


<hr>



### function Stop [2/3]

```C++
void AGE::AGESound::Stop (
    const Ref< AudioSource > & Source
) 
```




<hr>



### function Stop [3/3]

```C++
void AGE::AGESound::Stop (
    const std::vector< Ref< AudioSource > > & Sources
) 
```




<hr>



### function Update 

```C++
virtual void AGE::AGESound::Update () override
```



Implements [*AGE::AudioEngine::Update*](class_a_g_e_1_1_audio_engine.md#function-update)


<hr>



### function ~AGESound 

```C++
AGE::AGESound::~AGESound () override
```




<hr>
## Public Static Functions Documentation




### function LoadAudioSource 

```C++
static AudioSource AGE::AGESound::LoadAudioSource (
    const std::string & FileName
) 
```




<hr>



### function SetDebugLogging 

```C++
static void AGE::AGESound::SetDebugLogging (
    bool Log
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AGESound/Public/AGEAudio.h`

