

# Class AGE::AssetManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AssetManager**](class_a_g_e_1_1_asset_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AssetManager**](#function-assetmanager-13) () = default<br> |
|   | [**AssetManager**](#function-assetmanager-23) (const std::filesystem::path & GameContentPath) <br> |
|   | [**AssetManager**](#function-assetmanager-33) (void \* AddrToPakFile, size\_t SizeOfPakFile=0) <br> |
|  bool | [**DoesShaderExist**](#function-doesshaderexist) (const std::string & Name) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAsepriteTexture**](#function-getasepritetexture-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAsepriteTexture**](#function-getasepritetexture-22) (const std::string & Name) <br> |
|  Ref&lt; [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &gt; | [**GetAssetRegistry**](#function-getassetregistry) () const<br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-22) (const std::string & Name) <br> |
|  std::filesystem::path & | [**GetGameContentPath**](#function-getgamecontentpath) () <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-22) (const std::string & Name) <br> |
|  void | [**GetSceneNames**](#function-getscenenames) (std::vector&lt; std::string &gt; & OutArray) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**GetShader**](#function-getshader) (const std::string & Name) <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-22) (const std::string & Name) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-12) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-22) (const std::string & Name) <br>_Much slower option considering I had to implement the find function for this myself, however in the event that you don't know the ID for the particular texture you want to load you can search for it based on the name which == the filename._  |
|  bool | [**IsAsepriteFileLoaded**](#function-isasepritefileloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsFontLoaded**](#function-isfontloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsSceneLoaded**](#function-issceneloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsSoundLoaded**](#function-issoundloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsSoundbankLoaded**](#function-issoundbankloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsTextureLoaded**](#function-istextureloaded) (const std::filesystem::path & Filepath) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadAsepriteFile**](#function-loadasepritefile) (const std::filesystem::path & Filepath) <br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**LoadFont**](#function-loadfont) (const std::filesystem::path & Filepath) <br> |
|  bool | [**LoadPakFile**](#function-loadpakfile) (void \* AddrToPakFile, size\_t SizeOfPakFile=0) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Filepath) <br> |
|  void | [**LoadShader**](#function-loadshader-13) (const std::string & FilePath) <br> |
|  void | [**LoadShader**](#function-loadshader-23) (const std::string & FilePath1, const std::string & FilePath2) <br> |
|  void | [**LoadShader**](#function-loadshader-33) (const int Name, const std::string & Source) <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**LoadSound**](#function-loadsound) (const std::filesystem::path & Filepath) <br> |
|  void | [**LoadSoundbank**](#function-loadsoundbank) (const std::filesystem::path & Filepath) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture-12) (const std::filesystem::path & FilePath) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture-22) (void \* Addr, size\_t Size) <br> |
|  void | [**RegisterAsset**](#function-registerasset) (Ref&lt; T &gt; Asset) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**AssetManager**](class_a_g_e_1_1_asset_manager.md) & | [**Get**](#function-get) () <br> |


























## Public Functions Documentation




### function AssetManager [1/3]

```C++
AGE::AssetManager::AssetManager () = default
```




<hr>



### function AssetManager [2/3]

```C++
AGE::AssetManager::AssetManager (
    const std::filesystem::path & GameContentPath
) 
```




<hr>



### function AssetManager [3/3]

```C++
AGE::AssetManager::AssetManager (
    void * AddrToPakFile,
    size_t SizeOfPakFile=0
) 
```




<hr>



### function DoesShaderExist 

```C++
bool AGE::AssetManager::DoesShaderExist (
    const std::string & Name
) 
```




<hr>



### function GetAsepriteTexture [1/2]

```C++
Ref< Texture2D > AGE::AssetManager::GetAsepriteTexture (
    const UUID & ID
) 
```




<hr>



### function GetAsepriteTexture [2/2]

```C++
Ref< Texture2D > AGE::AssetManager::GetAsepriteTexture (
    const std::string & Name
) 
```




<hr>



### function GetAssetRegistry 

```C++
inline Ref< AssetRegistry > AGE::AssetManager::GetAssetRegistry () const
```




<hr>



### function GetFont [1/2]

```C++
Ref< AGEFont > AGE::AssetManager::GetFont (
    const UUID & ID
) 
```




<hr>



### function GetFont [2/2]

```C++
Ref< AGEFont > AGE::AssetManager::GetFont (
    const std::string & Name
) 
```




<hr>



### function GetGameContentPath 

```C++
inline std::filesystem::path & AGE::AssetManager::GetGameContentPath () 
```




<hr>



### function GetScene [1/2]

```C++
Ref< Scene > AGE::AssetManager::GetScene (
    const UUID & ID
) 
```




<hr>



### function GetScene [2/2]

```C++
Ref< Scene > AGE::AssetManager::GetScene (
    const std::string & Name
) 
```




<hr>



### function GetSceneNames 

```C++
void AGE::AssetManager::GetSceneNames (
    std::vector< std::string > & OutArray
) 
```




<hr>



### function GetShader 

```C++
Ref< Shader > AGE::AssetManager::GetShader (
    const std::string & Name
) 
```




<hr>



### function GetSound [1/2]

```C++
Ref< AudioSource > AGE::AssetManager::GetSound (
    const UUID & ID
) 
```




<hr>



### function GetSound [2/2]

```C++
Ref< AudioSource > AGE::AssetManager::GetSound (
    const std::string & Name
) 
```




<hr>



### function GetTexture [1/2]

```C++
Ref< Texture2D > AGE::AssetManager::GetTexture (
    UUID ID
) 
```




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




        

<hr>



### function IsAsepriteFileLoaded 

```C++
bool AGE::AssetManager::IsAsepriteFileLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsFontLoaded 

```C++
bool AGE::AssetManager::IsFontLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsSceneLoaded 

```C++
bool AGE::AssetManager::IsSceneLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsSoundLoaded 

```C++
bool AGE::AssetManager::IsSoundLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsSoundbankLoaded 

```C++
bool AGE::AssetManager::IsSoundbankLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsTextureLoaded 

```C++
bool AGE::AssetManager::IsTextureLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadAsepriteFile 

```C++
Ref< Texture2D > AGE::AssetManager::LoadAsepriteFile (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadFont 

```C++
Ref< AGEFont > AGE::AssetManager::LoadFont (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadPakFile 

```C++
bool AGE::AssetManager::LoadPakFile (
    void * AddrToPakFile,
    size_t SizeOfPakFile=0
) 
```




<hr>



### function LoadScene 

```C++
Ref< Scene > AGE::AssetManager::LoadScene (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadShader [1/3]

```C++
void AGE::AssetManager::LoadShader (
    const std::string & FilePath
) 
```




<hr>



### function LoadShader [2/3]

```C++
void AGE::AssetManager::LoadShader (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```




<hr>



### function LoadShader [3/3]

```C++
void AGE::AssetManager::LoadShader (
    const int Name,
    const std::string & Source
) 
```




<hr>



### function LoadSound 

```C++
Ref< AudioSource > AGE::AssetManager::LoadSound (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadSoundbank 

```C++
void AGE::AssetManager::LoadSoundbank (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadTexture [1/2]

```C++
Ref< Texture2D > AGE::AssetManager::LoadTexture (
    const std::filesystem::path & FilePath
) 
```




<hr>



### function LoadTexture [2/2]

```C++
Ref< Texture2D > AGE::AssetManager::LoadTexture (
    void * Addr,
    size_t Size
) 
```




<hr>



### function RegisterAsset 

```C++
template<typename T>
inline void AGE::AssetManager::RegisterAsset (
    Ref< T > Asset
) 
```




<hr>
## Public Static Functions Documentation




### function Get 

```C++
static inline AssetManager & AGE::AssetManager::Get () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Assets/Public/AssetManager.h`

