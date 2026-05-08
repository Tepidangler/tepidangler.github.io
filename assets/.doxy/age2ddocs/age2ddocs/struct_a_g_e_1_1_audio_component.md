

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
|  void | [**AddSound**](#function-addsound) (Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; Sound) <br> |
|   | [**AudioComponent**](#function-audiocomponent-12) (const Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; & Engine) <br> |
|   | [**AudioComponent**](#function-audiocomponent-22) (const [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) &) = default<br> |
|  Ref&lt; [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) &gt; & | [**GetAudioEngine**](#function-getaudioengine) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AudioComponent**](struct_a_g_e_1_1_audio_component.md) & Data) <br> |


























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

```C++
inline void AGE::AudioComponent::AddSound (
    Ref< AudioSource > Sound
) 
```




<hr>



### function AudioComponent [1/2]

```C++
inline AGE::AudioComponent::AudioComponent (
    const Ref< AudioEngine > & Engine
) 
```




<hr>



### function AudioComponent [2/2]

```C++
AGE::AudioComponent::AudioComponent (
    const AudioComponent &
) = default
```




<hr>



### function GetAudioEngine 

```C++
inline Ref< AudioEngine > & AGE::AudioComponent::GetAudioEngine () 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::AudioComponent::Deserialize (
    DataReader * Serializer,
    AudioComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::AudioComponent::Serialize (
    DataWriter * Serializer,
    const AudioComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

