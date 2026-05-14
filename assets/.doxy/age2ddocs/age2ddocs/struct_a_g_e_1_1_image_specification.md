

# Struct AGE::ImageSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md)



_Constructor for_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._[More...](#detailed-description)

* `#include <Image.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) & | [**GetBounds**](#function-getbounds) () <br>_Gets the bounds of an object._  |
|  int | [**GetChannels**](#function-getchannels) () <br>_Returns the number of channels in use by the system._  |
|  [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) & | [**GetFileData**](#function-getfiledata) () <br>_Returns the_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file data._ |
|  uint32\_t | [**GetHeight**](#function-getheight-12) () <br>_This function returns the height of an object._  |
|  uint32\_t | [**GetHeight**](#function-getheight-22) () const<br>_Returns the height of an object._  |
|  PixelType | [**GetPixelType**](#function-getpixeltype-12) () <br>_This function returns the type of a pixel._  |
|  PixelType | [**GetPixelType**](#function-getpixeltype-22) () const<br>_Returns the type of pixel represented by this object._  |
|  int | [**GetPixelsPerByte**](#function-getpixelsperbyte) () <br>_This function returns the number of pixels per byte._  |
|  [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) & | [**GetSize**](#function-getsize) () <br>_This function returns the size of an object._  |
|  uint32\_t | [**GetWidth**](#function-getwidth-12) () const<br>_Returns the width of an object._  |
|  uint32\_t | [**GetWidth**](#function-getwidth-22) () <br>_Returns the width of an object._  |
|  uint32\_t | [**GetWidthBytes**](#function-getwidthbytes) () <br>_This function returns the width of an image in bytes. The bit depth (bpp) is determined by the PixelType of the image. If the PixelType is RGBA, then bpp is 32; if it's RGB, then bpp is 24; for Greyscale and Indexed pixel types, bpp is 8. For any other unrecognized PixelType, a warning message is logged to inform user that the default value of bpp (RGBA) is being used._  |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetWidthHeight**](#function-getwidthheight) () <br>_This function returns a pair of integers representing the width and height._  |
|   | [**ImageSpecification**](#function-imagespecification-14) () = default<br>_Default constructor for_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._ |
|   | [**ImageSpecification**](#function-imagespecification-24) (const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) &) = default<br>_Default copy constructor for the_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._ |
|  Unknown | [**ImageSpecification**](#function-imagespecification-34) (uint32\_t width, uint32\_t height, int channels, uint8\_t type, [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) Data) <br> |
|   | [**ImageSpecification**](#function-imagespecification-44) (uint32\_t width, uint32\_t height, uint8\_t type, [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) Data) <br>_Constructs an_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _object with the given parameters._ |
|  void | [**SetBounds**](#function-setbounds) (const [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) & bounds) <br>_Sets the bounds of an object._  |
|  void | [**SetChannels**](#function-setchannels) (int channels) <br>_Sets the number of audio channels to be processed by the system._  |
|  void | [**SetFileData**](#function-setfiledata) (const [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) & Data) <br>_Sets the file data for the_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _object._ |
|  void | [**SetHeight**](#function-setheight) (const uint32\_t height) <br>_Sets the height of an object._  |
|  void | [**SetPixelType**](#function-setpixeltype) (const PixelType & type) <br>_Sets the pixel type of an object._  |
|  void | [**SetSize**](#function-setsize) (const [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) & size) <br>_Sets the size of an object._  |
|  void | [**SetWidth**](#function-setwidth) (const uint32\_t width) <br>_Sets the width of an object._  |
|  void | [**SetWidthHeight**](#function-setwidthheight) (const std::pair&lt; uint32\_t, uint32\_t &gt; & WidthHeight) <br>_Sets the width and height of an object using a pair of unsigned integers._  |
|   | [**~ImageSpecification**](#function-imagespecification) () = default<br>_Destructor for the_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._ |




























## Detailed Description


This function initializes an instance of the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class with given width, height, channels, type and data. It takes in five parameters - width (uint32\_t), height (uint32\_t), channels (int), type (uint8\_t) and Data ([**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md)). The function sets the Width, Height, Channels, Type, Size and FileData accordingly. It also handles the initialization of PixelsPerByte based on the type. 


    
## Public Functions Documentation




### function GetBounds 

_Gets the bounds of an object._ 
```C++
inline AGERect & AGE::ImageSpecification::GetBounds () 
```



This function returns a reference to the 'Bounds' variable, which represents the boundaries of the object. The returned value can be modified using assignment operators if required.




**Returns:**

A reference to the Bounds variable.


Gets the bounds of an object.


This function returns a reference to the 'Bounds' variable, which represents the boundaries of the object. The returned value can be modified using assignment operators if required.




**Returns:**

A reference to the Bounds object. 





        

<hr>



### function GetChannels 

_Returns the number of channels in use by the system._ 
```C++
inline int AGE::ImageSpecification::GetChannels () 
```



This function retrieves the current count of active channels in the system. It is used to manage resources and ensure efficient operation.




**Returns:**

int - The number of active channels. If no channels are available, it returns 0.


Returns the number of channels in use by the system.


This function returns an integer representing the current number of channels being used by the system. It does not take any parameters and has no side effects.




**Returns:**

int The number of active channels. If there are no active channels, it will return 0. 





        

<hr>



### function GetFileData 

_Returns the_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file data._
```C++
inline AsepriteFileData & AGE::ImageSpecification::GetFileData () 
```



This function returns a reference to the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file data object, which contains all the information about the loaded [**Aseprite**](class_a_g_e_1_1_aseprite.md) file.




**Returns:**

A reference to the [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) object.


Returns the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file data.


This function returns a reference to the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file data object, which contains all the information about the loaded [**Aseprite**](class_a_g_e_1_1_aseprite.md) file.




**Returns:**

A reference to the [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) object. 





        

<hr>



### function GetHeight [1/2]

_This function returns the height of an object._ 
```C++
inline uint32_t AGE::ImageSpecification::GetHeight () 
```





**Returns:**

The current height value as a uint32\_t.


Returns the height of an object.


This function retrieves and returns the current height value stored in the 'Height' variable. It does not take any parameters and has no side effects.




**Returns:**

The current height as a 32-bit unsigned integer. 





        

<hr>



### function GetHeight [2/2]

_Returns the height of an object._ 
```C++
inline uint32_t AGE::ImageSpecification::GetHeight () const
```



This function is used to get the current height value of an object. It does not take any parameters and returns a uint32\_t representing the height.




**Returns:**

The current height as a uint32\_t. If no height has been set, it will return 0.


This function returns the height of an object. 

**Returns:**

uint32\_t The height of the object in units as per the scale defined by the implementation. 





        

<hr>



### function GetPixelType [1/2]

_This function returns the type of a pixel._ 
```C++
inline PixelType AGE::ImageSpecification::GetPixelType () 
```





**Returns:**

PixelType The type of the pixel (e.g., RGB, Grayscale).


Returns the type of pixel represented by this object. 

**Returns:**

The PixelType enum value representing the type of pixel. 





        

<hr>



### function GetPixelType [2/2]

_Returns the type of pixel represented by this object._ 
```C++
inline PixelType AGE::ImageSpecification::GetPixelType () const
```





**Returns:**

The PixelType enum value representing the type of pixel.


Returns the type of pixel represented by this object. 

**Returns:**

The PixelType enum value representing the type of pixel. 





        

<hr>



### function GetPixelsPerByte 

_This function returns the number of pixels per byte._ 
```C++
inline int AGE::ImageSpecification::GetPixelsPerByte () 
```





**Returns:**

int The number of pixels per byte. If no value is set, it will return -1.


This function returns the number of pixels per byte. 

**Returns:**

The number of pixels per byte as an integer. 





        

<hr>



### function GetSize 

_This function returns the size of an object._ 
```C++
inline AGESize & AGE::ImageSpecification::GetSize () 
```





**Returns:**

A reference to the Size variable.


Gets the size of an object.


This function returns a reference to the 'Size' variable, which represents the size of an object. The returned value can be modified using other functions if necessary.




**Returns:**

A reference to the Size variable. 





        

<hr>



### function GetWidth [1/2]

_Returns the width of an object._ 
```C++
inline uint32_t AGE::ImageSpecification::GetWidth () const
```



This function returns the current width value stored in the 'Width' variable. It is a getter method for the 'Width' attribute.




**Returns:**

uint32\_t The current width of the object.


Returns the width of an object. 

**Returns:**

The width as a uint32\_t value. 





        

<hr>



### function GetWidth [2/2]

_Returns the width of an object._ 
```C++
inline uint32_t AGE::ImageSpecification::GetWidth () 
```





**Returns:**

The width as a uint32\_t value.


This function returns the width of an object. 

**Returns:**

The width as a uint32\_t value. 





        

<hr>



### function GetWidthBytes 

_This function returns the width of an image in bytes. The bit depth (bpp) is determined by the PixelType of the image. If the PixelType is RGBA, then bpp is 32; if it's RGB, then bpp is 24; for Greyscale and Indexed pixel types, bpp is 8. For any other unrecognized PixelType, a warning message is logged to inform user that the default value of bpp (RGBA) is being used._ 
```C++
inline uint32_t AGE::ImageSpecification::GetWidthBytes () 
```





**Returns:**

The width of the image in bytes. This is calculated by multiplying the Width of the image with its bit depth per pixel (bpp).


This function returns the width of an image in bytes. The bits per pixel (bpp) is determined by the PixelType of the image. 

**Returns:**

uint32\_t Returns the width of the image in bytes. 





        

<hr>



### function GetWidthHeight 

_This function returns a pair of integers representing the width and height._ 
```C++
inline std::pair< uint32_t, uint32_t > AGE::ImageSpecification::GetWidthHeight () 
```





**Returns:**

A std::pair&lt;uint32\_t, uint32\_t&gt; object containing the width and height.


This function returns a pair of integers representing the width and height. 

**Returns:**

A std::pair&lt;uint32\_t, uint32\_t&gt; where first element is the width and second is the height. 





        

<hr>



### function ImageSpecification [1/4]

_Default constructor for_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._
```C++
AGE::ImageSpecification::ImageSpecification () = default
```



This function initializes an instance of the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class with its default values. It does not take any parameters and returns nothing.


Default constructor for [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class. 


        

<hr>



### function ImageSpecification [2/4]

_Default copy constructor for the_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._
```C++
AGE::ImageSpecification::ImageSpecification (
    const ImageSpecification &
) = default
```



This function is used to create a new instance of an [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object by copying another existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object to be copied.

Copy constructor for the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class.


This function creates a new instance of the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class by copying all data from an existing instance. It uses the '= default' syntax to allow the compiler to generate its own copy constructor.




**Parameters:**


* `other` The existing [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) instance to be copied. 




        

<hr>



### function ImageSpecification [3/4]

```C++
inline Unknown AGE::ImageSpecification::ImageSpecification (
    uint32_t width,
    uint32_t height,
    int channels,
    uint8_t type,
    AsepriteFileData Data
) 
```




<hr>



### function ImageSpecification [4/4]

_Constructs an_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _object with the given parameters._
```C++
inline AGE::ImageSpecification::ImageSpecification (
    uint32_t width,
    uint32_t height,
    uint8_t type,
    AsepriteFileData Data
) 
```



The constructor initializes the image specification based on the provided width, height, type and data. It sets the number of channels and pixels per byte according to the pixel type. If the pixel type is invalid, it logs an error message. For greyscale images, a warning message is logged as there's currently no implementation for 2-channel textures.




**Parameters:**


* `width` The width of the image in pixels. 
* `height` The height of the image in pixels. 
* `type` The pixel type of the image (RGBA, RGB or Greyscale). 
* `Data` The [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) associated with this [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md).

Constructs an [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object with the given parameters.


This function initializes an [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object with a specified width, height, type and data. It sets up various properties based on the provided inputs such as Channels, PixelsPerByte, Bounds etc. The function also handles different pixel types (RGBA, RGB, Greyscale) by setting appropriate values for Channels and PixelsPerByte.




**Parameters:**


* `width` Width of the image in pixels. 
* `height` Height of the image in pixels. 
* `type` Type of the pixel data. It can be one of the following: RGBA, RGB or Greyscale. 
* `Data` [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) containing the raw pixel data. 




        

<hr>



### function SetBounds 

_Sets the bounds of an object._ 
```C++
inline void AGE::ImageSpecification::SetBounds (
    const AGERect & bounds
) 
```





**Parameters:**


* `bounds` The new bounds to set for the object.

Sets the bounds of an object. 

**Parameters:**


* `bounds` The new bounds to set for the object. 




        

<hr>



### function SetChannels 

_Sets the number of audio channels to be processed by the system._ 
```C++
inline void AGE::ImageSpecification::SetChannels (
    int channels
) 
```



This function sets the 'Channels' variable, which represents the number of audio channels in the system. It takes an integer parameter 'channels', which is used to set the value of Channels.




**Parameters:**


* `channels` The new number of audio channels.



**Returns:**

void


Sets the number of audio channels to be processed by the system.


This function sets the 'Channels' variable, which represents the number of audio channels in the system. The parameter 'channels' should be a positive integer representing the desired number of channels. If it is not, or if there are any issues with setting this value (e.g., an invalid argument), no action will be taken and the function will return immediately.




**Parameters:**


* `channels` The new number of audio channels to set. Must be a positive integer. 




        

<hr>



### function SetFileData 

_Sets the file data for the_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _object._
```C++
inline void AGE::ImageSpecification::SetFileData (
    const AsepriteFileData & Data
) 
```





**Parameters:**


* `Data` The new file data to be set.

Sets the file data for the [**Aseprite**](class_a_g_e_1_1_aseprite.md) object. 

**Parameters:**


* `Data` The new file data to be set. 




        

<hr>



### function SetHeight 

_Sets the height of an object._ 
```C++
inline void AGE::ImageSpecification::SetHeight (
    const uint32_t height
) 
```



This function sets the 'Height' member variable to a specified value. It takes one parameter, which is the new height value. The function does not return anything (void).




**Parameters:**


* `height` - The new height value for the object. Must be less than or equal to 4294967295. 



**Returns:**

void


Sets the height of an object. 

**Parameters:**


* `height` The new height value to be set. 




        

<hr>



### function SetPixelType 

_Sets the pixel type of an object._ 
```C++
inline void AGE::ImageSpecification::SetPixelType (
    const PixelType & type
) 
```



This function sets the pixel type for an object, which can be used to determine how the object should be rendered in a graphics context.




**Parameters:**


* `type` The new PixelType value to set. 



**Returns:**

void


Sets the pixel type of an object. 

**Parameters:**


* `type` The new pixel type to be set. 




        

<hr>



### function SetSize 

_Sets the size of an object._ 
```C++
inline void AGE::ImageSpecification::SetSize (
    const AGESize & size
) 
```



This function sets the size attribute of an object to a given value. The size is expected to be in the form of an [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) object.




**Parameters:**


* `size` - The new size for the object.



**Returns:**

void


Sets the size of an object. 

**Parameters:**


* `size` The new size to set for the object. 




        

<hr>



### function SetWidth 

_Sets the width of an object._ 
```C++
inline void AGE::ImageSpecification::SetWidth (
    const uint32_t width
) 
```





**Parameters:**


* `width` The new width to be set for the object.

This function sets the width of an object. 

**Parameters:**


* `width` The new width to be set for the object. 




        

<hr>



### function SetWidthHeight 

_Sets the width and height of an object using a pair of unsigned integers._ 
```C++
inline void AGE::ImageSpecification::SetWidthHeight (
    const std::pair< uint32_t, uint32_t > & WidthHeight
) 
```





**Parameters:**


* `WidthHeight` A pair of unsigned integers representing the new width and height.

Sets the width and height of an object using a pair of unsigned integers. 

**Parameters:**


* `WidthHeight` A pair containing the new width and height values. 




        

<hr>



### function ~ImageSpecification 

_Destructor for the_ [_**ImageSpecification**_](struct_a_g_e_1_1_image_specification.md) _class._
```C++
AGE::ImageSpecification::~ImageSpecification () = default
```



This function is responsible for freeing any resources that were allocated during the lifetime of an instance of this class.


Default destructor for the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) class. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Image.h`

