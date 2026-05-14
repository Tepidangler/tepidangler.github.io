

# Struct AGE::AudioComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AudioComponent**](struct_a_g_e_1_1_audio_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; | [**Audio**](#variable-audio)  <br> |
|  uint64\_t | [**GameObjID**](#variable-gameobjid)  <br> |
|  uint32\_t | [**SoundBankID**](#variable-soundbankid)  <br> |
|  std::vector&lt; Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; | [**Sounds**](#variable-sounds)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**AddSound**](#function-addsound) (Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; Sound) <br>_This function adds a sound to the Sounds vector._  |
|   | [**AudioComponent**](#function-audiocomponent-12) (const Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; & Engine) <br>_Constructs an instance of_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _with a reference to the audio engine._ |
|   | [**AudioComponent**](#function-audiocomponent-22) (const [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) &) = default<br>_Default copy constructor for the_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _class._ |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; & | [**GetAudioEngine**](#function-getaudioengine) () <br>_Returns a reference to the global instance of the_ [_**AudioEngine**_](class_a_g_e_1_1_audio_engine.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) & Data) <br>_This function deserializes data from a serialized format into an_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) & Data) <br>_This function serializes an instance of the_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _class into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


























## Public Attributes Documentation




### variable Audio 

```C++
Ref<AudioEngine> AGE::AudioComponent::Audio;
```




<hr>



### variable GameObjID 

```C++
uint64_t AGE::AudioComponent::GameObjID;
```




<hr>



### variable SoundBankID 

```C++
uint32_t AGE::AudioComponent::SoundBankID;
```




<hr>



### variable Sounds 

```C++
std::vector<Ref<AudioSource> > AGE::AudioComponent::Sounds;
```




<hr>
## Public Functions Documentation




### function AddSound 

_This function adds a sound to the Sounds vector._ 
```C++
inline void AGE::AudioComponent::AddSound (
    Ref< AudioSource > Sound
) 
```





**Parameters:**


* `Sound` A reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object which represents the sound to be added. 



**Returns:**

void 





        

<hr>



### function AudioComponent [1/2]

_Constructs an instance of_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _with a reference to the audio engine._
```C++
inline AGE::AudioComponent::AudioComponent (
    const Ref< AudioEngine > & Engine
) 
```





**Parameters:**


* `Engine` A reference to the audio engine. 




        

<hr>



### function AudioComponent [2/2]

_Default copy constructor for the_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _class._
```C++
AGE::AudioComponent::AudioComponent (
    const AudioComponent &
) = default
```



This function is used to create a new instance of an [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) by copying data from another existing instance. It uses the '= default' syntax in C++, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The existing [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) instance to copy data from. 




        

<hr>



### function GetAudioEngine 

_Returns a reference to the global instance of the_ [_**AudioEngine**_](class_a_g_e_1_1_audio_engine.md) _class._
```C++
inline Ref< AudioEngine > & AGE::AudioComponent::GetAudioEngine () 
```





**Returns:**

Reference to the global [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) object. 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes data from a serialized format into an_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _object._
```C++
static inline void AGE::AudioComponent::Deserialize (
    DataReader * Serializer,
    AudioComponent & Data
) 
```



The function takes in two parameters - a pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and a reference to an [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) object. It does not return anything, but it modifies the [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) object by filling its fields with data read from the [**DataReader**](class_a_g_e_1_1_data_reader.md) object.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains serialized data. 
* `Data` A reference to an [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) object which will be filled with deserialized data. 




        

<hr>



### function Serialize 

_This function serializes an instance of the_ [_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _class into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::AudioComponent::Serialize (
    DataWriter * Serializer,
    const AudioComponent & Data
) 
```



The function takes two parameters: a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object and a constant reference to an [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) object. It does not return anything, so void is used as the return type.




**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be serializing the data. 
* `Data` The constant reference to an [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) object that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

