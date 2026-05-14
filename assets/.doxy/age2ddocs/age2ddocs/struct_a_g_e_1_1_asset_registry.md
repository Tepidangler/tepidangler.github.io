

# Struct AGE::AssetRegistry



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  Scope&lt; [**Aseprite**](class_a_g_e_1_1_aseprite.md) &gt; | [**m\_AespriteManager**](#variable-m_aespritemanager)  <br> |
|  [**AudioManager**](class_a_g_e_1_1_audio_manager.md) \* | [**m\_AudioManager**](#variable-m_audiomanager)  <br> |
|  std::vector&lt; std::string &gt; | [**m\_FontNames**](#variable-m_fontnames)  <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; &gt; | [**m\_Fonts**](#variable-m_fonts)  <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; &gt; | [**m\_Scenes**](#variable-m_scenes)  <br> |
|  Ref&lt; [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md) &gt; | [**m\_ShaderLibrary**](#variable-m_shaderlibrary)  <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; | [**m\_SoundBanks**](#variable-m_soundbanks)  <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; | [**m\_Sounds**](#variable-m_sounds)  <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; &gt; | [**m\_TextureAssets**](#variable-m_textureassets)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AssetRegistry**](#function-assetregistry-13) ([**AudioManager**](class_a_g_e_1_1_audio_manager.md) \* AudioManagerPtr) <br>_Constructs an_ [_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _object._ |
|   | [**AssetRegistry**](#function-assetregistry-23) (const [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &) = delete<br>_Deleted copy constructor for the_ [_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _class to prevent copying._ |
|   | [**AssetRegistry**](#function-assetregistry-33) ([**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &&) = delete<br>[_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _is a class that manages assets in the game engine. It's designed to be efficient and secure, but it doesn't allow copying or moving instances of this class for safety reasons._ |
|  bool | [**DoesShaderExist**](#function-doesshaderexist) (const std::string & Name) <br>_Checks if a shader with the given name exists._  |
|  std::vector&lt; Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; &gt; | [**GetAllScenes**](#function-getallscenes) () <br>_GetAllScenes returns a vector of all scenes in the system._  |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves a font with the given_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map of fonts._ |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-22) (const std::string & Name) <br>_Retrieves a font from the collection based on its name._  |
|  const std::vector&lt; std::string &gt; & | [**GetFontNames**](#function-getfontnames) () <br>_Get the names of all available fonts._  |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; &gt; & | [**GetFonts**](#function-getfonts) () <br>_Returns a reference to the unordered map containing all fonts._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Retrieves a scene with the given_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map of scenes._ |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-22) (const std::string & Name) <br>_GetScene is a function that retrieves a scene from the map of scenes by its name._  |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; &gt; & | [**GetScenes**](#function-getscenes) () <br>_Returns a reference to the unordered map containing all scenes._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**GetShader**](#function-getshader) (const std::string & Name) <br>_Gets a shader from the library by name._  |
|  Ref&lt; [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md) &gt; & | [**GetShaders**](#function-getshaders) () <br>_Gets the shader library reference._  |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br>_Retrieves an_ [_**AudioSource**_](class_a_g_e_1_1_audio_source.md) _with the given_[_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map m\_Sounds._ |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-22) (const std::string & Name) <br>_Retrieves an_ [_**AudioSource**_](class_a_g_e_1_1_audio_source.md) _with a specific name from the map of sounds._ |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & | [**GetSoundbanks**](#function-getsoundbanks) () <br>_Returns a reference to the unordered map containing all SoundBanks._  |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; & | [**GetSounds**](#function-getsounds) () <br>_Returns a reference to the unordered map containing all audio sources._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-12) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Retrieves a texture from the asset manager using its_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-22) (const std::string & Name) <br>_Retrieves a reference to the_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object associated with the given name._ |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; &gt; & | [**GetTextures**](#function-gettextures) () <br>_Returns a reference to the unordered map containing all texture assets._  |
|  bool | [**IsFontLoaded**](#function-isfontloaded) (const std::filesystem::path & Filepath) <br>_Checks if a font is loaded._  |
|  bool | [**IsSceneLoaded**](#function-issceneloaded) (const std::filesystem::path & Path) <br>_Checks if a scene is loaded based on its path._  |
|  bool | [**IsSoundLoaded**](#function-issoundloaded) (const std::filesystem::path & Filepath) <br>_Checks if a sound is loaded based on the file path._  |
|  bool | [**IsSoundbankLoaded**](#function-issoundbankloaded) (const std::filesystem::path & Filepath) <br>_Checks if a soundbank is loaded._  |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-13) (const std::filesystem::path & Path) <br>_Checks if a texture is loaded based on its file path._  |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-23) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Checks whether a texture with the given ID is loaded or not._  |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-33) (const std::filesystem::path & Path, [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & OutID) <br>_Checks if a texture is loaded based on its file path._  |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**LoadFont**](#function-loadfont) (const std::filesystem::path & Filepath) <br>_Load a font from the specified filepath and return its reference._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Filepath) <br>_Loads a scene from the specified file path and returns it as a reference._  |
|  void | [**LoadShader**](#function-loadshader-13) (const std::string & FilePath) <br>_This function loads a shader from the given file path._  |
|  void | [**LoadShader**](#function-loadshader-23) (const std::string & FilePath1, const std::string & FilePath2) <br>_This function loads two shaders from the given file paths._  |
|  void | [**LoadShader**](#function-loadshader-33) (const int Name, const std::string & Source) <br>_This function loads a shader into the_ [_**Shader**_](class_a_g_e_1_1_shader.md) _Library._ |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**LoadSound**](#function-loadsound) (const std::filesystem::path & Filepath) <br>_Loads a sound file from the specified path and returns a reference to it._  |
|  bool | [**LoadSoundbank**](#function-loadsoundbank) (const std::filesystem::path & Filepath) <br>_Loads a sound bank from the specified file path._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture) (const std::filesystem::path & FilePath) <br> |
|  void | [**RegisterFont**](#function-registerfont) (const Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; & font) <br>_Registers a new font with the system._  |
|   | [**~AssetRegistry**](#function-assetregistry) () = default<br> |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::AssetRegistry::__pad0__;
```




<hr>



### variable m\_AespriteManager 

```C++
Scope<Aseprite> AGE::AssetRegistry::m_AespriteManager;
```




<hr>



### variable m\_AudioManager 

```C++
AudioManager* AGE::AssetRegistry::m_AudioManager;
```




<hr>



### variable m\_FontNames 

```C++
std::vector<std::string> AGE::AssetRegistry::m_FontNames;
```




<hr>



### variable m\_Fonts 

```C++
std::unordered_map<UUID, Ref<AGEFont> > AGE::AssetRegistry::m_Fonts;
```




<hr>



### variable m\_Scenes 

```C++
std::unordered_map<UUID,Ref<Scene> > AGE::AssetRegistry::m_Scenes;
```




<hr>



### variable m\_ShaderLibrary 

```C++
Ref<ShaderLibrary> AGE::AssetRegistry::m_ShaderLibrary;
```




<hr>



### variable m\_SoundBanks 

```C++
std::unordered_map<UUID, Ref<SoundBank> > AGE::AssetRegistry::m_SoundBanks;
```




<hr>



### variable m\_Sounds 

```C++
std::unordered_map<UUID, Ref<AudioSource> > AGE::AssetRegistry::m_Sounds;
```




<hr>



### variable m\_TextureAssets 

```C++
std::unordered_map<UUID, Ref<Texture2D> > AGE::AssetRegistry::m_TextureAssets;
```




<hr>
## Public Functions Documentation




### function AssetRegistry [1/3]

_Constructs an_ [_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _object._
```C++
inline AGE::AssetRegistry::AssetRegistry (
    AudioManager * AudioManagerPtr
) 
```



This constructor initializes the [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md), [**Aseprite**](class_a_g_e_1_1_aseprite.md) manager and sets the [**AudioManager**](class_a_g_e_1_1_audio_manager.md) pointer.




**Parameters:**


* `AudioManagerPtr` Pointer to the [**AudioManager**](class_a_g_e_1_1_audio_manager.md) instance. 




        

<hr>



### function AssetRegistry [2/3]

_Deleted copy constructor for the_ [_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _class to prevent copying._
```C++
AGE::AssetRegistry::AssetRegistry (
    const AssetRegistry &
) = delete
```





**Parameters:**


* `other` The instance of the [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) that is being copied. 




        

<hr>



### function AssetRegistry [3/3]

[_**AssetRegistry**_](struct_a_g_e_1_1_asset_registry.md) _is a class that manages assets in the game engine. It's designed to be efficient and secure, but it doesn't allow copying or moving instances of this class for safety reasons._
```C++
AGE::AssetRegistry::AssetRegistry (
    AssetRegistry &&
) = delete
```





**Returns:**

The function does not return any value. 





        

<hr>



### function DoesShaderExist 

_Checks if a shader with the given name exists._ 
```C++
inline bool AGE::AssetRegistry::DoesShaderExist (
    const std::string & Name
) 
```



This function checks whether a shader with the specified name exists in the shader library. It returns true if the shader exists and false otherwise.




**Parameters:**


* `Name` The name of the shader to check for. 



**Returns:**

True if the shader exists, false otherwise. 





        

<hr>



### function GetAllScenes 

_GetAllScenes returns a vector of all scenes in the system._ 
```C++
inline std::vector< Ref< Scene > > AGE::AssetRegistry::GetAllScenes () 
```



This function iterates over the map m\_Scenes and emplaces each scene into the returned vector. The scenes are stored as Ref&lt;Scene&gt; objects, which allows for polymorphic usage.




**Returns:**

std::vector&lt;Ref&lt;Scene&gt;&gt; A vector containing all scenes in the system. 





        

<hr>



### function GetFont [1/2]

_Retrieves a font with the given_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map of fonts._
```C++
inline Ref< AGEFont > AGE::AssetRegistry::GetFont (
    const UUID & ID
) 
```



This function searches for a font in the map 'm\_Fonts' using the provided [**UUID**](class_a_g_e_1_1_u_u_i_d.md). If the font is found, it returns a reference to that font. Otherwise, it returns a null reference. 

**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the font to be retrieved. 



**Returns:**

A reference to the font with the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md) if it exists in 'm\_Fonts'. Otherwise, a null reference. 





        

<hr>



### function GetFont [2/2]

_Retrieves a font from the collection based on its name._ 
```C++
inline Ref< AGEFont > AGE::AssetRegistry::GetFont (
    const std::string & Name
) 
```



This function iterates over all fonts in the collection and checks if their atlas texture's name matches the provided one. If it does, that font is returned. Otherwise, nullptr is returned to indicate that no such font exists.




**Parameters:**


* `Name` The name of the font to retrieve. 



**Returns:**

A reference to the requested font or a null reference if no matching font was found. 





        

<hr>



### function GetFontNames 

_Get the names of all available fonts._ 
```C++
inline const std::vector< std::string > & AGE::AssetRegistry::GetFontNames () 
```



This function retrieves a list of font names from the internal map of fonts. If the list is empty, it populates it by iterating over each font in the map and adding its name to the list. The resulting list is then returned.




**Returns:**

A const reference to a vector of strings representing the names of all available fonts. 





        

<hr>



### function GetFonts 

_Returns a reference to the unordered map containing all fonts._ 
```C++
inline std::unordered_map< UUID , Ref< AGEFont > > & AGE::AssetRegistry::GetFonts () 
```



This function returns a reference to an unordered map that contains all the fonts in the system. The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) is used as the key and Ref&lt;AGEFont&gt; is the value.




**Returns:**

std::unordered\_map&lt;UUID, Ref&lt;AGEFont&gt;&gt;& A reference to the m\_Fonts member variable. 





        

<hr>



### function GetScene [1/2]

_Retrieves a scene with the given_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map of scenes._
```C++
inline Ref< Scene > AGE::AssetRegistry::GetScene (
    const UUID ID
) 
```



This function takes in an [**UUID**](class_a_g_e_1_1_u_u_i_d.md) and returns the corresponding [**Scene**](class_a_g_e_1_1_scene.md) object from the map 'm\_Scenes'. If no such scene exists, it will return an empty Ref&lt;Scene&gt;.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the scene to be retrieved. 



**Returns:**

A reference to the requested [**Scene**](class_a_g_e_1_1_scene.md) if found in the map; otherwise, an empty Ref&lt;Scene&gt;. 





        

<hr>



### function GetScene [2/2]

_GetScene is a function that retrieves a scene from the map of scenes by its name._ 
```C++
inline Ref< Scene > AGE::AssetRegistry::GetScene (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The name of the scene to be retrieved. 



**Returns:**

A reference to the [**Scene**](class_a_g_e_1_1_scene.md) object if it exists, otherwise nullptr. If no such scene exists, an error message will be logged and nullptr will be returned. 





        

<hr>



### function GetScenes 

_Returns a reference to the unordered map containing all scenes._ 
```C++
inline std::unordered_map< UUID , Ref< Scene > > & AGE::AssetRegistry::GetScenes () 
```



This function returns a reference to an unordered map that contains all the scenes in the system. The key is of type [**UUID**](class_a_g_e_1_1_u_u_i_d.md) and the value is of type Ref&lt;Scene&gt;, which represents a scene reference.




**Returns:**

A reference to the unordered map containing all scenes. 





        

<hr>



### function GetShader 

_Gets a shader from the library by name._ 
```C++
inline Ref< Shader > AGE::AssetRegistry::GetShader (
    const std::string & Name
) 
```



This function retrieves a shader object from the library using the provided name. If the shader does not exist, it will return an empty reference.




**Parameters:**


* `Name` The name of the shader to retrieve. 



**Returns:**

A reference to the shader with the given name, or an empty reference if no such shader exists in the library. 





        

<hr>



### function GetShaders 

_Gets the shader library reference._ 
```C++
inline Ref< ShaderLibrary > & AGE::AssetRegistry::GetShaders () 
```



This function returns a reference to the shader library object, which can be used to access and manipulate the shaders in the library.




**Returns:**

A reference to the [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md) object. 





        

<hr>



### function GetSound [1/2]

_Retrieves an_ [_**AudioSource**_](class_a_g_e_1_1_audio_source.md) _with the given_[_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _from the map m\_Sounds._
```C++
inline Ref< AudioSource > AGE::AssetRegistry::GetSound (
    const UUID & ID
) 
```



This function takes a constant reference to a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) (ID) and attempts to find it in the map m\_Sounds. If the ID is found, the corresponding Ref&lt;AudioSource&gt; object is returned. Otherwise, a null pointer is returned.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the [**AudioSource**](class_a_g_e_1_1_audio_source.md) to retrieve from the map. 



**Returns:**

A Ref&lt;AudioSource&gt; object that corresponds to the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md) in m\_Sounds. If no such object exists, a null pointer is returned. 





        

<hr>



### function GetSound [2/2]

_Retrieves an_ [_**AudioSource**_](class_a_g_e_1_1_audio_source.md) _with a specific name from the map of sounds._
```C++
inline Ref< AudioSource > AGE::AssetRegistry::GetSound (
    const std::string & Name
) 
```



This function iterates over all entries in the m\_Sounds map and checks if the GetName() method of each entry returns the same string as the input parameter 'Name'. If it does, that entry is returned. If no such entry exists, a nullptr is returned.




**Parameters:**


* `Name` The name to search for in the [**AudioSource**](class_a_g_e_1_1_audio_source.md) objects. 



**Returns:**

A Ref&lt;AudioSource&gt; object representing the found sound or nullptr if not found. 





        

<hr>



### function GetSoundbanks 

_Returns a reference to the unordered map containing all SoundBanks._ 
```C++
inline std::unordered_map< UUID , Ref< SoundBank > > & AGE::AssetRegistry::GetSoundbanks () 
```



This function returns a reference to an unordered map that contains all SoundBanks in the system. The keys of this map are UUIDs and the values are references (Ref) to [**SoundBank**](class_a_g_e_1_1_sound_bank.md) objects.




**Returns:**

A reference to the unordered\_map&lt;UUID, Ref&lt;SoundBank&gt;&gt; containing all SoundBanks. 





        

<hr>



### function GetSounds 

_Returns a reference to the unordered map containing all audio sources._ 
```C++
inline std::unordered_map< UUID , Ref< AudioSource > > & AGE::AssetRegistry::GetSounds () 
```



This function returns a reference to an unordered map that contains all [**AudioSource**](class_a_g_e_1_1_audio_source.md) objects in the system. The UUIDs of these objects are used as keys for this map.




**Returns:**

A reference to the unordered map m\_Sounds. 





        

<hr>



### function GetTexture [1/2]

_Retrieves a texture from the asset manager using its_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._
```C++
inline Ref< Texture2D > AGE::AssetRegistry::GetTexture (
    UUID ID
) 
```



This function searches for a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object in the m\_TextureAssets map with the given ID. If it finds one, it returns a reference to that object. Otherwise, it logs an error and returns a nullptr. 

**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the texture to retrieve. 



**Returns:**

A Reference (Ref) to the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object if found, otherwise nullptr. 





        

<hr>



### function GetTexture [2/2]

_Retrieves a reference to the_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object associated with the given name._
```C++
inline Ref< Texture2D > AGE::AssetRegistry::GetTexture (
    const std::string & Name
) 
```



This function iterates over all stored texture assets and checks if any of them have the same name as the input parameter 'Name'. If it finds one, it returns a reference to that [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. Otherwise, it logs an error message and returns a null reference.




**Parameters:**


* `Name` The name of the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) asset to retrieve. 



**Returns:**

A reference to the requested [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object if found, otherwise nullptr. 





        

<hr>



### function GetTextures 

_Returns a reference to the unordered map containing all texture assets._ 
```C++
inline std::unordered_map< UUID , Ref< Texture2D > > & AGE::AssetRegistry::GetTextures () 
```



This function returns a reference to an unordered map that contains all [**Texture2D**](class_a_g_e_1_1_texture2_d.md) assets currently loaded in the game. The UUIDs of these textures are used as keys for this map.




**Returns:**

A reference to the unordered\_map&lt;UUID, Ref&lt;Texture2D&gt;&gt; containing all texture assets. 





        

<hr>



### function IsFontLoaded 

_Checks if a font is loaded._ 
```C++
inline bool AGE::AssetRegistry::IsFontLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether the given file path corresponds to any of the fonts in the system. It does this by iterating over all stored fonts and comparing their atlas texture paths with the provided one. If it finds a match, it returns true indicating that the font is loaded. Otherwise, it returns false.




**Parameters:**


* `Filepath` The path of the file to check for.



**Returns:**

True if the font is loaded, false otherwise. 





        

<hr>



### function IsSceneLoaded 

_Checks if a scene is loaded based on its path._ 
```C++
inline bool AGE::AssetRegistry::IsSceneLoaded (
    const std::filesystem::path & Path
) 
```



This function takes in the file system path of a potential scene and checks if it exists within the list of currently loaded scenes. It does this by comparing the filename part of the path with the names of all currently loaded scenes.




**Parameters:**


* `Path` The file system path to check for a loaded scene. 



**Returns:**

True if a scene is found at the given path, false otherwise. 





        

<hr>



### function IsSoundLoaded 

_Checks if a sound is loaded based on the file path._ 
```C++
inline bool AGE::AssetRegistry::IsSoundLoaded (
    const std::filesystem::path & Filepath
) 
```



This function iterates over all sounds stored in the m\_Sounds map and checks if any of them have the same file path as provided. If it finds one, it returns true; otherwise, false.




**Parameters:**


* `Filepath` The file path to check for. 



**Returns:**

True if a sound with the given file path is loaded, false otherwise. 





        

<hr>



### function IsSoundbankLoaded 

_Checks if a soundbank is loaded._ 
```C++
inline bool AGE::AssetRegistry::IsSoundbankLoaded (
    const std::filesystem::path & Filepath
) 
```



This function checks whether a soundbank with the given filepath is loaded based on the audio engine type in use by the [**AudioManager**](class_a_g_e_1_1_audio_manager.md). It supports two types of engines - Wwise and FMod. For each, it uses preprocessor directives to check if the corresponding SDKs are enabled during compilation.




**Parameters:**


* `Filepath` The path to the soundbank file. 



**Returns:**

True if the soundbank is loaded, false otherwise. 





        

<hr>



### function IsTextureLoaded [1/3]

_Checks if a texture is loaded based on its file path._ 
```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const std::filesystem::path & Path
) 
```



This function iterates over the map of textures (m\_TextureAssets) and checks if any texture's GetTextureFilePath() matches the provided path. If it does, the function returns true indicating that the texture is loaded. Otherwise, it returns false.




**Parameters:**


* `Path` The file path to check for a loaded texture. 



**Returns:**

True if the texture is loaded, false otherwise. 





        

<hr>



### function IsTextureLoaded [2/3]

_Checks whether a texture with the given ID is loaded or not._ 
```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const UUID ID
) 
```



This function checks if the texture associated with the provided [**UUID**](class_a_g_e_1_1_u_u_i_d.md) (Universally Unique Identifier) is already loaded in memory. It does this by comparing the value of `m_TextureAssets[ID]` to `nullptr`. If it's equal, then the texture has not been loaded and the function returns false; otherwise, if it's not equal (i.e., the texture is loaded), the function returns true.




**Parameters:**


* `ID` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the texture to check for. 



**Returns:**

True if the texture with the given ID is loaded, False otherwise. 





        

<hr>



### function IsTextureLoaded [3/3]

_Checks if a texture is loaded based on its file path._ 
```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const std::filesystem::path & Path,
    UUID & OutID
) 
```



This function iterates over the map of textures (m\_TextureAssets) and checks if any of them have the same file path as the one provided. If it finds a match, it sets the OutID parameter to the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) associated with that texture and returns true. Otherwise, it returns false.




**Parameters:**


* `Path` The file path of the texture to check for. 
* `OutID` A reference to an [**UUID**](class_a_g_e_1_1_u_u_i_d.md) variable which will be set if the texture is found.



**Returns:**

Returns true if a texture with the given file path exists in m\_TextureAssets, false otherwise. 





        

<hr>



### function LoadFont 

_Load a font from the specified filepath and return its reference._ 
```C++
inline Ref< AGEFont > AGE::AssetRegistry::LoadFont (
    const std::filesystem::path & Filepath
) 
```



This function creates a new instance of [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) with the provided filepath, generates a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for it, stores the font in the map m\_Fonts using the generated [**UUID**](class_a_g_e_1_1_u_u_i_d.md) as key, then returns the newly created font's reference. 

**Parameters:**


* `Filepath` The path to the font file. 



**Returns:**

Reference to the loaded font. 





        

<hr>



### function LoadScene 

_Loads a scene from the specified file path and returns it as a reference._ 
```C++
inline Ref< Scene > AGE::AssetRegistry::LoadScene (
    const std::filesystem::path & Filepath
) 
```



If the function is unable to load the scene due to an error, it will log an error message and return nullptr. 


        

<hr>



### function LoadShader [1/3]

_This function loads a shader from the given file path._ 
```C++
inline void AGE::AssetRegistry::LoadShader (
    const std::string & FilePath
) 
```





**Parameters:**


* `FilePath` The path to the shader file. 



**Returns:**

void 





        

<hr>



### function LoadShader [2/3]

_This function loads two shaders from the given file paths._ 
```C++
inline void AGE::AssetRegistry::LoadShader (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```





**Parameters:**


* `FilePath1` The path to the first shader file. 
* `FilePath2` The path to the second shader file. 



**Returns:**

void 





        

<hr>



### function LoadShader [3/3]

_This function loads a shader into the_ [_**Shader**_](class_a_g_e_1_1_shader.md) _Library._
```C++
inline void AGE::AssetRegistry::LoadShader (
    const int Name,
    const std::string & Source
) 
```





**Parameters:**


* `Name` The identifier for the shader to be loaded. 
* `Source` The source code of the shader.



**Returns:**

void 





        

<hr>



### function LoadSound 

_Loads a sound file from the specified path and returns a reference to it._ 
```C++
inline Ref< AudioSource > AGE::AssetRegistry::LoadSound (
    const std::filesystem::path & Filepath
) 
```



The function creates an [**AudioSource**](class_a_g_e_1_1_audio_source.md) object with the given filepath, generates a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for the sound, stores the sound in the m\_Sounds map under its ID, then retrieves and returns the sound using its ID.




**Parameters:**


* `Filepath` The path of the sound file to load. 



**Returns:**

A reference to the loaded [**AudioSource**](class_a_g_e_1_1_audio_source.md) object. 





        

<hr>



### function LoadSoundbank 

_Loads a sound bank from the specified file path._ 
```C++
inline bool AGE::AssetRegistry::LoadSoundbank (
    const std::filesystem::path & Filepath
) 
```



This function loads a sound bank into the audio manager based on the type of audio engine currently in use. If the audio engine is WWise, it directly loads the bank into the audio engine using `AudioEngine::LoadBank`. For FModEngine, it creates a Sound Bank object and then loads that into the audio engine.




**Parameters:**


* `Filepath` The path to the sound bank file. 



**Returns:**

True if the sound bank was successfully loaded, false otherwise. 





        

<hr>



### function LoadTexture 

```C++
inline Ref< Texture2D > AGE::AssetRegistry::LoadTexture (
    const std::filesystem::path & FilePath
) 
```



Loads a texture from the given file path and returns it as a reference. If the texture is already loaded, it will return that instance instead of loading again. The function checks if the texture is already loaded by its [**UUID**](class_a_g_e_1_1_u_u_i_d.md). If so, it directly returns the existing texture. Otherwise, it creates a new [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object based on the file type: .aseprite for AespriteManager, and regular image files otherwise. After creating the texture, it assigns an unique [**UUID**](class_a_g_e_1_1_u_u_i_d.md) to it and stores it in m\_TextureAssets map with its [**UUID**](class_a_g_e_1_1_u_u_i_d.md) as key. Finally, it returns the loaded [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object from m\_TextureAssets using its [**UUID**](class_a_g_e_1_1_u_u_i_d.md). 


        

<hr>



### function RegisterFont 

_Registers a new font with the system._ 
```C++
inline void AGE::AssetRegistry::RegisterFont (
    const Ref< AGEFont > & font
) 
```



This function takes in a reference to an [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) object and adds it to the map of registered fonts. The key for this entry is the AssetID of the font, which can be accessed using GetAssetID() method on the font object.




**Parameters:**


* `font` - Reference to the font that needs to be registered.



**Returns:**

void 





        

<hr>



### function ~AssetRegistry 

```C++
AGE::AssetRegistry::~AssetRegistry () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Assets/Public/AssetManager.h`

