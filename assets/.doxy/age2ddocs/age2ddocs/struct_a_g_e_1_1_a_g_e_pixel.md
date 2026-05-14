

# Struct AGE::AGEPixel



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEPixel**](struct_a_g_e_1_1_a_g_e_pixel.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint8\_t | [**RGBAc**](#variable-rgbac)  <br> |
|  float | [**RGBAf**](#variable-rgbaf)  <br> |
|  uint32\_t | [**U32RBGA**](#variable-u32rbga)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEPixel**](#function-agepixel-13) () = default<br>_Default constructor for the_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _class._ |
|   | [**AGEPixel**](#function-agepixel-23) (uint8\_t a, uint8\_t b, uint8\_t c, uint8\_t d) <br>_Constructs an instance of_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _with the given RGBA values._ |
|   | [**AGEPixel**](#function-agepixel-33) (float a, float b, float c, float d) <br>_Constructs an instance of_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _with the given float values._ |
|   | [**operator Bytef \***](#function-operator-bytef-*) () <br>_This function converts the object to a Bytef pointer._  |
|   | [**operator uint32\_t**](#function-operator-uint32_t) () <br>_Converts the RGBA color to a uint32\_t value._  |




























## Public Attributes Documentation




### variable RGBAc 

```C++
uint8_t AGE::AGEPixel::RGBAc[4];
```




<hr>



### variable RGBAf 

```C++
float AGE::AGEPixel::RGBAf[4];
```




<hr>



### variable U32RBGA 

```C++
uint32_t AGE::AGEPixel::U32RBGA[4];
```




<hr>
## Public Functions Documentation




### function AGEPixel [1/3]

_Default constructor for the_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _class._
```C++
AGE::AGEPixel::AGEPixel () = default
```




<hr>



### function AGEPixel [2/3]

_Constructs an instance of_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _with the given RGBA values._
```C++
inline AGE::AGEPixel::AGEPixel (
    uint8_t a,
    uint8_t b,
    uint8_t c,
    uint8_t d
) 
```



The function takes four uint8\_t parameters representing the red, green, blue and alpha components of a color in that order. It then stores these values internally as Uint32\_t for further processing. 

**Parameters:**


* `a` Red component (0-255). 
* `b` Green component (0-255). 
* `c` Blue component (0-255). 
* `d` Alpha component (0-255). 




        

<hr>



### function AGEPixel [3/3]

_Constructs an instance of_ [_**AGEPixel**_](struct_a_g_e_1_1_a_g_e_pixel.md) _with the given float values._
```C++
inline AGE::AGEPixel::AGEPixel (
    float a,
    float b,
    float c,
    float d
) 
```



This function takes four float values and assigns them to the RGBAf array in the order they are provided. It then converts these floats into a uint32\_t representation using ConvertFloatToU32() function, which is stored in U32RBGA array. 

**Parameters:**


* `a` First float value. 
* `b` Second float value. 
* `c` Third float value. 
* `d` Fourth float value. 




        

<hr>



### function operator Bytef \* 

_This function converts the object to a Bytef pointer._ 
```C++
inline AGE::AGEPixel::operator Bytef * () 
```



The function returns a pointer of type Bytef that points to the RGBA color array. It is used for certain operations in the Zlib library, which requires data to be in this format.




**Returns:**

A pointer of type Bytef pointing to the RGBA color array. 





        

<hr>



### function operator uint32\_t 

_Converts the RGBA color to a uint32\_t value._ 
```C++
inline AGE::AGEPixel::operator uint32_t () 
```



The function shifts and combines the four bytes of the RGBA color into one uint32\_t value, with each byte contributing 0 bits, 8 bits, 16 bits, and 24 bits respectively. This is done using bitwise shift and OR operations.




**Returns:**

A uint32\_t representation of the RGBA color. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

