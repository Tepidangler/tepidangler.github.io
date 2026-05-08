

# Class AGE::Image



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Image**](class_a_g_e_1_1_image.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t \* | [**GetImageBuffer**](#function-getimagebuffer-12) () <br> |
|  const uint32\_t \* | [**GetImageBuffer**](#function-getimagebuffer-22) () const<br> |
|  size\_t | [**GetImageByteSize**](#function-getimagebytesize) () <br> |
|  [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & | [**GetImageSpec**](#function-getimagespec-12) () <br> |
|  const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & | [**GetImageSpec**](#function-getimagespec-22) () const<br> |
|  T | [**GetPixel**](#function-getpixel) (T x, T y) <br> |
|   | [**Image**](#function-image-14) () = default<br> |
|   | [**Image**](#function-image-24) ([**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & Spec, bool FlipVerticallyOnLoad=false) <br> |
|   | [**Image**](#function-image-34) (const [**Image**](class_a_g_e_1_1_image.md) & Other) = default<br> |
|   | [**Image**](#function-image-44) (const [**Image**](class_a_g_e_1_1_image.md) && Other) noexcept<br> |
|  void | [**SetImageSpec**](#function-setimagespec) (const [**ImageSpecification**](struct_a_g_e_1_1_image_specification.md) & Spec) <br> |
| virtual  | [**~Image**](#function-image) () <br> |




























## Public Functions Documentation




### function GetImageBuffer [1/2]

```C++
inline uint32_t * AGE::Image::GetImageBuffer () 
```




<hr>



### function GetImageBuffer [2/2]

```C++
inline const uint32_t * AGE::Image::GetImageBuffer () const
```




<hr>



### function GetImageByteSize 

```C++
inline size_t AGE::Image::GetImageByteSize () 
```




<hr>



### function GetImageSpec [1/2]

```C++
inline ImageSpecification & AGE::Image::GetImageSpec () 
```




<hr>



### function GetImageSpec [2/2]

```C++
inline const ImageSpecification & AGE::Image::GetImageSpec () const
```




<hr>



### function GetPixel 

```C++
template<typename T>
inline T AGE::Image::GetPixel (
    T x,
    T y
) 
```




<hr>



### function Image [1/4]

```C++
AGE::Image::Image () = default
```




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

```C++
AGE::Image::Image (
    const Image & Other
) = default
```




<hr>



### function Image [4/4]

```C++
inline AGE::Image::Image (
    const Image && Other
) noexcept
```




<hr>



### function SetImageSpec 

```C++
inline void AGE::Image::SetImageSpec (
    const ImageSpecification & Spec
) 
```




<hr>



### function ~Image 

```C++
virtual AGE::Image::~Image () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Image.h`

