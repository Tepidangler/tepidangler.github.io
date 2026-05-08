

# Struct AGE::ImageSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) & | [**GetBounds**](#function-getbounds) () <br> |
|  int | [**GetChannels**](#function-getchannels) () <br> |
|  [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) & | [**GetFileData**](#function-getfiledata) () <br> |
|  uint32\_t | [**GetHeight**](#function-getheight-12) () <br> |
|  uint32\_t | [**GetHeight**](#function-getheight-22) () const<br> |
|  PixelType | [**GetPixelType**](#function-getpixeltype-12) () <br> |
|  PixelType | [**GetPixelType**](#function-getpixeltype-22) () const<br> |
|  int | [**GetPixelsPerByte**](#function-getpixelsperbyte) () <br> |
|  [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) & | [**GetSize**](#function-getsize) () <br> |
|  uint32\_t | [**GetWidth**](#function-getwidth-12) () const<br> |
|  uint32\_t | [**GetWidth**](#function-getwidth-22) () <br> |
|  uint32\_t | [**GetWidthBytes**](#function-getwidthbytes) () <br> |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetWidthHeight**](#function-getwidthheight) () <br> |
|   | [**ImageSpecification**](#function-imagespecification-14) () = default<br> |
|   | [**ImageSpecification**](#function-imagespecification-24) (const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) &) = default<br> |
|   | [**ImageSpecification**](#function-imagespecification-34) (uint32\_t width, uint32\_t height, int channels, uint8\_t type, [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) Data) <br> |
|   | [**ImageSpecification**](#function-imagespecification-44) (uint32\_t width, uint32\_t height, uint8\_t type, [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) Data) <br> |
|  void | [**SetBounds**](#function-setbounds) (const [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) & bounds) <br> |
|  void | [**SetChannels**](#function-setchannels) (int channels) <br> |
|  void | [**SetFileData**](#function-setfiledata) (const [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) & Data) <br> |
|  void | [**SetHeight**](#function-setheight) (const uint32\_t height) <br> |
|  void | [**SetPixelType**](#function-setpixeltype) (const PixelType & type) <br> |
|  void | [**SetSize**](#function-setsize) (const [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) & size) <br> |
|  void | [**SetWidth**](#function-setwidth) (const uint32\_t width) <br> |
|  void | [**SetWidthHeight**](#function-setwidthheight) (const std::pair&lt; uint32\_t, uint32\_t &gt; & WidthHeight) <br> |
|   | [**~ImageSpecification**](#function-imagespecification) () = default<br> |




























## Public Functions Documentation




### function GetBounds 

```C++
inline AGERect & AGE::ImageSpecification::GetBounds () 
```




<hr>



### function GetChannels 

```C++
inline int AGE::ImageSpecification::GetChannels () 
```




<hr>



### function GetFileData 

```C++
inline AsepriteFileData & AGE::ImageSpecification::GetFileData () 
```




<hr>



### function GetHeight [1/2]

```C++
inline uint32_t AGE::ImageSpecification::GetHeight () 
```




<hr>



### function GetHeight [2/2]

```C++
inline uint32_t AGE::ImageSpecification::GetHeight () const
```




<hr>



### function GetPixelType [1/2]

```C++
inline PixelType AGE::ImageSpecification::GetPixelType () 
```




<hr>



### function GetPixelType [2/2]

```C++
inline PixelType AGE::ImageSpecification::GetPixelType () const
```




<hr>



### function GetPixelsPerByte 

```C++
inline int AGE::ImageSpecification::GetPixelsPerByte () 
```




<hr>



### function GetSize 

```C++
inline AGESize & AGE::ImageSpecification::GetSize () 
```




<hr>



### function GetWidth [1/2]

```C++
inline uint32_t AGE::ImageSpecification::GetWidth () const
```




<hr>



### function GetWidth [2/2]

```C++
inline uint32_t AGE::ImageSpecification::GetWidth () 
```




<hr>



### function GetWidthBytes 

```C++
inline uint32_t AGE::ImageSpecification::GetWidthBytes () 
```




<hr>



### function GetWidthHeight 

```C++
inline std::pair< uint32_t, uint32_t > AGE::ImageSpecification::GetWidthHeight () 
```




<hr>



### function ImageSpecification [1/4]

```C++
AGE::ImageSpecification::ImageSpecification () = default
```




<hr>



### function ImageSpecification [2/4]

```C++
AGE::ImageSpecification::ImageSpecification (
    const ImageSpecification &
) = default
```




<hr>



### function ImageSpecification [3/4]

```C++
inline AGE::ImageSpecification::ImageSpecification (
    uint32_t width,
    uint32_t height,
    int channels,
    uint8_t type,
    AsepriteFileData Data
) 
```




<hr>



### function ImageSpecification [4/4]

```C++
inline AGE::ImageSpecification::ImageSpecification (
    uint32_t width,
    uint32_t height,
    uint8_t type,
    AsepriteFileData Data
) 
```




<hr>



### function SetBounds 

```C++
inline void AGE::ImageSpecification::SetBounds (
    const AGERect & bounds
) 
```




<hr>



### function SetChannels 

```C++
inline void AGE::ImageSpecification::SetChannels (
    int channels
) 
```




<hr>



### function SetFileData 

```C++
inline void AGE::ImageSpecification::SetFileData (
    const AsepriteFileData & Data
) 
```




<hr>



### function SetHeight 

```C++
inline void AGE::ImageSpecification::SetHeight (
    const uint32_t height
) 
```




<hr>



### function SetPixelType 

```C++
inline void AGE::ImageSpecification::SetPixelType (
    const PixelType & type
) 
```




<hr>



### function SetSize 

```C++
inline void AGE::ImageSpecification::SetSize (
    const AGESize & size
) 
```




<hr>



### function SetWidth 

```C++
inline void AGE::ImageSpecification::SetWidth (
    const uint32_t width
) 
```




<hr>



### function SetWidthHeight 

```C++
inline void AGE::ImageSpecification::SetWidthHeight (
    const std::pair< uint32_t, uint32_t > & WidthHeight
) 
```




<hr>



### function ~ImageSpecification 

```C++
AGE::ImageSpecification::~ImageSpecification () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Image.h`

