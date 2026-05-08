

# Class AGE::AGEFont



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md)








Inherits the following classes: std::enable_shared_from_this< AGEFont >


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEFont**](#function-agefont) (const std::filesystem::path & Font, bool LoadingDefault=false) <br> |
|  uint64\_t | [**GetAssetID**](#function-getassetid) () const<br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetAtlasTexture**](#function-getatlastexture) () const<br> |
|  const std::string & | [**GetFontName**](#function-getfontname) () const<br> |
|  const [**MSDFData**](struct_a_g_e_1_1_m_s_d_f_data.md) \* | [**GetMSDFData**](#function-getmsdfdata) () const<br> |
|  void | [**LoadFont**](#function-loadfont) (const std::string & FontName) <br> |
|  void | [**SaveFont**](#function-savefont) () <br> |
|   | [**~AGEFont**](#function-agefont) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**AGEFont**](class_a_g_e_1_1_a_g_e_font.md) &gt; | [**GetDefault**](#function-getdefault) () <br> |


























## Public Functions Documentation




### function AGEFont 

```C++
AGE::AGEFont::AGEFont (
    const std::filesystem::path & Font,
    bool LoadingDefault=false
) 
```




<hr>



### function GetAssetID 

```C++
inline uint64_t AGE::AGEFont::GetAssetID () const
```




<hr>



### function GetAtlasTexture 

```C++
inline Ref< Texture2D > AGE::AGEFont::GetAtlasTexture () const
```




<hr>



### function GetFontName 

```C++
inline const std::string & AGE::AGEFont::GetFontName () const
```




<hr>



### function GetMSDFData 

```C++
inline const MSDFData * AGE::AGEFont::GetMSDFData () const
```




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

```C++
AGE::AGEFont::~AGEFont () 
```




<hr>
## Public Static Functions Documentation




### function GetDefault 

```C++
static Ref< AGEFont > AGE::AGEFont::GetDefault () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Font.h`

