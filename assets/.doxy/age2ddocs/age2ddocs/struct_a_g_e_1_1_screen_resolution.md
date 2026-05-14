

# Struct AGE::ScreenResolution



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ScreenResolution**](struct_a_g_e_1_1_screen_resolution.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**x**](#variable-x)   = `1280`<br> |
|  uint32\_t | [**y**](#variable-y)   = `720`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetHeight**](#function-getheight) () <br>_This function returns the height of an object._  |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetResolution**](#function-getresolution) () <br>_Returns the resolution of the screen in pixels as a pair of uint32\_t values. The first value is the width and the second one is the height._  |
|  uint32\_t | [**GetWidth**](#function-getwidth) () <br>_This function returns the width of an object._  |
|  void | [**SetResolution**](#function-setresolution) (uint32\_t X, uint32\_t Y) <br>_Sets the resolution of the display to a specified width and height._  |




























## Public Attributes Documentation




### variable x 

```C++
uint32_t AGE::ScreenResolution::x;
```




<hr>



### variable y 

```C++
uint32_t AGE::ScreenResolution::y;
```




<hr>
## Public Functions Documentation




### function GetHeight 

_This function returns the height of an object._ 
```C++
inline uint32_t AGE::ScreenResolution::GetHeight () 
```





**Returns:**

uint32\_t The height of the object in units not specified by the function. 





        

<hr>



### function GetResolution 

_Returns the resolution of the screen in pixels as a pair of uint32\_t values. The first value is the width and the second one is the height._ 
```C++
inline std::pair< uint32_t, uint32_t > AGE::ScreenResolution::GetResolution () 
```





**Returns:**

A pair containing two uint32\_t values representing the resolution of the screen. 





        

<hr>



### function GetWidth 

_This function returns the width of an object._ 
```C++
inline uint32_t AGE::ScreenResolution::GetWidth () 
```





**Returns:**

The width as a uint32\_t value. 





        

<hr>



### function SetResolution 

_Sets the resolution of the display to a specified width and height._ 
```C++
inline void AGE::ScreenResolution::SetResolution (
    uint32_t X,
    uint32_t Y
) 
```





**Parameters:**


* `X` The new width of the display in pixels. 
* `Y` The new height of the display in pixels. 



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

