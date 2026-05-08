

# Class AGE::AudioSource



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AudioSource**](class_a_g_e_1_1_audio_source.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AudioSource**](#function-audiosource-15) (const std::string & FilePath) <br> |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br> |
|  std::string | [**GetFilePath**](#function-getfilepath) () const<br> |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetLengthMinutesAndSeconds**](#function-getlengthminutesandseconds) () const<br> |
|  std::string | [**GetName**](#function-getname) () const<br> |
|  bool | [**IsLoaded**](#function-isloaded) () const<br> |
|  bool | [**IsLooping**](#function-islooping) () <br> |
|  bool | [**IsPlaying**](#function-isplaying) () const<br> |
|  void | [**SetAssetID**](#function-setassetid) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  void | [**SetGain**](#function-setgain) (float Gain) <br> |
|  void | [**SetLoop**](#function-setloop) (bool Loop) <br> |
|  void | [**SetPitch**](#function-setpitch) (float Pitch) <br> |
|  void | [**SetPlaying**](#function-setplaying) (bool Playing) <br> |
|  void | [**SetPosition**](#function-setposition-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & P) <br> |
|  void | [**SetPosition**](#function-setposition-22) (float x, float y, float z) <br> |
|  void | [**SetSoundData**](#function-setsounddata) (std::vector&lt; char &gt; Data) <br> |
|  void | [**SetSpatial**](#function-setspatial) (bool Spatial) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AudioSource**](class_a_g_e_1_1_audio_source.md) | [**LoadFromFile**](#function-loadfromfile) (const std::string & File, bool Spatial=false) <br> |


























## Public Functions Documentation




### function AudioSource [1/5]

```C++
AGE::AudioSource::AudioSource (
    const std::string & FilePath
) 
```




<hr>



### function GetAssetID 

```C++
inline UUID & AGE::AudioSource::GetAssetID () 
```




<hr>



### function GetFilePath 

```C++
inline std::string AGE::AudioSource::GetFilePath () const
```




<hr>



### function GetLengthMinutesAndSeconds 

```C++
std::pair< uint32_t, uint32_t > AGE::AudioSource::GetLengthMinutesAndSeconds () const
```




<hr>



### function GetName 

```C++
inline std::string AGE::AudioSource::GetName () const
```




<hr>



### function IsLoaded 

```C++
inline bool AGE::AudioSource::IsLoaded () const
```




<hr>



### function IsLooping 

```C++
inline bool AGE::AudioSource::IsLooping () 
```




<hr>



### function IsPlaying 

```C++
inline bool AGE::AudioSource::IsPlaying () const
```




<hr>



### function SetAssetID 

```C++
inline void AGE::AudioSource::SetAssetID (
    const UUID & ID
) 
```




<hr>



### function SetGain 

```C++
void AGE::AudioSource::SetGain (
    float Gain
) 
```




<hr>



### function SetLoop 

```C++
void AGE::AudioSource::SetLoop (
    bool Loop
) 
```




<hr>



### function SetPitch 

```C++
void AGE::AudioSource::SetPitch (
    float Pitch
) 
```




<hr>



### function SetPlaying 

```C++
inline void AGE::AudioSource::SetPlaying (
    bool Playing
) 
```




<hr>



### function SetPosition [1/2]

```C++
void AGE::AudioSource::SetPosition (
    const Vector3 & P
) 
```




<hr>



### function SetPosition [2/2]

```C++
void AGE::AudioSource::SetPosition (
    float x,
    float y,
    float z
) 
```




<hr>



### function SetSoundData 

```C++
inline void AGE::AudioSource::SetSoundData (
    std::vector< char > Data
) 
```




<hr>



### function SetSpatial 

```C++
void AGE::AudioSource::SetSpatial (
    bool Spatial
) 
```




<hr>
## Public Static Functions Documentation




### function LoadFromFile 

```C++
static AudioSource AGE::AudioSource::LoadFromFile (
    const std::string & File,
    bool Spatial=false
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AGESound/Public/Sound.h`

