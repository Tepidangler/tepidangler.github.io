

# Class AGE::AudioSource



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AudioSource**](class_a_g_e_1_1_audio_source.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AudioSource**](#function-audiosource-15) (const std::string & FilePath) <br> |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br>_Gets the Asset ID of the object._  |
|  std::string | [**GetFilePath**](#function-getfilepath) () const<br>_This function returns the file path of the object._  |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetLengthMinutesAndSeconds**](#function-getlengthminutesandseconds) () const<br>_This function returns the total duration of the audio source in minutes and seconds._  |
|  std::string | [**GetName**](#function-getname) () const<br>_Returns the name of the object._  |
|  bool | [**IsLoaded**](#function-isloaded) () const<br>_Checks whether the object is loaded or not._  |
|  bool | [**IsLooping**](#function-islooping) () <br>_Checks whether the looping condition is set or not._  |
|  bool | [**IsPlaying**](#function-isplaying) () const<br>_Checks whether the game is currently playing or not._  |
|  void | [**SetAssetID**](#function-setassetid) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Sets the Asset ID of an object._  |
|  void | [**SetGain**](#function-setgain) (float Gain) <br>_Set the gain of the audio source._  |
|  void | [**SetLoop**](#function-setloop) (bool Loop) <br>_Sets the looping state of the audio source._  |
|  void | [**SetPitch**](#function-setpitch) (float Pitch) <br>_This function sets the pitch of an audio source._  |
|  void | [**SetPlaying**](#function-setplaying) (bool Playing) <br>_Sets the playing state of the object._  |
|  void | [**SetPosition**](#function-setposition-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & P) <br>_Sets the position of the audio source in 3D space._  |
|  void | [**SetPosition**](#function-setposition-22) (float x, float y, float z) <br>_Sets the position of the audio source in 3D space._  |
|  void | [**SetSoundData**](#function-setsounddata) (std::vector&lt; char &gt; Data) <br>_This function sets the sound data to a given vector of characters._  |
|  void | [**SetSpatial**](#function-setspatial) (bool Spatial) <br>_Sets the spatialization state of this audio source._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AudioSource**](class_a_g_e_1_1_audio_source.md) | [**LoadFromFile**](#function-loadfromfile) (const std::string & File, bool Spatial=false) <br>_Loads an audio source from a file and sets its spatial property._  |


























## Public Functions Documentation




### function AudioSource [1/5]

```C++
AGE::AudioSource::AudioSource (
    const std::string & FilePath
) 
```




<hr>



### function GetAssetID 

_Gets the Asset ID of the object._ 
```C++
inline UUID & AGE::AudioSource::GetAssetID () 
```



This function returns a reference to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) member variable 'm\_AssetID'. It is used to access and manipulate the unique identifier for an asset in the system.




**Returns:**

A reference to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) representing the Asset ID.


Gets the Asset ID of the object.


This function returns a reference to the private member variable 'm\_AssetID'. It provides access to this data, but does not allow modification.




**Returns:**

A reference to [**UUID**](class_a_g_e_1_1_u_u_i_d.md)& representing the Asset ID. 





        

<hr>



### function GetFilePath 

_This function returns the file path of the object._ 
```C++
inline std::string AGE::AudioSource::GetFilePath () const
```





**Returns:**

A string containing the file path.


This function returns the file path of a class instance. 

**Returns:**

A string containing the file path. If no file path is set, it will return an empty string. 





        

<hr>



### function GetLengthMinutesAndSeconds 

_This function returns the total duration of the audio source in minutes and seconds._ 
```C++
std::pair< uint32_t, uint32_t > AGE::AudioSource::GetLengthMinutesAndSeconds () const
```





**Returns:**

A pair where the first element is the number of minutes, and the second element is the number of seconds.


This function returns the total duration of the audio source in minutes and seconds. 

**Returns:**

A pair of unsigned 32-bit integers representing the length of the audio in minutes and seconds respectively. 





        

<hr>



### function GetName 

_Returns the name of the object._ 
```C++
inline std::string AGE::AudioSource::GetName () const
```





**Returns:**

A string containing the name of the object. If no name is set, returns an empty string.


Returns the name of the object. 

**Returns:**

A string containing the name of the object. If no name is set, an empty string will be returned. 





        

<hr>



### function IsLoaded 

_Checks whether the object is loaded or not._ 
```C++
inline bool AGE::AudioSource::IsLoaded () const
```



This function returns a boolean value indicating whether the object is loaded or not. It does this by returning the 'bLoaded' member variable of the class instance.




**Returns:**

True if the object is loaded, false otherwise.


Checks whether the object is loaded.


This function returns a boolean value indicating whether the object has been loaded or not.




**Returns:**

True if the object is loaded, false otherwise. 





        

<hr>



### function IsLooping 

_Checks whether the looping condition is set or not._ 
```C++
inline bool AGE::AudioSource::IsLooping () 
```



This function returns a boolean value indicating whether the 'bLoop' variable, which represents the looping condition in the code, has been set to true or false.




**Returns:**

True if the looping condition is set (i.e., bLoop == true), False otherwise.


Checks whether the looping condition is set.


This function returns a boolean value indicating whether the 'bLoop' variable, which represents the looping condition in the code, has been set or not.




**Returns:**

True if the looping condition is set (i.e., bLoop is true), false otherwise. 





        

<hr>



### function IsPlaying 

_Checks whether the game is currently playing or not._ 
```C++
inline bool AGE::AudioSource::IsPlaying () const
```



This function returns a boolean value indicating if the game is in play mode. It does this by examining the 'bIsPlaying' member variable of the class instance.




**Returns:**

True if the game is currently being played, false otherwise.


This function checks whether the game is currently playing. 

**Returns:**

Returns true if the game is currently playing, false otherwise. 





        

<hr>



### function SetAssetID 

_Sets the Asset ID of an object._ 
```C++
inline void AGE::AudioSource::SetAssetID (
    const UUID & ID
) 
```





**Parameters:**


* `ID` The unique identifier for the asset. 



**Returns:**

void


Sets the Asset ID of an object. 

**Parameters:**


* `ID` The unique identifier for the asset. 




        

<hr>



### function SetGain 

_Set the gain of the audio source._ 
```C++
void AGE::AudioSource::SetGain (
    float Gain
) 
```



This function sets the gain value for the audio source represented by m\_SourceHandle. The gain is a float value that represents the volume level of the audio source. It also updates the OpenAL source with the new Gain value using alSourcef().




**Parameters:**


* `Gain` A float representing the desired gain level. Must be between 0.0 and 1.0.

This function sets the gain of an audio source.


The function takes a float parameter representing the desired gain level for the audio source. It then updates the member variable m\_Gain with this value and applies it to the OpenAL source handle using alSourcef().




**Parameters:**


* `Gain` A floating-point number representing the desired gain level (0.0 - 1.0). 




        

<hr>



### function SetLoop 

_Sets the looping state of the audio source._ 
```C++
void AGE::AudioSource::SetLoop (
    bool Loop
) 
```



This function sets the looping state of the audio source by modifying the 'bLoop' member variable and the OpenAL source handle. If Loop is true, the AL\_LOOPING parameter will be set to AL\_TRUE indicating that the audio should continue playing indefinitely when it reaches the end. If Loop is false, the AL\_LOOPING parameter will be set to AL\_FALSE signifying that the audio should stop playing once it has reached the end.




**Parameters:**


* `Loop` A boolean value indicating whether or not the source should loop.

Sets the looping state of the audio source.


This function sets the looping state of the audio source by modifying the OpenAL source parameter for looping. If Loop is true, the source will play in a loop until explicitly stopped or the end of the sound data is reached. If Loop is false, the source will stop playing when the end of the sound data is reached.




**Parameters:**


* `Loop` The new state for looping (true = loop, false = no loop). 




        

<hr>



### function SetPitch 

_This function sets the pitch of an audio source._ 
```C++
void AGE::AudioSource::SetPitch (
    float Pitch
) 
```



The function takes a float value as input and assigns it to the member variable m\_Pitch. It then uses this value to set the 'AL\_PITCH' property of the OpenAL source represented by m\_SourceHandle. This change in pitch will affect how the audio is played back, affecting its speed or tempo.




**Parameters:**


* `Pitch` The new pitch value for the audio source.

Set the pitch of the audio source.


This function sets the pitch of the audio source by adjusting its pitch factor in the OpenAL context. The pitch is a value that affects the speed at which the sound wave repeats, affecting both frequency and duration. A higher pitch will result in faster playback for sounds with a lower fundamental frequency (like musical notes). Conversely, a lower pitch will slow down the playback of high-frequency sounds. The function takes as input a float value representing the new pitch to be set.




**Parameters:**


* `Pitch` The new pitch value to be set. Must be greater than or equal to 0.0 for no change in pitch. 




        

<hr>



### function SetPlaying 

_Sets the playing state of the object._ 
```C++
inline void AGE::AudioSource::SetPlaying (
    bool Playing
) 
```





**Parameters:**


* `Playing` The new playing state to set.

Sets the playing state of the object. 

**Parameters:**


* `Playing` The new playing state to set. 




        

<hr>



### function SetPosition [1/2]

_Sets the position of the audio source in 3D space._ 
```C++
void AGE::AudioSource::SetPosition (
    const Vector3 & P
) 
```



This function sets the position of the audio source to a specified [**Vector3**](struct_a_g_e_1_1_vector3.md) value P. The actual OpenAL call is made within this function, setting the position of the audio source represented by m\_SourceHandle using the alSourcefv function with AL\_POSITION as the parameter and &m\_Position.x as the argument.




**Parameters:**


* `P` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the new position for the audio source.

Sets the position of the audio source in 3D space.


This function sets the position of the audio source to a specified [**Vector3**](struct_a_g_e_1_1_vector3.md) value P. The actual OpenAL call is made within this function, setting the position of the source using alSourcefv with AL\_POSITION as the parameter and &m\_Position.x as the argument. 

**Parameters:**


* `P` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the new position for the audio source. 




        

<hr>



### function SetPosition [2/2]

_Sets the position of the audio source in 3D space._ 
```C++
void AGE::AudioSource::SetPosition (
    float x,
    float y,
    float z
) 
```



This function sets the position of the audio source using three floating-point values (x, y, z). The new position is then applied to the OpenAL source handle associated with this [**AudioSource**](class_a_g_e_1_1_audio_source.md) instance.




**Parameters:**


* `x` The x coordinate of the new position. 
* `y` The y coordinate of the new position. 
* `z` The z coordinate of the new position.

Sets the position of the audio source in a 3D space.


This function sets the position of the audio source by updating its internal position vector and then applying this change to the OpenAL source represented by m\_SourceHandle.




**Parameters:**


* `x` The new X coordinate for the position. 
* `y` The new Y coordinate for the position. 
* `z` The new Z coordinate for the position. 




        

<hr>



### function SetSoundData 

_This function sets the sound data to a given vector of characters._ 
```C++
inline void AGE::AudioSource::SetSoundData (
    std::vector< char > Data
) 
```





**Parameters:**


* `Data` The new sound data as a std::vector of characters.

This function sets the sound data to a given vector of characters. 

**Parameters:**


* `Data` The new sound data as a std::vector of characters. 




        

<hr>



### function SetSpatial 

_Sets the spatialization state of this audio source._ 
```C++
void AGE::AudioSource::SetSpatial (
    bool Spatial
) 
```



This function sets the spatialization state of the audio source, enabling or disabling spatialization based on the input parameter. It also sets the distance model to AL\_INVERSE\_DISTANCE\_CLAMPED for proper spatialization behavior.




**Parameters:**


* `Spatial` The new spatialization state. If true, spatialization is enabled; if false, it's disabled.

Sets the spatialization state of this audio source.


This function sets the `bSpatial` member variable to the provided value and then updates the OpenAL source with the new setting for spatialization. If Spatial is true, it enables spatialization; if false, it disables spatialization.




**Parameters:**


* `Spatial` The new state of spatialization. 




        

<hr>
## Public Static Functions Documentation




### function LoadFromFile 

_Loads an audio source from a file and sets its spatial property._ 
```C++
static AudioSource AGE::AudioSource::LoadFromFile (
    const std::string & File,
    bool Spatial=false
) 
```



This function loads an audio source from the specified file path using [**AGESound::LoadAudioSource()**](class_a_g_e_1_1_a_g_e_sound.md#function-loadaudiosource). It then sets the spatial property of the loaded audio source to the provided value. The file path is also stored in the resultant [**AudioSource**](class_a_g_e_1_1_audio_source.md) object for future reference.




**Parameters:**


* `File` A string representing the file path of the audio file to load. 
* `Spatial` A boolean indicating whether or not the audio should be spatialized.



**Returns:**

An [**AudioSource**](class_a_g_e_1_1_audio_source.md) object loaded from the specified file and with its spatial property set according to the provided value.


Loads an audio source from a file and sets its spatial property.


This function loads an audio source from the specified file path using [**AGESound**](class_a_g_e_1_1_a_g_e_sound.md)'s `LoadAudioSource` method, then it sets the spatial property of the loaded audio source to the provided value. The file path is also stored in the resultant [**AudioSource**](class_a_g_e_1_1_audio_source.md) object for future reference.




**Parameters:**


* `File` A string representing the file path from which to load the audio source. 
* `Spatial` A boolean indicating whether or not the loaded audio source should be spatialized.



**Returns:**

An instance of `AudioSource` containing the loaded audio data and its properties set as per the provided parameters. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AGESound/Public/Sound.h`

