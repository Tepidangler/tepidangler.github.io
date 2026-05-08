

# Struct AGE::AssetRegistry



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
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
|   | [**AssetRegistry**](#function-assetregistry-13) ([**AudioManager**](class_a_g_e_1_1_audio_manager.md) \* AudioManagerPtr) <br> |
|   | [**AssetRegistry**](#function-assetregistry-23) (const [**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &) = delete<br> |
|   | [**AssetRegistry**](#function-assetregistry-33) ([**AssetRegistry**](struct_a_g_e_1_1_asset_registry.md) &&) = delete<br> |
|  bool | [**DoesShaderExist**](#function-doesshaderexist) (const std::string & Name) <br> |
|  std::vector&lt; Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; &gt; | [**GetAllScenes**](#function-getallscenes) () <br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetFont**](#function-getfont-22) (const std::string & Name) <br> |
|  const std::vector&lt; std::string &gt; & | [**GetFontNames**](#function-getfontnames) () <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; &gt; & | [**GetFonts**](#function-getfonts) () <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene-22) (const std::string & Name) <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; &gt; & | [**GetScenes**](#function-getscenes) () <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**GetShader**](#function-getshader) (const std::string & Name) <br> |
|  Ref&lt; [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md) &gt; & | [**GetShaders**](#function-getshaders) () <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-12) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & ID) <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**GetSound**](#function-getsound-22) (const std::string & Name) <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &gt; &gt; & | [**GetSoundbanks**](#function-getsoundbanks) () <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; &gt; & | [**GetSounds**](#function-getsounds) () <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-12) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture-22) (const std::string & Name) <br> |
|  std::unordered\_map&lt; [**UUID**](class_a_g_e_1_1_u_u_i_d.md), Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; &gt; & | [**GetTextures**](#function-gettextures) () <br> |
|  bool | [**IsFontLoaded**](#function-isfontloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsSceneLoaded**](#function-issceneloaded) (const std::filesystem::path & Path) <br> |
|  bool | [**IsSoundLoaded**](#function-issoundloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsSoundbankLoaded**](#function-issoundbankloaded) (const std::filesystem::path & Filepath) <br> |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-13) (const std::filesystem::path & Path) <br> |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-23) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|  bool | [**IsTextureLoaded**](#function-istextureloaded-33) (const std::filesystem::path & Path, [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & OutID) <br> |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**LoadFont**](#function-loadfont) (const std::filesystem::path & Filepath) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Filepath) <br> |
|  void | [**LoadShader**](#function-loadshader-13) (const std::string & FilePath) <br> |
|  void | [**LoadShader**](#function-loadshader-23) (const std::string & FilePath1, const std::string & FilePath2) <br> |
|  void | [**LoadShader**](#function-loadshader-33) (const int Name, const std::string & Source) <br> |
|  Ref&lt; [**AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; | [**LoadSound**](#function-loadsound) (const std::filesystem::path & Filepath) <br> |
|  bool | [**LoadSoundbank**](#function-loadsoundbank) (const std::filesystem::path & Filepath) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**LoadTexture**](#function-loadtexture) (const std::filesystem::path & FilePath) <br> |
|  void | [**RegisterFont**](#function-registerfont) (const Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; & font) <br> |
|   | [**~AssetRegistry**](#function-assetregistry) () = default<br> |




























## Public Attributes Documentation




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

```C++
inline AGE::AssetRegistry::AssetRegistry (
    AudioManager * AudioManagerPtr
) 
```




<hr>



### function AssetRegistry [2/3]

```C++
AGE::AssetRegistry::AssetRegistry (
    const AssetRegistry &
) = delete
```




<hr>



### function AssetRegistry [3/3]

```C++
AGE::AssetRegistry::AssetRegistry (
    AssetRegistry &&
) = delete
```




<hr>



### function DoesShaderExist 

```C++
inline bool AGE::AssetRegistry::DoesShaderExist (
    const std::string & Name
) 
```




<hr>



### function GetAllScenes 

```C++
inline std::vector< Ref< Scene > > AGE::AssetRegistry::GetAllScenes () 
```




<hr>



### function GetFont [1/2]

```C++
inline Ref< AGEFont > AGE::AssetRegistry::GetFont (
    const UUID & ID
) 
```




<hr>



### function GetFont [2/2]

```C++
inline Ref< AGEFont > AGE::AssetRegistry::GetFont (
    const std::string & Name
) 
```




<hr>



### function GetFontNames 

```C++
inline const std::vector< std::string > & AGE::AssetRegistry::GetFontNames () 
```




<hr>



### function GetFonts 

```C++
inline std::unordered_map< UUID , Ref< AGEFont > > & AGE::AssetRegistry::GetFonts () 
```




<hr>



### function GetScene [1/2]

```C++
inline Ref< Scene > AGE::AssetRegistry::GetScene (
    const UUID ID
) 
```




<hr>



### function GetScene [2/2]

```C++
inline Ref< Scene > AGE::AssetRegistry::GetScene (
    const std::string & Name
) 
```




<hr>



### function GetScenes 

```C++
inline std::unordered_map< UUID , Ref< Scene > > & AGE::AssetRegistry::GetScenes () 
```




<hr>



### function GetShader 

```C++
inline Ref< Shader > AGE::AssetRegistry::GetShader (
    const std::string & Name
) 
```




<hr>



### function GetShaders 

```C++
inline Ref< ShaderLibrary > & AGE::AssetRegistry::GetShaders () 
```




<hr>



### function GetSound [1/2]

```C++
inline Ref< AudioSource > AGE::AssetRegistry::GetSound (
    const UUID & ID
) 
```




<hr>



### function GetSound [2/2]

```C++
inline Ref< AudioSource > AGE::AssetRegistry::GetSound (
    const std::string & Name
) 
```




<hr>



### function GetSoundbanks 

```C++
inline std::unordered_map< UUID , Ref< SoundBank > > & AGE::AssetRegistry::GetSoundbanks () 
```




<hr>



### function GetSounds 

```C++
inline std::unordered_map< UUID , Ref< AudioSource > > & AGE::AssetRegistry::GetSounds () 
```




<hr>



### function GetTexture [1/2]

```C++
inline Ref< Texture2D > AGE::AssetRegistry::GetTexture (
    UUID ID
) 
```




<hr>



### function GetTexture [2/2]

```C++
inline Ref< Texture2D > AGE::AssetRegistry::GetTexture (
    const std::string & Name
) 
```




<hr>



### function GetTextures 

```C++
inline std::unordered_map< UUID , Ref< Texture2D > > & AGE::AssetRegistry::GetTextures () 
```




<hr>



### function IsFontLoaded 

```C++
inline bool AGE::AssetRegistry::IsFontLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsSceneLoaded 

```C++
inline bool AGE::AssetRegistry::IsSceneLoaded (
    const std::filesystem::path & Path
) 
```




<hr>



### function IsSoundLoaded 

```C++
inline bool AGE::AssetRegistry::IsSoundLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsSoundbankLoaded 

```C++
inline bool AGE::AssetRegistry::IsSoundbankLoaded (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function IsTextureLoaded [1/3]

```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const std::filesystem::path & Path
) 
```




<hr>



### function IsTextureLoaded [2/3]

```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const UUID ID
) 
```




<hr>



### function IsTextureLoaded [3/3]

```C++
inline bool AGE::AssetRegistry::IsTextureLoaded (
    const std::filesystem::path & Path,
    UUID & OutID
) 
```




<hr>



### function LoadFont 

```C++
inline Ref< AGEFont > AGE::AssetRegistry::LoadFont (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadScene 

```C++
inline Ref< Scene > AGE::AssetRegistry::LoadScene (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadShader [1/3]

```C++
inline void AGE::AssetRegistry::LoadShader (
    const std::string & FilePath
) 
```




<hr>



### function LoadShader [2/3]

```C++
inline void AGE::AssetRegistry::LoadShader (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```




<hr>



### function LoadShader [3/3]

```C++
inline void AGE::AssetRegistry::LoadShader (
    const int Name,
    const std::string & Source
) 
```




<hr>



### function LoadSound 

```C++
inline Ref< AudioSource > AGE::AssetRegistry::LoadSound (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadSoundbank 

```C++
inline bool AGE::AssetRegistry::LoadSoundbank (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function LoadTexture 

```C++
inline Ref< Texture2D > AGE::AssetRegistry::LoadTexture (
    const std::filesystem::path & FilePath
) 
```




<hr>



### function RegisterFont 

```C++
inline void AGE::AssetRegistry::RegisterFont (
    const Ref< AGEFont > & font
) 
```




<hr>



### function ~AssetRegistry 

```C++
AGE::AssetRegistry::~AssetRegistry () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Assets/Public/AssetManager.h`

