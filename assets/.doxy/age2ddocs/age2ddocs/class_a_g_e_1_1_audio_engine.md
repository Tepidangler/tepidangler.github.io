

# Class AGE::AudioEngine



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AudioEngine**](class_a_g_e_1_1_audio_engine.md)










Inherited by the following classes: [AGE::AGESound](class_a_g_e_1_1_a_g_e_sound.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br>_This function is a placeholder and will always fail an assertion. It's used as a stub for future development._  |
|  [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) \* | [**As**](#function-as-22) () <br>_This function returns a pointer to the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._ |
| virtual std::string & | [**GetCurrentEventName**](#function-getcurrenteventname) () = 0<br> |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual bool | [**IsEventValid**](#function-iseventvalid) (const std::string & EventName) = 0<br> |
| virtual void | [**LoadBank**](#function-loadbank) (Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; Bank) = 0<br> |
| virtual void | [**LoadBanks**](#function-loadbanks) (const std::vector&lt; Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & Banks) = 0<br> |
| virtual void | [**LoadEvents**](#function-loadevents) () = 0<br> |
| virtual void | [**Set3DAttributes**](#function-set3dattributes) (void \* Attributes) = 0<br> |
| virtual void | [**SetCurrentEventName**](#function-setcurrenteventname) (const std::string & Name) = 0<br> |
| virtual void | [**SetParameterByName**](#function-setparameterbyname) (const std::string & Name, float Value) = 0<br> |
| virtual void | [**Shutdown**](#function-shutdown) () = 0<br> |
| virtual void | [**Start**](#function-start) () = 0<br> |
| virtual void | [**Stop**](#function-stop) () = 0<br> |
| virtual void | [**Update**](#function-update) () = 0<br> |
| virtual  | [**~AudioEngine**](#function-audioengine) () = default<br>_Virtual destructor for the_ [_**AudioEngine**_](class_a_g_e_1_1_audio_engine.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; | [**Create**](#function-create) (AudioEngineType Type) <br> |


























## Public Functions Documentation




### function As [1/2]

_This function is a placeholder and will always fail an assertion. It's used as a stub for future development._ 
```C++
template<typename T>
T * AGE::AudioEngine::As () 
```





**Returns:**

Unknown


This function is a placeholder and should not be called directly. It always asserts false with an error message indicating that the [**As()**](class_a_g_e_1_1_audio_engine.md#function-as-12) function has failed. 

**Returns:**

Unknown 





        

<hr>



### function As [2/2]

_This function returns a pointer to the_ [_**AGESound**_](class_a_g_e_1_1_a_g_e_sound.md) _object._
```C++
template<>
AGESound * AGE::AudioEngine::As () 
```



The function is used to obtain an instance of [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) that can be cast back into its original class type using dynamic\_cast. It does this by returning 'this' as a pointer to [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md), which allows it to be treated as if it were an instance of the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) class.




**Returns:**

A pointer to the [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object.


This function returns a pointer to [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object casted from the current instance of [**AudioEngine**](class_a_g_e_1_1_audio_engine.md). 

**Returns:**

A pointer to an [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) object, or nullptr if this is not an [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md) instance. 





        

<hr>



### function GetCurrentEventName 

```C++
virtual std::string & AGE::AudioEngine::GetCurrentEventName () = 0
```




<hr>



### function Init 

```C++
virtual void AGE::AudioEngine::Init () = 0
```




<hr>



### function IsEventValid 

```C++
virtual bool AGE::AudioEngine::IsEventValid (
    const std::string & EventName
) = 0
```




<hr>



### function LoadBank 

```C++
virtual void AGE::AudioEngine::LoadBank (
    Ref< SoundBank > Bank
) = 0
```




<hr>



### function LoadBanks 

```C++
virtual void AGE::AudioEngine::LoadBanks (
    const std::vector< Ref< SoundBank > > & Banks
) = 0
```




<hr>



### function LoadEvents 

```C++
virtual void AGE::AudioEngine::LoadEvents () = 0
```




<hr>



### function Set3DAttributes 

```C++
virtual void AGE::AudioEngine::Set3DAttributes (
    void * Attributes
) = 0
```




<hr>



### function SetCurrentEventName 

```C++
virtual void AGE::AudioEngine::SetCurrentEventName (
    const std::string & Name
) = 0
```




<hr>



### function SetParameterByName 

```C++
virtual void AGE::AudioEngine::SetParameterByName (
    const std::string & Name,
    float Value
) = 0
```




<hr>



### function Shutdown 

```C++
virtual void AGE::AudioEngine::Shutdown () = 0
```




<hr>



### function Start 

```C++
virtual void AGE::AudioEngine::Start () = 0
```




<hr>



### function Stop 

```C++
virtual void AGE::AudioEngine::Stop () = 0
```




<hr>



### function Update 

```C++
virtual void AGE::AudioEngine::Update () = 0
```




<hr>



### function ~AudioEngine 

_Virtual destructor for the_ [_**AudioEngine**_](class_a_g_e_1_1_audio_engine.md) _class._
```C++
virtual AGE::AudioEngine::~AudioEngine () = default
```



This function is responsible for releasing any resources that were acquired by the [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) instance, such as memory or file handles. It does not return anything (void) and thus it doesn't need a Doxygen comment to specify its return type. 


        

<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< AudioEngine > AGE::AudioEngine::Create (
    AudioEngineType Type
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AudioEngine/Public/AudioEngine.h`

