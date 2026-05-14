

# Class AGE::Image



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Image**](class_a_g_e_1_1_image.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t \* | [**GetImageBuffer**](#function-getimagebuffer-12) () <br>_This function returns a pointer to the RGB image buffer._  |
|  const uint32\_t \* | [**GetImageBuffer**](#function-getimagebuffer-22) () const<br>_Returns a pointer to the RGB image buffer._  |
|  size\_t | [**GetImageByteSize**](#function-getimagebytesize) () <br>_This function returns the size of an image in bytes._  |
|  [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & | [**GetImageSpec**](#function-getimagespec-12) () <br>_Returns the image specification object._  |
|  const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & | [**GetImageSpec**](#function-getimagespec-22) () const<br>_Returns the image specification object associated with this instance._  |
|  T | [**GetPixel**](#function-getpixel) (T x, T y) <br>_This function returns the pixel value at a given position._  |
|   | [**Image**](#function-image-14) () = default<br>_Default constructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._ |
|   | [**Image**](#function-image-24) ([**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & Spec, bool FlipVerticallyOnLoad=false) <br> |
|   | [**Image**](#function-image-34) (const [**Image**](class_a_g_e_1_1_image.md) & Other) = default<br>_Copy constructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._ |
|   | [**Image**](#function-image-44) (const [**Image**](class_a_g_e_1_1_image.md) && Other) noexcept<br>_Move constructor for_ [_**Image**_](class_a_g_e_1_1_image.md) _class._ |
|  void | [**SetImageSpec**](#function-setimagespec) (const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & Spec) <br>_Sets the image specification._  |
| virtual  | [**~Image**](#function-image) () <br>_Destructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._ |




























## Public Functions Documentation




### function GetImageBuffer [1/2]

_This function returns a pointer to the RGB image buffer._ 
```C++
inline uint32_t * AGE::Image::GetImageBuffer () 
```





**Returns:**

Pointer to the RGB image buffer, type is uint32\_t\*. If no image data exists, it will return nullptr.


This function returns a pointer to the RGB image buffer. 

**Returns:**

Pointer to the RGB image buffer, type is uint32\_t\*. If no image data exists, it will return nullptr. 





        

<hr>



### function GetImageBuffer [2/2]

_Returns a pointer to the RGB image buffer._ 
```C++
inline const uint32_t * AGE::Image::GetImageBuffer () const
```





**Returns:**

Pointer to the RGB image buffer, or nullptr if no image is available.


Returns a pointer to the RGB image buffer. 

**Returns:**

Pointer to the RGB image buffer, or nullptr if no image is available. 





        

<hr>



### function GetImageByteSize 

_This function returns the size of an image in bytes._ 
```C++
inline size_t AGE::Image::GetImageByteSize () 
```





**Returns:**

The byte size of the image.


This function returns the byte size of an image. 

**Returns:**

The byte size of the image as a size\_t value. 





        

<hr>



### function GetImageSpec [1/2]

_Returns the image specification object._ 
```C++
inline ImageSpecification & AGE::Image::GetImageSpec () 
```



This function returns a reference to an [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object, which contains information about the image such as its size and format.




**Returns:**

A reference to the [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object.


Returns the image specification object.


This function returns a reference to the internal image specification object, which contains all the information about an image such as its size and format.




**Returns:**

A reference to the image specification object (m\_Spec). 





        

<hr>



### function GetImageSpec [2/2]

_Returns the image specification object associated with this instance._ 
```C++
inline const ImageSpecification & AGE::Image::GetImageSpec () const
```





**Returns:**

A constant reference to the image specification object (m\_Spec).


Returns the image specification.


This function returns a constant reference to the image specification stored in the object. The returned value can be used to access various properties of the image, such as its size or format.




**Returns:**

A constant reference to the image specification. 





        

<hr>



### function GetPixel 

_This function returns the pixel value at a given position._ 
```C++
template<typename T>
inline T AGE::Image::GetPixel (
    T x,
    T y
) 
```



The function checks if the template type T is uint32\_t or uint16\_t and calls the appropriate function to get the pixel address. If T is not either of these types, it will return a default value of T. 

**Parameters:**


* `x` The x-coordinate of the pixel position. 
* `y` The y-coordinate of the pixel position. 



**Returns:**

Returns the pixel value at the given position.


This function returns a pixel value based on the template type. If T is of type uint32\_t it calls the GetRGBAddress() function with parameters x and y. If T is of type uint16\_t it calls the GetGSAddress() function with parameters x and y. 

**Parameters:**


* `x` The x-coordinate of the pixel to get. 
* `y` The y-coordinate of the pixel to get. 



**Returns:**

Returns a value based on the template type. If T is uint32\_t, it returns an RGB address. If T is uint16\_t, it returns a grayscale address. 





        

<hr>



### function Image [1/4]

_Default constructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._
```C++
AGE::Image::Image () = default
```



This function initializes an instance of the [**Image**](class_a_g_e_1_1_image.md) class with default values. It is used to create a new image object without any specific attributes set.




**Returns:**

A new [**Image**](class_a_g_e_1_1_image.md) object with all fields initialized to their default values.


Default constructor for the [**Image**](class_a_g_e_1_1_image.md) class.


This function initializes an instance of the [**Image**](class_a_g_e_1_1_image.md) class with default values. It is used to create a new image object without any specific attributes set.




**Returns:**

A newly created [**Image**](class_a_g_e_1_1_image.md) object with all fields initialized to their default values. 





        

<hr>



### function Image [2/4]

```C++
AGE::Image::Image (
    ImageSpecification & Spec,
    bool FlipVerticallyOnLoad=false
) 
```




<hr>



### function Image [3/4]

_Copy constructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._
```C++
AGE::Image::Image (
    const Image & Other
) = default
```



This function creates a new instance of an [**Image**](class_a_g_e_1_1_image.md) object by copying all data from another [**Image**](class_a_g_e_1_1_image.md) object. It uses the '= default' syntax to delegate the copy construction to the compiler, which means it will use the default implementation provided by the compiler. The compiler-generated copy constructor performs a memberwise copy of the source object into this new object. This includes copying all data members that are part of the [**Image**](class_a_g_e_1_1_image.md) class.




**Parameters:**


* `Other` The [**Image**](class_a_g_e_1_1_image.md) object to be copied.

Copy constructor for the [**Image**](class_a_g_e_1_1_image.md) class.


This function creates a new instance of an [**Image**](class_a_g_e_1_1_image.md) object by copying all data from another [**Image**](class_a_g_e_1_1_image.md) object. It is used to ensure deep copy semantics when passing objects by value or returning them from functions.




**Parameters:**


* `Other` The [**Image**](class_a_g_e_1_1_image.md) object to be copied. 




        

<hr>



### function Image [4/4]

_Move constructor for_ [_**Image**_](class_a_g_e_1_1_image.md) _class._
```C++
inline AGE::Image::Image (
    const Image && Other
) noexcept
```



This function is used to create a new instance of the [**Image**](class_a_g_e_1_1_image.md) class by moving all its data from an existing instance. It takes in a const lvalue reference to another [**Image**](class_a_g_e_1_1_image.md) object and moves its data into this new object, leaving the original object empty. The move operation is exception-safe as it does not throw exceptions under normal circumstances.




**Parameters:**


* `Other` An rvalue reference to an existing [**Image**](class_a_g_e_1_1_image.md) object.

Move constructor for the [**Image**](class_a_g_e_1_1_image.md) class.


This function creates a new instance of the [**Image**](class_a_g_e_1_1_image.md) class by moving all data from another instance to this one. It is used when an rvalue reference to an [**Image**](class_a_g_e_1_1_image.md) object is passed in, such as when it's returned from a function.




**Parameters:**


* `Other` The other [**Image**](class_a_g_e_1_1_image.md) object from which to move data. 




        

<hr>



### function SetImageSpec 

_Sets the image specification._ 
```C++
inline void AGE::Image::SetImageSpec (
    const ImageSpecification & Spec
) 
```



This function sets the image specification to a new value. The [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object is passed by const reference, meaning that no copy of it will be made and the original object can still be used elsewhere in the code.




**Parameters:**


* `Spec` A constant reference to an [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) object containing the new image specification.

Sets the image specification. 

**Parameters:**


* `Spec` The new image specification to set. 




        

<hr>



### function ~Image 

_Destructor for the_ [_**Image**_](class_a_g_e_1_1_image.md) _class._
```C++
virtual AGE::Image::~Image () 
```



This destructor does not perform any specific action as it is a default one provided by the compiler. It simply releases any resources that were acquired during object creation, such as memory allocated with 'new'.




**Returns:**

void


Destructor for the [**Image**](class_a_g_e_1_1_image.md) class.


This destructor is responsible for releasing any resources that were acquired by the [**Image**](class_a_g_e_1_1_image.md) object, such as memory allocated for its pixels. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Image.h`

