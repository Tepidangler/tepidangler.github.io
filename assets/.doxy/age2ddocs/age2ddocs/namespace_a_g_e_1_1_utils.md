

# Namespace AGE::Utils



[**Namespace List**](namespaces.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Utils**](namespace_a_g_e_1_1_utils.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**EngineStatics**](class_a_g_e_1_1_utils_1_1_engine_statics.md) <br> |
























## Public Static Functions

| Type | Name |
| ---: | :--- |
|  GLenum | [**AGEImageFormatToGLDataFormat**](#function-ageimageformattogldataformat) (ImageFormat Format) <br> |
|  GLenum | [**AGEImageFormatToGLInternalFormat**](#function-ageimageformattoglinternalformat) (ImageFormat Format) <br> |
|  GLenum | [**AGETextureFormatToGL**](#function-agetextureformattogl) (FramebufferTextureFormat Format) <br> |
|  void | [**AttachColorTexture**](#function-attachcolortexture) (uint32\_t ID, int Samples, GLenum InternalFormat, GLenum Format, uint32\_t Width, uint32\_t Height, int Index) <br> |
|  void | [**AttachDepthTexture**](#function-attachdepthtexture) (uint32\_t ID, int Samples, GLenum Format, GLenum AttachmentType, uint32\_t Width, uint32\_t Height) <br> |
|  void | [**BindTexture**](#function-bindtexture) (bool Multisampled, uint32\_t ID) <br> |
|  std::string | [**ConvertAPIToString**](#function-convertapitostring) () <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, bool Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int16\_t Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int64\_t Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint16\_t Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint32\_t Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint64\_t Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector2**](struct_a_g_e_1_1_vector2.md) Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector3**](struct_a_g_e_1_1_vector3.md) Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector4**](struct_a_g_e_1_1_vector4.md) Value) <br> |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, float Value) <br> |
|  void | [**CreateTextures**](#function-createtextures) (bool Multisampled, uint32\_t \* OutID, uint32\_t Count) <br> |
|  bool | [**IsDepthFormat**](#function-isdepthformat) (FramebufferTextureFormat Format) <br> |
|  GLenum | [**TextureTarget**](#function-texturetarget) (bool Multisampled) <br> |


























## Public Static Functions Documentation




### function AGEImageFormatToGLDataFormat 

```C++
static GLenum AGE::Utils::AGEImageFormatToGLDataFormat (
    ImageFormat Format
) 
```




<hr>



### function AGEImageFormatToGLInternalFormat 

```C++
static GLenum AGE::Utils::AGEImageFormatToGLInternalFormat (
    ImageFormat Format
) 
```




<hr>



### function AGETextureFormatToGL 

```C++
static GLenum AGE::Utils::AGETextureFormatToGL (
    FramebufferTextureFormat Format
) 
```




<hr>



### function AttachColorTexture 

```C++
static void AGE::Utils::AttachColorTexture (
    uint32_t ID,
    int Samples,
    GLenum InternalFormat,
    GLenum Format,
    uint32_t Width,
    uint32_t Height,
    int Index
) 
```




<hr>



### function AttachDepthTexture 

```C++
static void AGE::Utils::AttachDepthTexture (
    uint32_t ID,
    int Samples,
    GLenum Format,
    GLenum AttachmentType,
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function BindTexture 

```C++
static void AGE::Utils::BindTexture (
    bool Multisampled,
    uint32_t ID
) 
```




<hr>



### function ConvertAPIToString 

```C++
static std::string AGE::Utils::ConvertAPIToString () 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    bool Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int16_t Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int64_t Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint16_t Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint32_t Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint64_t Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector2 Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector3 Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector4 Value
) 
```




<hr>



### function ConvertToString 

```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    float Value
) 
```




<hr>



### function CreateTextures 

```C++
static void AGE::Utils::CreateTextures (
    bool Multisampled,
    uint32_t * OutID,
    uint32_t Count
) 
```




<hr>



### function IsDepthFormat 

```C++
static bool AGE::Utils::IsDepthFormat (
    FramebufferTextureFormat Format
) 
```




<hr>



### function TextureTarget 

```C++
static GLenum AGE::Utils::TextureTarget (
    bool Multisampled
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Private/OpenGLFrameBuffer.cpp`

