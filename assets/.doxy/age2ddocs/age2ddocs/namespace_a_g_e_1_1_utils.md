

# Namespace AGE::Utils



[**Namespace List**](namespaces.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Utils**](namespace_a_g_e_1_1_utils.md)




















## Classes

| Type | Name |
| ---: | :--- |
| class | [**EngineStatics**](class_a_g_e_1_1_utils_1_1_engine_statics.md) <br> |
























## Public Static Functions

| Type | Name |
| ---: | :--- |
|  GLenum | [**AGEImageFormatToGLDataFormat**](#function-ageimageformattogldataformat) (ImageFormat Format) <br>_Converts an ImageFormat to a GLenum data format._  |
|  GLenum | [**AGEImageFormatToGLInternalFormat**](#function-ageimageformattoglinternalformat) (ImageFormat Format) <br>_Converts an ImageFormat to its corresponding GL internal format._  |
|  GLenum | [**AGETextureFormatToGL**](#function-agetextureformattogl) (FramebufferTextureFormat Format) <br>_Converts a FramebufferTextureFormat to its corresponding GLenum._  |
|  void | [**AttachColorTexture**](#function-attachcolortexture) (uint32\_t ID, int Samples, GLenum InternalFormat, GLenum Format, uint32\_t Width, uint32\_t Height, int Index) <br>_Attaches a color texture to the framebuffer._  |
|  void | [**AttachDepthTexture**](#function-attachdepthtexture) (uint32\_t ID, int Samples, GLenum Format, GLenum AttachmentType, uint32\_t Width, uint32\_t Height) <br> |
|  void | [**BindTexture**](#function-bindtexture) (bool Multisampled, uint32\_t ID) <br>_This function binds a texture to the OpenGL context._  |
|  std::string | [**ConvertAPIToString**](#function-convertapitostring) () <br>_Converts the current_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _to a string._ |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, bool Value) <br>_Converts a boolean value to its string representation._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int Value) <br>_Converts an integer value to a string._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int16\_t Value) <br>_Converts a numeric value to string._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, int64\_t Value) <br>_Converts a numeric value to string._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint16\_t Value) <br>_Converts a numeric value to string._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint32\_t Value) <br>_Converts a value of an AGE pin type to its string representation._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, uint64\_t Value) <br>_Converts a value of any type to string._  |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector2**](struct_a_g_e_1_1_vector2.md) Value) <br>_Converts an AGEPinType and a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _to a string._ |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector3**](struct_a_g_e_1_1_vector3.md) Value) <br>_Converts an AGEPinType and a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a string._ |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, [**Vector4**](struct_a_g_e_1_1_vector4.md) Value) <br>_Converts a given AGEPinType and_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to string._ |
|  std::string | [**ConvertToString**](#function-converttostring) (AGEPinType Type, float Value) <br>_Converts a floating-point value to a string._  |
|  void | [**CreateTextures**](#function-createtextures) (bool Multisampled, uint32\_t \* OutID, uint32\_t Count) <br>_Creates a set of textures._  |
|  bool | [**IsDepthFormat**](#function-isdepthformat) (FramebufferTextureFormat Format) <br>_Checks if the given format is a depth format._  |
|  GLenum | [**TextureTarget**](#function-texturetarget) (bool Multisampled) <br>_Determines the OpenGL texture target based on whether multisampling is enabled._  |


























## Public Static Functions Documentation




### function AGEImageFormatToGLDataFormat 

_Converts an ImageFormat to a GLenum data format._ 
```C++
static GLenum AGE::Utils::AGEImageFormatToGLDataFormat (
    ImageFormat Format
) 
```



This function takes in an ImageFormat and returns the corresponding GLenum data format. It uses a switch-case statement to handle different ImageFormats, returning GL\_RGB for RGB8 and GL\_RGBA for RGBA8. If the ImageFormat is not supported by AGE (which should never happen), it asserts false and returns 0.




**Parameters:**


* `Format` The ImageFormat to convert. 



**Returns:**

The corresponding GLenum data format. 





        

<hr>



### function AGEImageFormatToGLInternalFormat 

_Converts an ImageFormat to its corresponding GL internal format._ 
```C++
static GLenum AGE::Utils::AGEImageFormatToGLInternalFormat (
    ImageFormat Format
) 
```



This function takes in an ImageFormat and returns the equivalent GL internal format. It uses a switch-case statement to handle different ImageFormats, returning the appropriate GL\_RGB8 or GL\_RGBA8 based on the input. If the input is not supported by AGE (which should never happen as we only have two defined formats), it asserts false and returns 0.




**Parameters:**


* `Format` The ImageFormat to convert. 



**Returns:**

The corresponding GL internal format, or 0 if the ImageFormat is not supported. 





        

<hr>



### function AGETextureFormatToGL 

_Converts a FramebufferTextureFormat to its corresponding GLenum._ 
```C++
static GLenum AGE::Utils::AGETextureFormatToGL (
    FramebufferTextureFormat Format
) 
```



This function takes in a FramebufferTextureFormat and returns the equivalent GLenum value. It handles four formats: RGBA8, RED\_INTEGER. For any other format, it asserts false and returns 0.




**Parameters:**


* `Format` The FramebufferTextureFormat to convert. 



**Returns:**

The corresponding GLenum for the input FramebufferTextureFormat. If the input is not a recognized format, it will return 0.


Converts a FramebufferTextureFormat to its corresponding GLenum.


This function takes in a FramebufferTextureFormat and returns the equivalent GLenum value. It handles four cases: RGBA8, which corresponds to GL\_RGBA8, RED\_INTEGER, which corresponds to GL\_RED\_INTEGER, and any other format that is not handled by this function results in an assertion failure with a message "Invalid Format".




**Parameters:**


* `Format` The FramebufferTextureFormat to convert. 



**Returns:**

The corresponding GLenum value for the given FramebufferTextureFormat. 





        

<hr>



### function AttachColorTexture 

_Attaches a color texture to the framebuffer._ 
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



This function sets up and attaches a color texture to the OpenGL framebuffer object. The texture can be either multisampled or regular, depending on the 'Samples' parameter. It then binds this texture as a color attachment point for rendering.


Attach a color texture to the framebuffer.


This function attaches a color texture to the OpenGL framebuffer. The texture can be either multisampled or regular. If it's multisampled, we use glTexImage2DMultisample to create the texture with specified samples and internal format. Otherwise, we use glTexImage2D to create a 2D texture with given width, height, and format. We then set various texture parameters such as minification and magnification filters, wrapping modes etc., before attaching it to the framebuffer using glFramebufferTexture2D.




**Parameters:**


* `ID` The OpenGL ID of the texture to attach. 
* `Samples` Number of samples for multisampling (if any). 
* `InternalFormat` The internal format of the texture. 
* `Format` The format of the pixel data. 
* `Width` The width of the texture. 
* `Height` The height of the texture. 
* `Index` The index for color attachment point in framebuffer object. 




        

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



This function is used to attach a depth texture to the frame buffer. It takes in several parameters including the OpenGL ID, number of samples for multisampling, format of the texture data, type of attachment and dimensions of the texture. The function first checks if the texture should be multisampled based on the provided sample count. If it is, a multisample texture image is created using glTexImage2DMultisample. Otherwise, a regular 2D texture storage is created with glTexStorage2D and some basic parameters are set for the texture. Finally, the function attaches the texture to the frame buffer using glFramebufferTexture2D. 


        

<hr>



### function BindTexture 

_This function binds a texture to the OpenGL context._ 
```C++
static void AGE::Utils::BindTexture (
    bool Multisampled,
    uint32_t ID
) 
```



The function takes two parameters, a boolean indicating whether the texture is multisampled and an unsigned integer representing the ID of the texture. It uses these values to determine the appropriate target for binding the texture with glBindTexture().




**Parameters:**


* `Multisampled` A boolean value that indicates if the texture is multisampled or not. 
* `ID` An unsigned integer representing the ID of the texture to be bound.



**Returns:**

void


This function binds a texture to the OpenGL context.


It takes two parameters, one boolean and one unsigned integer. The boolean indicates whether the texture is multisampled or not, while the unsigned integer represents the ID of the texture. The function uses these inputs to determine the correct target for binding the texture using glBindTexture().




**Parameters:**


* `Multisampled` A boolean indicating if the texture is multisampled (true) or not (false). 
* `ID` An unsigned integer representing the ID of the texture.



**Returns:**

void 





        

<hr>



### function ConvertAPIToString 

_Converts the current_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _to a string._
```C++
static std::string AGE::Utils::ConvertAPIToString () 
```



This function converts the enum value of [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) into a human-readable string representation. It uses a switch statement to check the integer equivalent of the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) and returns a corresponding string. If the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is not recognized, it defaults to "UNDEFINED".




**Returns:**

A string representing the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md). Possible values are: "Headless", "OpenGL", or "UNDEFINED" if the API is unknown. 





        

<hr>



### function ConvertToString 

_Converts a boolean value to its string representation._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    bool Value
) 
```



This function takes an AGEPinType and a boolean value as input, converts the boolean value into its string representation ("True" or "False"), and returns it along with the AGEPinType in a formatted string.




**Parameters:**


* `Type` The type of pin to be converted. 
* `Value` The boolean value to be converted. 



**Returns:**

The string representation of the input boolean value.


Converts a boolean value to its string representation.


This function takes an AGEPinType and a boolean value as input, converts the boolean value into its string representation ("True" or "False"), and returns it as a std::string.




**Parameters:**


* `Type` The type of pin that is being converted. This parameter does not contribute to the function's output but is included for context. 
* `Value` The boolean value to be converted into its string representation. 



**Returns:**

A std::string containing "True" if Value is true, and "False" otherwise. 





        

<hr>



### function ConvertToString 

_Converts an integer value to a string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int Value
) 
```



This function takes in two parameters, an AGEPinType and an int Value. It converts the int Value into a string using std::to\_string() and returns it as a std::string. The purpose of this function is to provide a standardized way of converting integer values to strings for use in various parts of the AGE system.




**Parameters:**


* `Type` This parameter represents the type of pin that we are working with, but its actual meaning or functionality within the context of the AGE system is not specified here as it's beyond the scope of this function's documentation. 
* `Value` The integer value to be converted into a string.



**Returns:**

Returns a std::string that represents the input integer Value in textual form. If the conversion fails, an empty string ("") is returned.


Converts an integer value to a string.


This function takes in two parameters, an enumeration of type AGEPinType and an integer Value. It converts the integer into a string representation using std::to\_string() and returns it. The purpose of this conversion is typically for logging or debugging purposes where you might want to display the value as a string instead of its numeric representation.




**Parameters:**


* `Type` An enumeration representing different types of pins. This parameter does not contribute to the functionality of the function, but it provides context about what kind of pin the Value represents. 
* `Value` The integer value that will be converted into a string.



**Returns:**

Returns a std::string representation of the input integer Value. 





        

<hr>



### function ConvertToString 

_Converts a numeric value to string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int16_t Value
) 
```



This function takes an AGEPinType and an int16\_t as input, converts the int16\_t to a string using std::to\_string(), and returns it. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` An enumeration value representing the type of pin being processed. This parameter's role in the function is not clear from the context provided, so its documentation has been left as "Unknown". 
* `Value` A numeric value to be converted to a string.



**Returns:**

The input int16\_t value as a string.


Converts a numeric value to string.


This function takes an AGEPinType and an int16\_t as input, converts the int16\_t to a string using std::to\_string(), and returns this string. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` An enumeration value representing the type of pin being processed. This parameter's role in the function is not clear. 
* `Value` A numeric value to be converted to a string.



**Returns:**

Returns a string representation of the input int16\_t Value. 





        

<hr>



### function ConvertToString 

_Converts a numeric value to string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    int64_t Value
) 
```



This function takes an AGEPinType and an int64\_t as input, converts the int64\_t to a string representation, and returns it. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` - The type of pin being converted. It's not clear what this parameter represents or its significance. 
* `Value` - The numeric value to be converted into a string.



**Returns:**

Returns the string representation of the input int64\_t Value.


Converts a value to string.


This function takes an AGEPinType and an int64\_t as input, converts the int64\_t to a string representation, and returns it. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` - The type of pin being converted. 
* `Value` - The value to be converted to a string. 



**Returns:**

A string representation of the input value. 





        

<hr>



### function ConvertToString 

_Converts a numeric value to string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint16_t Value
) 
```



This function takes an AGEPinType and a uint16\_t as input, converts the uint16\_t to a string representation, and returns it. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` - The type of pin being converted. Not used in the conversion process. 
* `Value` - The numeric value to be converted to a string.



**Returns:**

A string representation of the input uint16\_t value.


Converts a numeric value to string.


This function takes an AGEPinType and a uint16\_t as input, converts the uint16\_t to a string representation, and returns it. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` - The type of pin being converted. It's not clear what this parameter represents or its significance. 
* `Value` - The numeric value to be converted to a string.



**Returns:**

Returns the string representation of the input uint16\_t value. 





        

<hr>



### function ConvertToString 

_Converts a value of an AGE pin type to its string representation._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint32_t Value
) 
```



This function takes in the type of the AGE pin and its corresponding value, converts the value into a string representation using std::to\_string() and returns it.




**Parameters:**


* `Type` The type of the AGE pin (not used in this conversion but included for completeness). 
* `Value` The value to be converted to a string. 



**Returns:**

Returns the string representation of the input value.


Converts a numeric value to string.


This function takes an AGEPinType and a uint32\_t as input, converts the latter to a string representation, and returns it. The conversion is done using std::to\_string() function from C++ standard library.




**Parameters:**


* `Type` - The type of pin being converted. This parameter does not contribute to the functionality of this function. 
* `Value` - The numeric value to be converted to a string.



**Returns:**

Returns a string representation of the input uint32\_t value. 





        

<hr>



### function ConvertToString 

_Converts a value of any type to string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    uint64_t Value
) 
```



This function takes an AGEPinType and a uint64\_t as input, converts the uint64\_t to a string representation, and returns it. The conversion is done based on the provided AGEPinType which can be used for further processing or presentation of the value.




**Parameters:**


* `Type` - The type of pin that needs to be converted. This parameter does not contribute to the actual conversion but provides context about what kind of representation is expected from the function. 
* `Value` - The uint64\_t value which needs to be converted to string.



**Returns:**

Returns a string representation of the input uint64\_t value.


Converts a value to string.


This function takes an AGEPinType and a uint64\_t as input, converts the uint64\_t to a string representation, and returns it. The conversion is done based on the provided AGEPinType which can be used for further processing or display purposes.




**Parameters:**


* `Type` - The type of pin that we are converting from. 
* `Value` - The value of the pin that we want to convert into a string.



**Returns:**

Returns a string representation of the input uint64\_t value. 





        

<hr>



### function ConvertToString 

_Converts an AGEPinType and a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _to a string._
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector2 Value
) 
```



This function takes in an AGEPinType and a [**Vector2**](struct_a_g_e_1_1_vector2.md) as parameters, converts the [**Vector2**](struct_a_g_e_1_1_vector2.md) to a string using static\_cast, then returns this string. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` The type of pin being converted. 
* `Value` The value of the pin being converted. 



**Returns:**

A string representation of the input parameters.


Converts a given AGEPinType and [**Vector2**](struct_a_g_e_1_1_vector2.md) value to string.


This function takes an AGEPinType and a [**Vector2**](struct_a_g_e_1_1_vector2.md) as input, converts the [**Vector2**](struct_a_g_e_1_1_vector2.md) value to string format using static\_cast, then returns this converted string. The returned string is empty if the conversion fails.




**Parameters:**


* `Type` The type of pin that needs to be converted. 
* `Value` The value of the pin that needs to be converted. 



**Returns:**

A string representation of the input [**Vector2**](struct_a_g_e_1_1_vector2.md) value, or an empty string if the conversion failed. 





        

<hr>



### function ConvertToString 

_Converts an AGEPinType and a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a string._
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector3 Value
) 
```



This function takes in two parameters, an AGEPinType and a [**Vector3**](struct_a_g_e_1_1_vector3.md). It converts the [**Vector3**](struct_a_g_e_1_1_vector3.md) to a string using the `std::string` constructor and returns it. The conversion is done by simply casting the [**Vector3**](struct_a_g_e_1_1_vector3.md) object to a std::string.




**Parameters:**


* `Type` The type of pin that we are converting. 
* `Value` The value of the pin, represented as a [**Vector3**](struct_a_g_e_1_1_vector3.md).



**Returns:**

A string representation of the input parameters.


Converts a given AGEPinType and [**Vector3**](struct_a_g_e_1_1_vector3.md) value to string.


This function takes an AGEPinType and a [**Vector3**](struct_a_g_e_1_1_vector3.md) as input, converts the [**Vector3**](struct_a_g_e_1_1_vector3.md) into a string representation, and returns it along with the AGEPinType in string format.




**Parameters:**


* `Type` The type of pin that needs to be converted to string. 
* `Value` The value of the pin that needs to be converted to string. 



**Returns:**

Returns the string representation of the input values. 





        

<hr>



### function ConvertToString 

_Converts a given AGEPinType and_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to string._
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    Vector4 Value
) 
```



This function takes an AGEPinType and a [**Vector4**](struct_a_g_e_1_1_vector4.md) as input, converts the [**Vector4**](struct_a_g_e_1_1_vector4.md) to a string representation, and returns it along with the AGEPinType. The conversion is done by simply casting the [**Vector4**](struct_a_g_e_1_1_vector4.md) to a std::string.




**Parameters:**


* `Type` The type of pin that we are converting. 
* `Value` The value of the pin in [**Vector4**](struct_a_g_e_1_1_vector4.md) format. 



**Returns:**

Returns the string representation of the input [**Vector4**](struct_a_g_e_1_1_vector4.md) along with the AGEPinType.


Converts a given AGEPinType and [**Vector4**](struct_a_g_e_1_1_vector4.md) to string.


This function takes an AGEPinType and a [**Vector4**](struct_a_g_e_1_1_vector4.md) as input, converts the [**Vector4**](struct_a_g_e_1_1_vector4.md) to a string using static\_cast, and returns this string. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` The type of pin that we are converting. 
* `Value` The value of the pin that we are converting.



**Returns:**

Returns the converted string representation of the [**Vector4**](struct_a_g_e_1_1_vector4.md) input. 





        

<hr>



### function ConvertToString 

_Converts a floating-point value to a string._ 
```C++
static std::string AGE::Utils::ConvertToString (
    AGEPinType Type,
    float Value
) 
```



This function takes an AGEPinType and a float as input, converts the float to a string using std::to\_string(), and returns this string. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` An enumeration value representing the type of pin being processed. This parameter's role in the function is not clear from the context provided. 
* `Value` A floating-point number to be converted to a string.



**Returns:**

The float value as a string. If an error occurs during conversion, it returns an empty string.


Converts a floating-point value to a string.


This function takes an AGEPinType and a float as input, converts the float to a string using std::to\_string(), and returns this string. The purpose of this conversion is unknown at present.




**Parameters:**


* `Type` An enum representing different types of pins in the system. It's not clear what this parameter represents or its significance. 
* `Value` A floating-point value to be converted to a string.



**Returns:**

The float value as a string. 





        

<hr>



### function CreateTextures 

_Creates a set of textures._ 
```C++
static void AGE::Utils::CreateTextures (
    bool Multisampled,
    uint32_t * OutID,
    uint32_t Count
) 
```



This function creates a set of OpenGL textures using the glCreateTextures function. The number of textures to be created is specified by 'Count'. The parameter 'Multisampled' determines whether the textures are multisampled or not, and 'OutID' is an array that will hold the IDs of the newly created textures.




**Parameters:**


* `Multisampled` A boolean value indicating if the textures should be multisampled. 
* `OutID` An array to store the IDs of the newly created textures. 
* `Count` The number of textures to create.



**Returns:**

void


Creates a set of textures.


This function creates a set of OpenGL textures with the specified parameters. The number of textures to be created is given by 'Count'. If 'Multisampled' is true, multisampling will be used for the textures; otherwise, they won't. The IDs of the newly created textures are stored in the array pointed to by 'OutID'.




**Parameters:**


* `Multisampled` A boolean indicating whether or not to use multisampling. 
* `OutID` An array that will store the IDs of the newly created textures. 
* `Count` The number of textures to be created. 




        

<hr>



### function IsDepthFormat 

_Checks if the given format is a depth format._ 
```C++
static bool AGE::Utils::IsDepthFormat (
    FramebufferTextureFormat Format
) 
```



This function checks whether the provided FramebufferTextureFormat is one of the depth formats. It returns true for DEPTH24STENCIL8 and false otherwise.




**Parameters:**


* `Format` The format to check. 



**Returns:**

True if the format is a depth format, false otherwise.


Checks if the given format is a depth format.


This function checks whether the provided FramebufferTextureFormat is one of the depth formats. The only depth format currently supported by this application is DEPTH24STENCIL8.




**Parameters:**


* `Format` The format to check. 



**Returns:**

True if the format is a depth format, false otherwise. 





        

<hr>



### function TextureTarget 

_Determines the OpenGL texture target based on whether multisampling is enabled._ 
```C++
static GLenum AGE::Utils::TextureTarget (
    bool Multisampled
) 
```



This function takes a boolean parameter indicating if multisampling should be used. If true, it returns GL\_TEXTURE\_2D\_MULTISAMPLE; otherwise, it returns GL\_TEXTURE\_2D.




**Parameters:**


* `Multisampled` A boolean value indicating whether to use multisampling or not. 



**Returns:**

The OpenGL texture target corresponding to the input parameter.


Determines the OpenGL texture target based on whether multisampling is enabled.


This function takes a boolean parameter indicating if multisampling should be used. If true, it returns GL\_TEXTURE\_2D\_MULTISAMPLE; otherwise, it returns GL\_TEXTURE\_2D.




**Parameters:**


* `Multisampled` A boolean value indicating whether to use multisampling or not. 



**Returns:**

The OpenGL texture target based on the input parameter. Returns GL\_TEXTURE\_2D if false is passed and GL\_TEXTURE\_2D\_MULTISAMPLE if true is passed. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Private/OpenGLFrameBuffer.cpp`

