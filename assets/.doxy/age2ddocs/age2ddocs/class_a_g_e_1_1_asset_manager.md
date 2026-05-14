

# Class AGE::AssetManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AssetManager**](class_a_g_e_1_1_asset_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AssetManager**](#function-assetmanager-13) () = default<br>_Default constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class._ |
|   | [**AssetManager**](#function-assetmanager-23) (const std::filesystem::path & GameContentPath) <br>_Constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class. Initializes the game content path and creates an instance of the_[_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _._ |
|   | [**AssetManager**](#function-assetmanager-33) (void \* AddrToPakFile, size\_t SizeOfPakFile=0) <br>_Constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class._ |
|  bool | [**DoesShaderExist**](#function-doesshaderexist) (const std::string & Name) <br>_Checks if a shader with the given name exists._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAsepriteTexture**](#function-getasepritetexture-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves a texture from the registry using its unique identifier._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAsepriteTexture**](#function-getasepritetexture-22) (const std::string & Name) <br>_Retrieves a texture from the asset registry using an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file name._ |
|  Ref&lt; [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &gt; | [**GetAssetRegistry**](#function-getassetregistry) () const<br>_Retrieves the Asset Registry object associated with this instance._  |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves a font from the asset manager._  |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-22) (const std::string & Name) <br>_Get a font from the asset manager._  |
|  std::filesystem::path & | [**GetGameContentPath**](#function-getgamecontentpath) () <br>_Returns the game content path._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves a scene from the registry using its unique identifier._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-22) (const std::string & Name) <br>_Retrieves a scene with the given name._  |
|  void | [**GetSceneNames**](#function-getscenenames) (std::vector&lt; std::string &gt; & OutArray) <br>_This function retrieves the names of all scenes in the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._ |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**GetShader**](#function-getshader) (const std::string & Name) <br>_Get a shader from the registry by name._  |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves an audio source with a specific_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._ |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-22) (const std::string & Name) <br>_Retrieves an audio source with the given name._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-12) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Retrieves a texture from the asset manager._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-22) (const std::string & Name) <br>_Much slower option considering I had to implement the find function for this myself, however in the event that you don't know the ID for the particular texture you want to load you can search for it based on the name which == the filename._  |
|  bool | [**IsAsepriteFileLoaded**](#function-isasepritefileloaded) (const std::filesystem::path & Filepath) <br>_Checks if an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file is loaded._ |
|  bool | [**IsFontLoaded**](#function-isfontloaded) (const std::filesystem::path & Filepath) <br>_Checks if a font is loaded._  |
|  bool | [**IsSceneLoaded**](#function-issceneloaded) (const std::filesystem::path & Filepath) <br>_Checks if a scene is loaded._  |
|  bool | [**IsSoundLoaded**](#function-issoundloaded) (const std::filesystem::path & Filepath) <br>_Checks if a sound is loaded._  |
|  bool | [**IsSoundbankLoaded**](#function-issoundbankloaded) (const std::filesystem::path & Filepath) <br>_Checks if a soundbank is loaded._  |
|  bool | [**IsTextureLoaded**](#function-istextureloaded) (const std::filesystem::path & Filepath) <br>_Checks if a texture is loaded._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadAsepriteFile**](#function-loadasepritefile) (const std::filesystem::path & Filepath) <br>_Loads an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file from the specified path._ |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**LoadFont**](#function-loadfont) (const std::filesystem::path & Filepath) <br>_Loads a font from the specified file path._  |
|  bool | [**LoadPakFile**](#function-loadpakfile) (void \* AddrToPakFile, size\_t SizeOfPakFile=0) <br>_Loads a PAK file into the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._ |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Filepath) <br>_Loads a scene from the given file path._  |
|  void | [**LoadShader**](#function-loadshader-13) (const std::string & FilePath) <br>_Loads a shader from the specified file path._  |
|  void | [**LoadShader**](#function-loadshader-23) (const std::string & FilePath1, const std::string & FilePath2) <br>_Loads a shader from two file paths._  |
|  void | [**LoadShader**](#function-loadshader-33) (const int Name, const std::string & Source) <br>_Loads a shader into the asset manager._  |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**LoadSound**](#function-loadsound) (const std::filesystem::path & Filepath) <br>_Loads a sound from the specified file path._  |
|  void | [**LoadSoundbank**](#function-loadsoundbank) (const std::filesystem::path & Filepath) <br>_Loads a soundbank from the specified file path._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture-12) (const std::filesystem::path & FilePath) <br>_Loads a texture from the specified file path._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture-22) (void \* Addr, size\_t Size) <br>_Loads a texture from binary data._  |
|  void | [**RegisterAsset**](#function-registerasset) (Ref&lt; T &gt; Asset) <br>_Registers an asset of type T into the system._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AssetManager**](class_a_g_e_1_1_asset_manager.md) & | [**Get**](#function-get) () <br>_Returns a reference to the global instance of_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._ |


























## Public Functions Documentation




### function AssetManager [1/3]

_Default constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class._
```C++
AGE::AssetManager::AssetManager () = default
```




<hr>



### function AssetManager [2/3]

_Constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class. Initializes the game content path and creates an instance of the_[_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _._
```C++
AGE::AssetManager::AssetManager (
    const std::filesystem::path & GameContentPath
) 
```





**Parameters:**


* `GameContentPath` The path to the game's content directory.

Constructor for [**AssetManager**](class_a_g_e_1_1_asset_manager.md) class.


This constructor initializes the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) with a given game content path and creates an instance of [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md). It also checks if there is already an instance of [**AssetManager**](class_a_g_e_1_1_asset_manager.md), in which case it asserts that no other instance should exist.




**Parameters:**


* `GameContentPath` The path to the game's content directory. 




        

<hr>



### function AssetManager [3/3]

_Constructor for the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _class._
```C++
AGE::AssetManager::AssetManager (
    void * AddrToPakFile,
    size_t SizeOfPakFile=0
) 
```



This constructor initializes an instance of the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) class with a pointer to a pak file and its size. It also checks if an instance of [**AssetManager**](class_a_g_e_1_1_asset_manager.md) already exists, logging an error message if it does. The instance is then set as the current one. 

**Parameters:**


* `AddrToPakFile` A void pointer to the start of the pak file memory block. 
* `SizeOfPakFile` The size of the pak file in bytes.

Constructor for [**AssetManager**](class_a_g_e_1_1_asset_manager.md) class. Initializes the asset manager with a pointer to an [**AssetPak**](class_a_g_e_1_1_asset_pak.md) object and its size. 

**Parameters:**


* `AddrToPakFile` Pointer to an [**AssetPak**](class_a_g_e_1_1_asset_pak.md) object. 
* `SizeOfPakFile` Size of the [**AssetPak**](class_a_g_e_1_1_asset_pak.md) object in bytes. 



**Returns:**

None 





        

<hr>



### function DoesShaderExist 

_Checks if a shader with the given name exists._ 
```C++
bool AGE::AssetManager::DoesShaderExist (
    const std::string & Name
) 
```



This function checks whether there is an existing shader in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry that matches the provided name.




**Parameters:**


* `Name` The name of the shader to check for. 



**Returns:**

True if a shader with the given name exists, false otherwise.


Checks if a shader with the given name exists.


This function checks whether there is a registered shader in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry that has the same name as provided.




**Parameters:**


* `Name` The name of the shader to check for. 



**Returns:**

True if a shader with the given name exists, false otherwise. 





        

<hr>



### function GetAsepriteTexture [1/2]

_Retrieves a texture from the registry using its unique identifier._ 
```C++
Ref< Texture2D > AGE::AssetManager::GetAsepriteTexture (
    const UUID & ID
) 
```



This function uses the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s Registry to get a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object with the specified [**UUID**](class_a_g_e_1_1_u_u_i_d.md). The returned reference can be used for further operations on the texture.




**Parameters:**


* `ID` A const reference to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the texture to retrieve. 



**Returns:**

Ref&lt;Texture2D&gt; A reference to the retrieved [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. If no such texture exists, an empty reference is returned.


Retrieves a texture from the asset manager using its unique identifier.


This function retrieves a texture from the registry of the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) instance by its unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)). The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) is used to identify and retrieve the specific texture.




**Parameters:**


* `ID` A constant reference to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) that represents the texture to be retrieved. 



**Returns:**

A Ref&lt;Texture2D&gt; object representing the requested texture. If no such texture exists, an empty Ref&lt;Texture2D&gt; object is returned. 





        

<hr>



### function GetAsepriteTexture [2/2]

_Retrieves a texture from the asset registry using an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file name._
```C++
Ref< Texture2D > AGE::AssetManager::GetAsepriteTexture (
    const std::string & Name
) 
```



This function takes in a string representing the name of an [**Aseprite**](class_a_g_e_1_1_aseprite.md) file, and returns a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. The actual retrieval is done through the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s internal registry.




**Parameters:**


* `Name` The name of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to retrieve the texture for. 



**Returns:**

Reference to the retrieved [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. If no such texture exists, an empty reference will be returned.


Retrieves a texture from the asset registry using an [**Aseprite**](class_a_g_e_1_1_aseprite.md) file name.


This function takes in an [**Aseprite**](class_a_g_e_1_1_aseprite.md) file name and returns a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. The actual retrieval of the texture is handled by the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s internal registry, which this function interacts with through `m_Registry`.




**Parameters:**


* `Name` The name of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file for which to retrieve the texture.



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object representing the desired texture. If no such texture exists in the registry, this function will return an empty Ref&lt;Texture2D&gt;. 





        

<hr>



### function GetAssetRegistry 

_Retrieves the Asset Registry object associated with this instance._ 
```C++
inline Ref< AssetRegistry > AGE::AssetManager::GetAssetRegistry () const
```





**Returns:**

A reference to the Asset Registry object. 





        

<hr>



### function GetFont [1/2]

_Retrieves a font from the asset manager._ 
```C++
Ref< AGEFont > AGE::AssetManager::GetFont (
    const UUID & ID
) 
```



This function retrieves a font with the specified unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)). The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) is used to identify and retrieve the font from the registry. If the font does not exist in the registry, an exception will be thrown.




**Parameters:**


* `ID` The unique identifier of the font to retrieve. 



**Returns:**

A reference to the requested font. 




**Exception:**


* `std::runtime_error` if the font with the specified [**UUID**](class_a_g_e_1_1_u_u_i_d.md) is not found in the registry.

Retrieves a font from the asset manager.


This function retrieves a font with the specified unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)). It returns a reference to the font if it exists, or an empty reference otherwise.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the font to retrieve. 



**Returns:**

A reference to the font if found, or an empty reference. 





        

<hr>



### function GetFont [2/2]

_Get a font from the asset manager._ 
```C++
Ref< AGEFont > AGE::AssetManager::GetFont (
    const std::string & Name
) 
```



This function retrieves a font with a specified name from the asset manager's registry. If the font does not exist, it will return an empty reference.




**Parameters:**


* `Name` The name of the font to retrieve. 



**Returns:**

A reference to the requested font if found; otherwise, an empty reference.


Retrieves a font from the asset manager.


This function is used to get a font with a specific name from the asset manager. The font can then be used for rendering text in the game.




**Parameters:**


* `Name` The name of the font to retrieve. 



**Returns:**

A reference to the requested font. If no such font exists, an empty reference will be returned. 





        

<hr>



### function GetGameContentPath 

_Returns the game content path._ 
```C++
inline std::filesystem::path & AGE::AssetManager::GetGameContentPath () 
```



This function returns a reference to the game content path, which is used as the root directory for all game-related content files. The returned path may be empty if it has not been set yet.




**Returns:**

A reference to the game content path. 





        

<hr>



### function GetScene [1/2]

_Retrieves a scene from the registry using its unique identifier._ 
```C++
Ref< Scene > AGE::AssetManager::GetScene (
    const UUID & ID
) 
```



This function takes in a constant reference to a [**UUID**](class_a_g_e_1_1_u_u_i_d.md), which is used as an identifier for the scene. It then returns a reference to the scene with that specific ID. If no such scene exists, it will return an empty reference.




**Parameters:**


* `ID` The unique identifier of the scene to be retrieved. 



**Returns:**

A reference to the scene if found, otherwise an empty reference.


Retrieves a scene from the registry using its unique identifier.


This function takes in a constant reference to a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) (Universally Unique Identifier), which is used as an index to retrieve the corresponding scene from the asset manager's registry. The function returns a `Ref< Scene >`, which represents a smart pointer to a [**Scene**](class_a_g_e_1_1_scene.md) object. If no such scene exists with the given ID, it will return an empty reference.




**Parameters:**


* `ID` A constant reference to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the scene to be retrieved. 



**Returns:**

The requested scene if found, otherwise an empty reference. 





        

<hr>



### function GetScene [2/2]

_Retrieves a scene with the given name._ 
```C++
Ref< Scene > AGE::AssetManager::GetScene (
    const std::string & Name
) 
```



This function retrieves and returns a reference to a [**Scene**](class_a_g_e_1_1_scene.md) object from the registry using the provided name string. If no such scene exists, it will return an empty Ref&lt;Scene&gt;.




**Parameters:**


* `Name` The name of the scene to retrieve. 



**Returns:**

A reference to the requested scene if found; otherwise, an empty Ref&lt;Scene&gt;.


Retrieves a scene by its name.


This function retrieves and returns the scene with the given name from the registry. If no such scene exists, it will return an empty reference.




**Parameters:**


* `Name` The name of the scene to retrieve. 



**Returns:**

A reference to the requested scene if found; otherwise, an empty reference. 





        

<hr>



### function GetSceneNames 

_This function retrieves the names of all scenes in the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._
```C++
void AGE::AssetManager::GetSceneNames (
    std::vector< std::string > & OutArray
) 
```





**Parameters:**


* `OutArray` A reference to a std::vector&lt;std::string&gt; where the scene names will be stored.



**Returns:**

void


This function retrieves the names of all scenes in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md).




**Parameters:**


* `OutArray` A reference to a std::vector&lt;std::string&gt; where the scene names will be stored.



**Returns:**

void 





        

<hr>



### function GetShader 

_Get a shader from the registry by name._ 
```C++
Ref< Shader > AGE::AssetManager::GetShader (
    const std::string & Name
) 
```



This function retrieves a shader object from the asset manager's registry using the provided name. The returned reference can be used to access and manipulate the shader.




**Parameters:**


* `Name` The name of the shader to retrieve. 



**Returns:**

A reference to the requested shader, or an empty reference if no such shader exists in the registry.


Get a shader from the registry by name. 

**Parameters:**


* `Name` The name of the shader to retrieve. 



**Returns:**

A reference to the requested shader, or an empty Ref if no such shader exists. 





        

<hr>



### function GetSound [1/2]

_Retrieves an audio source with a specific_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._
```C++
Ref< AudioSource > AGE::AssetManager::GetSound (
    const UUID & ID
) 
```



This function retrieves and returns the audio source associated with the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md) from the asset manager's registry. If no such sound exists, it will return an empty reference.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the audio source to retrieve. 



**Returns:**

A reference to the retrieved audio source or an empty reference if no such sound exists.


Retrieves an audio source with the given unique identifier.


This function retrieves and returns a reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object from the registry using its unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)). If no such sound exists, it will return an empty Ref&lt;AudioSource&gt;.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the audio source to retrieve. 



**Returns:**

A reference to the requested audio source if found; otherwise, an empty Ref&lt;AudioSource&gt;. 





        

<hr>



### function GetSound [2/2]

_Retrieves an audio source with the given name._ 
```C++
Ref< AudioSource > AGE::AssetManager::GetSound (
    const std::string & Name
) 
```



This function retrieves and returns a reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object from the registry using the provided name. If no such sound exists, it will return an empty reference.




**Parameters:**


* `Name` The name of the sound to retrieve. 



**Returns:**

A reference to the audio source with the given name, or an empty reference if no such sound exists.


Retrieves an audio source from the registry by name.


This function retrieves a reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object stored in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s Registry with the given Name. The returned Reference can be used to access and manipulate the sound data associated with this name.




**Parameters:**


* `Name` - A string representing the unique identifier of the audio source. 



**Returns:**

Ref&lt;AudioSource&gt; - A reference to an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s Registry. 





        

<hr>



### function GetTexture [1/2]

_Retrieves a texture from the asset manager._ 
```C++
Ref< Texture2D > AGE::AssetManager::GetTexture (
    UUID ID
) 
```



This function takes in an [**UUID**](class_a_g_e_1_1_u_u_i_d.md) (Universally Unique Identifier) of a texture, and returns a reference to that texture. If the texture does not exist, it will return an empty reference.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the texture to retrieve. 



**Returns:**

A reference to the requested texture if it exists, otherwise an empty reference.


Retrieves a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object with the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md).


This function retrieves and returns a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object from the asset manager's registry using the provided [**UUID**](class_a_g_e_1_1_u_u_i_d.md). The returned reference can be used for further operations on the texture, such as rendering or manipulation.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object to retrieve. 



**Returns:**

A reference to the requested [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. If no matching [**Texture2D**](class_a_g_e_1_1_texture2_d.md) is found in the registry, an empty Ref&lt;Texture2D&gt; will be returned. 





        

<hr>



### function GetTexture [2/2]

_Much slower option considering I had to implement the find function for this myself, however in the event that you don't know the ID for the particular texture you want to load you can search for it based on the name which == the filename._ 
```C++
Ref< Texture2D > AGE::AssetManager::GetTexture (
    const std::string & Name
) 
```





**Parameters:**


* `Name` - Name of [**Texture**](class_a_g_e_1_1_texture.md) 



**Return value:**


* `-` A newly created shared\_ptr with the texture

Retrieves a texture from the asset manager.


This function retrieves a texture with the specified name from the registry and returns it as a reference. If no such texture exists, an exception is thrown.




**Parameters:**


* `Name` The name of the texture to retrieve. 



**Returns:**

A reference to the retrieved texture. 




**Exception:**


* `std::runtime_error` if there's no texture with the given name in the registry.

Retrieves a texture from the asset manager. 

**Parameters:**


* `Name` The name of the texture to retrieve. 



**Returns:**

A reference to the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object if it exists, otherwise an empty Ref&lt;Texture2D&gt;. 





        

<hr>



### function IsAsepriteFileLoaded 

_Checks if an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file is loaded._
```C++
bool AGE::AssetManager::IsAsepriteFileLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether a given [**Aseprite**](class_a_g_e_1_1_aseprite.md) file has been loaded into the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` The path of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to check for. 



**Returns:**

True if the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file is loaded, false otherwise.


Checks if an [**Aseprite**](class_a_g_e_1_1_aseprite.md) file is loaded.


This function checks whether a given [**Aseprite**](class_a_g_e_1_1_aseprite.md) file has been loaded into the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` The path of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to check for. 



**Returns:**

True if the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file is loaded, false otherwise. 





        

<hr>



### function IsFontLoaded 

_Checks if a font is loaded._ 
```C++
bool AGE::AssetManager::IsFontLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the specified font file has been loaded into memory. It uses an internal registry to check this information.




**Parameters:**


* `Filepath` The path of the font file to be checked. 



**Returns:**

True if the font is loaded, false otherwise.


Checks if a font is loaded.


This function checks whether the specified font file is currently loaded in memory. It does this by querying the [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) object associated with the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) instance.




**Parameters:**


* `Filepath` The path to the font file to check for. 



**Returns:**

True if the font is loaded, false otherwise. 





        

<hr>



### function IsSceneLoaded 

_Checks if a scene is loaded._ 
```C++
bool AGE::AssetManager::IsSceneLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the given file path corresponds to an already loaded scene in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` The path of the scene to check for. 



**Returns:**

True if the scene is loaded, false otherwise.


Checks if a scene is loaded.


This function checks whether the specified file path corresponds to an already loaded scene in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` The path of the scene to be checked. 



**Returns:**

True if the scene is loaded, false otherwise. 





        

<hr>



### function IsSoundLoaded 

_Checks if a sound is loaded._ 
```C++
bool AGE::AssetManager::IsSoundLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the specified sound file is currently loaded in memory. It does this by using an [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) object to check its internal state.




**Parameters:**


* `Filepath` The path of the sound file to be checked. 



**Returns:**

True if the sound is loaded, false otherwise.


Checks if a sound is loaded.


This function checks whether the specified sound file is currently loaded in memory. It uses an internal registry to keep track of all loaded sounds, and returns true if the given filepath corresponds to a known sound that has been loaded. If the sound is not loaded or there was an error during the check, it will return false.




**Parameters:**


* `Filepath` The path to the sound file to be checked. 



**Returns:**

True if the sound is loaded, false otherwise. 





        

<hr>



### function IsSoundbankLoaded 

_Checks if a soundbank is loaded._ 
```C++
bool AGE::AssetManager::IsSoundbankLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the specified soundbank file has been loaded into memory. It does this by calling `AssetManager::IsSoundbankLoaded` on the internal registry object, which presumably handles all asset loading and management.




**Parameters:**


* `Filepath` The path to the soundbank file to check for. 



**Returns:**

True if the soundbank is loaded, false otherwise.


Checks if a soundbank is loaded.


This function checks whether the specified soundbank file has been loaded into memory. It does this by calling `AssetManager::IsSoundbankLoaded` on the internal registry object.




**Parameters:**


* `Filepath` The path to the soundbank file to check for. 



**Returns:**

True if the soundbank is loaded, false otherwise. 





        

<hr>



### function IsTextureLoaded 

_Checks if a texture is loaded._ 
```C++
bool AGE::AssetManager::IsTextureLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the given file path corresponds to an already loaded texture in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` The path of the texture to check for. 



**Returns:**

True if the texture is loaded, false otherwise.


Checks if a texture is loaded.


This function checks whether the given file path corresponds to an already loaded texture in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md).




**Parameters:**


* `Filepath` The path of the texture to check for. 



**Returns:**

True if the texture is loaded, false otherwise. 





        

<hr>



### function LoadAsepriteFile 

_Loads an_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file from the specified path._
```C++
Ref< Texture2D > AGE::AssetManager::LoadAsepriteFile (
    const std::filesystem::path & Filepath
) 
```



This function loads a texture from the provided file path using the Asset Registry's LoadTexture method. The loaded texture is then returned as a Ref&lt;Texture2D&gt; object.




**Parameters:**


* `Filepath` The path to the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to load. 



**Returns:**

A Ref&lt;Texture2D&gt; object representing the loaded texture, or an empty Ref if the file could not be loaded.


Loads an [**Aseprite**](class_a_g_e_1_1_aseprite.md) file from the specified path.


This function loads a texture from the given file path using the Asset Registry's LoadTexture method. The loaded texture is then returned as a Ref&lt;Texture2D&gt; object.




**Parameters:**


* `Filepath` The path to the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to load. 



**Returns:**

A Ref&lt;Texture2D&gt; object representing the loaded texture, or an empty Ref if the file could not be loaded. 





        

<hr>



### function LoadFont 

_Loads a font from the specified file path._ 
```C++
Ref< AGEFont > AGE::AssetManager::LoadFont (
    const std::filesystem::path & Filepath
) 
```



This function loads a font from the given file path and returns a reference to it. If the font is already loaded, this function will return a reference to that existing instance instead of loading the font again.




**Parameters:**


* `Filepath` The path to the font file. 



**Returns:**

A reference to the loaded font.


Loads a font from the specified file path.


This function loads a font from the given file path and returns a reference to it. If the font is already loaded, this will return a reference to that instance instead of loading again.




**Parameters:**


* `Filepath` The path to the font file. 



**Returns:**

A reference to the loaded font. 





        

<hr>



### function LoadPakFile 

_Loads a PAK file into the_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._
```C++
bool AGE::AssetManager::LoadPakFile (
    void * AddrToPakFile,
    size_t SizeOfPakFile=0
) 
```



This function takes in an address and size of a PAK file, stores them as members of the class, and returns true if the pointer to the PAK file is not null.




**Parameters:**


* `AddrToPakFile` A void pointer to the start of the PAK file data. 
* `SizeOfPakFile` The size of the PAK file in bytes.



**Returns:**

True if the PAK file was successfully loaded, false otherwise.


Loads a PAK file into the [**AssetManager**](class_a_g_e_1_1_asset_manager.md).


This function takes in an address and size of a PAK file, stores them as a pair in m\_PakPair, and returns true if the pointer to the PAK file is not null.




**Parameters:**


* `AddrToPakFile` A void pointer to the start of the PAK file data. 
* `SizeOfPakFile` The size of the PAK file in bytes.



**Returns:**

True if the PAK file was successfully loaded, false otherwise. 





        

<hr>



### function LoadScene 

_Loads a scene from the given file path._ 
```C++
Ref< Scene > AGE::AssetManager::LoadScene (
    const std::filesystem::path & Filepath
) 
```



This function loads a scene from the specified file path and returns it as a reference to a [**Scene**](class_a_g_e_1_1_scene.md) object. If the scene cannot be loaded, an exception is thrown.




**Parameters:**


* `Filepath` The path of the scene file to load. 



**Returns:**

A reference to the loaded [**Scene**](class_a_g_e_1_1_scene.md) object. 




**Exception:**


* `std::runtime_error` if the scene could not be loaded.

Loads a scene from the given file path.


This function loads a scene from the specified file path and returns it as a reference to an [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s [**Scene**](class_a_g_e_1_1_scene.md) object. The file path is used to identify the location of the scene data.




**Parameters:**


* `Filepath` The path to the scene file. 



**Returns:**

A reference to the loaded scene. 





        

<hr>



### function LoadShader [1/3]

_Loads a shader from the specified file path._ 
```C++
void AGE::AssetManager::LoadShader (
    const std::string & FilePath
) 
```



This function takes in a constant string reference (const std::string&) as an argument, which represents the file path of the shader to be loaded. It then calls the `LoadShader` method on the member variable m\_Registry with this file path as its parameter.




**Parameters:**


* `FilePath` The file path of the shader to load.

Loads a shader from the specified file path.


This function takes in a constant string reference, which represents the file path of the shader to be loaded. It then uses this file path to load the shader using the `LoadShader` method on the `m_Registry` object.




**Parameters:**


* `FilePath` The file path of the shader to be loaded. 




        

<hr>



### function LoadShader [2/3]

_Loads a shader from two file paths._ 
```C++
void AGE::AssetManager::LoadShader (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```



This function loads a shader using the provided file paths and registers it in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry. The first parameter is the path to the vertex shader file, while the second one is for the fragment (or pixel) shader.




**Parameters:**


* `FilePath1` Path to the vertex shader file. 
* `FilePath2` Path to the fragment shader file.

Loads a shader from two file paths.


This function loads a shader using the provided file paths and registers it in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry. The first parameter is the path to the vertex shader, while the second one is for the fragment (or pixel) shader. 

**Parameters:**


* `FilePath1` Path to the vertex shader file. 
* `FilePath2` Path to the fragment shader file. 




        

<hr>



### function LoadShader [3/3]

_Loads a shader into the asset manager._ 
```C++
void AGE::AssetManager::LoadShader (
    const int Name,
    const std::string & Source
) 
```



This function takes in an integer Name and a string reference Source. It then calls the LoadShader method on the m\_Registry object with these parameters. The purpose of this function is to load a shader into the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) for later use.




**Parameters:**


* `Name` A unique identifier for the shader. 
* `Source` The source code of the shader.

Loads a shader into the asset manager.


This function takes an integer and a string as parameters. The integer is used to identify the shader in some way (e.g., its name or ID), while the string contains the source code of the shader. It then calls the `LoadShader` method on the registry object, passing these two values along.




**Parameters:**


* `Name` A unique identifier for the shader to be loaded. 
* `Source` The source code of the shader. 




        

<hr>



### function LoadSound 

_Loads a sound from the specified file path._ 
```C++
Ref< AudioSource > AGE::AssetManager::LoadSound (
    const std::filesystem::path & Filepath
) 
```



This function loads an audio source from the given file path and returns a reference to it. If the sound is already loaded, this function will return a reference to the existing sound.




**Parameters:**


* `Filepath` The path of the sound file to load. 



**Returns:**

A reference to the loaded or existing sound.


Loads a sound from the given file path.


This function loads an audio source from the specified file path and returns a reference to it. If the sound is already loaded, this will return a reference to that existing sound.




**Parameters:**


* `Filepath` The path of the sound file to load. 



**Returns:**

A reference to the loaded audio source. 





        

<hr>



### function LoadSoundbank 

_Loads a soundbank from the specified file path._ 
```C++
void AGE::AssetManager::LoadSoundbank (
    const std::filesystem::path & Filepath
) 
```



This function takes in a const reference to a std::filesystem::path object, which represents the location of the soundbank file on disk. The function then uses this path to load the soundbank into the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry.




**Parameters:**


* `Filepath` A constant reference to a std::filesystem::path object representing the location of the soundbank file on disk.



**Returns:**

void No return value is provided by this function.


Loads a soundbank from the specified file path.


This function takes in a const reference to a std::filesystem::path object, which represents the location of the soundbank file on disk. The function then uses this path to load the soundbank into memory using the [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md)'s LoadSoundbank method.




**Parameters:**


* `Filepath` A const reference to a std::filesystem::path object representing the location of the soundbank file on disk. 



**Returns:**

void No return value. 





        

<hr>



### function LoadTexture [1/2]

_Loads a texture from the specified file path._ 
```C++
Ref< Texture2D > AGE::AssetManager::LoadTexture (
    const std::filesystem::path & FilePath
) 
```



This function takes in a constant reference to a filesystem path, which represents the location of the texture file on disk. It returns an instance of Ref&lt;Texture2D&gt;, which is essentially a smart pointer that manages the lifetime of [**Texture2D**](class_a_g_e_1_1_texture2_d.md) objects. The actual loading and management of textures is handled by the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s registry object.




**Parameters:**


* `FilePath` A constant reference to the filesystem path of the texture file on disk. 



**Returns:**

An instance of Ref&lt;Texture2D&gt;, which represents a smart pointer managing the lifetime of [**Texture2D**](class_a_g_e_1_1_texture2_d.md) objects.


Loads a texture from the specified file path.


This function takes in a constant reference to a filesystem path, which represents the location of the texture file on disk. It returns a `Ref< Texture2D >` object, which is essentially a smart pointer that manages the lifetime of a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) instance. The actual loading and management of textures is handled by an internal registry in the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) class.




**Parameters:**


* `FilePath` A constant reference to a filesystem path representing the location of the texture file on disk. 



**Returns:**

Ref&lt;Texture2D&gt; A smart pointer that manages the lifetime of a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) instance. 





        

<hr>



### function LoadTexture [2/2]

_Loads a texture from binary data._ 
```C++
Ref< Texture2D > AGE::AssetManager::LoadTexture (
    void * Addr,
    size_t Size
) 
```



This function loads a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object from raw binary data. The binary data is expected to be in the format that was used when saving the texture, i.e., it should contain all necessary information for re-creating the texture.




**Parameters:**


* `Addr` A pointer to the start of the binary data. 
* `Size` The size of the binary data in bytes.



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, or nullptr if the loading failed.


Loads a texture from binary data.


This function loads a texture from the provided binary data. The binary data is expected to be in a format that can be understood by the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) class, such as PNG or JPEG. If the loading fails for any reason, it returns nullptr.




**Parameters:**


* `Addr` A pointer to the start of the binary data. 
* `Size` The size of the binary data in bytes.



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object representing the loaded texture. If loading fails, this will be a null reference. 





        

<hr>



### function RegisterAsset 

_Registers an asset of type T into the system._ 
```C++
template<typename T>
inline void AGE::AssetManager::RegisterAsset (
    Ref< T > Asset
) 
```



This function registers an asset of a specific type (T) into the system. If the type is [**AudioSource**](class_a_g_e_1_1_audio_source.md), it will log an error message saying that registering audio sources is currently unsupported. For [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) and [**Texture2D**](class_a_g_e_1_1_texture2_d.md) types, it will call the RegisterFont method on the registry object with the given asset as parameter.




**Parameters:**


* `Asset` The asset to be registered. 




        

<hr>
## Public Static Functions Documentation




### function Get 

_Returns a reference to the global instance of_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._
```C++
static inline AssetManager & AGE::AssetManager::Get () 
```





**Returns:**

Reference to the global [**AssetManager**](class_a_g_e_1_1_asset_manager.md) instance. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Assets/Public/AssetManager.h`

