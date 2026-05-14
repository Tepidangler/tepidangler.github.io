

# Class AGE::AGEFont



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md)








Inherits the following classes: std::enable_shared_from_this< AGEFont >


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEFont**](#function-agefont) (const std::filesystem::path & Font, bool LoadingDefault=false) <br> |
|  uint64\_t | [**GetAssetID**](#function-getassetid) () const<br>_Returns the Asset ID of the object._  |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAtlasTexture**](#function-getatlastexture) () const<br>_Returns the atlas texture reference._  |
|  const std::string & | [**GetFontName**](#function-getfontname) () const<br>_Returns the name of the font used in this object._  |
|  const [**MSDFData**](struct_a_g_e_1_1_m_s_d_f_data.md) \* | [**GetMSDFData**](#function-getmsdfdata) () const<br>_Retrieves the MSDF data associated with this object._  |
|  void | [**LoadFont**](#function-loadfont) (const std::string & FontName) <br> |
|  void | [**SaveFont**](#function-savefont) () <br> |
|   | [**~AGEFont**](#function-agefont) () <br>_Destructor for_ [_**AGEFont**_](class_a_g_e_1_1_a_g_e_font.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetDefault**](#function-getdefault) () <br>_Get the default font instance. If it doesn't exist, create a new one and register it in_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._ |


























## Public Functions Documentation




### function AGEFont 

```C++
AGE::AGEFont::AGEFont (
    const std::filesystem::path & Font,
    bool LoadingDefault=false
) 
```



Constructor for [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) class. It loads a font from the given path and initializes [**MSDFData**](struct_a_g_e_1_1_m_s_d_f_data.md) object with it. The function checks if the provided file exists, initializes FreeType library, loads the font using FreeType, generates glyphs for each character in the charset, packs them into an atlas, applies edge coloring to them, creates a texture from the packed glyphs and caches it. If LoadingDefault is true, it saves the default fonts; otherwise, it saves the custom ones. 

**Parameters:**


* `FontPath` The filesystem path to the font file. 
* `LoadingDefault` Flag indicating whether we are loading default fonts or not. 




        

<hr>



### function GetAssetID 

_Returns the Asset ID of the object._ 
```C++
inline uint64_t AGE::AGEFont::GetAssetID () const
```





**Returns:**

The unique identifier for this asset. 





        

<hr>



### function GetAtlasTexture 

_Returns the atlas texture reference._ 
```C++
inline Ref< Texture2D > AGE::AGEFont::GetAtlasTexture () const
```



This function returns a constant reference to the atlas texture stored in the object. The returned reference can be used to access and manipulate the atlas texture data.




**Returns:**

A constant reference to the atlas texture.


Returns the atlas texture reference. 

**Returns:**

The atlas texture reference. 





        

<hr>



### function GetFontName 

_Returns the name of the font used in this object._ 
```C++
inline const std::string & AGE::AGEFont::GetFontName () const
```





**Returns:**

A constant reference to a string containing the font name. 





        

<hr>



### function GetMSDFData 

_Retrieves the MSDF data associated with this object._ 
```C++
inline const MSDFData * AGE::AGEFont::GetMSDFData () const
```





**Returns:**

A pointer to the MSDF data, or nullptr if no data is available.


Returns the MSDF data associated with this object. 

**Returns:**

Pointer to an immutable [**MSDFData**](struct_a_g_e_1_1_m_s_d_f_data.md) instance, or nullptr if no data is available. 





        

<hr>



### function LoadFont 

```C++
void AGE::AGEFont::LoadFont (
    const std::string & FontName
) 
```




<hr>



### function SaveFont 

```C++
void AGE::AGEFont::SaveFont () 
```




<hr>



### function ~AGEFont 

_Destructor for_ [_**AGEFont**_](class_a_g_e_1_1_a_g_e_font.md) _class._
```C++
AGE::AGEFont::~AGEFont () 
```



This function is responsible for releasing the memory allocated to the data member 'm\_Data' which holds the font data. It does this by deleting the pointer, effectively freeing up the memory space it was using. 


        

<hr>
## Public Static Functions Documentation




### function GetDefault 

_Get the default font instance. If it doesn't exist, create a new one and register it in_ [_**AssetManager**_](class_a_g_e_1_1_asset_manager.md) _._
```C++
static Ref< AGEFont > AGE::AGEFont::GetDefault () 
```





**Returns:**

Ref&lt;AGEFont&gt; A reference to the default font instance. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Font.h`

