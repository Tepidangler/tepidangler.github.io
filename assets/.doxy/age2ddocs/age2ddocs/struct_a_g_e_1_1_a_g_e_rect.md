

# Struct AGE::AGERect



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int32\_t | [**Height**](#variable-height)  <br> |
|  int32\_t | [**Width**](#variable-width)  <br> |
|  [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) | [**XY**](#variable-xy)  <br> |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGERect**](#function-agerect-13) () = default<br>_Default constructor for_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _class._ |
|   | [**AGERect**](#function-agerect-23) ([**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) Point, int32\_t width, int32\_t height) <br>_Constructs an_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _object with a given point, width and height._ |
|   | [**AGERect**](#function-agerect-33) (int32\_t x, int32\_t y, int32\_t width, int32\_t height) <br>_Constructs an instance of_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _with the given coordinates and dimensions._ |
|  bool | [**Contains**](#function-contains) ([**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) Point) <br>_Checks whether the current point is equal to another given point._  |
|   | [**~AGERect**](#function-agerect) () = default<br> |




























## Public Attributes Documentation




### variable Height 

```C++
int32_t AGE::AGERect::Height;
```




<hr>



### variable Width 

```C++
int32_t AGE::AGERect::Width;
```




<hr>



### variable XY 

```C++
AGEPoint AGE::AGERect::XY;
```




<hr>



### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::AGERect::__pad0__;
```




<hr>
## Public Functions Documentation




### function AGERect [1/3]

_Default constructor for_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _class._
```C++
AGE::AGERect::AGERect () = default
```



This function initializes an instance of the [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) class with default values. It does not take any parameters and returns no value. 


        

<hr>



### function AGERect [2/3]

_Constructs an_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _object with a given point, width and height._
```C++
inline AGE::AGERect::AGERect (
    AGEPoint Point,
    int32_t width,
    int32_t height
) 
```





**Parameters:**


* `Point` The top-left corner of the rectangle. 
* `width` The width of the rectangle. 
* `height` The height of the rectangle. 




        

<hr>



### function AGERect [3/3]

_Constructs an instance of_ [_**AGERect**_](struct_a_g_e_1_1_a_g_e_rect.md) _with the given coordinates and dimensions._
```C++
inline AGE::AGERect::AGERect (
    int32_t x,
    int32_t y,
    int32_t width,
    int32_t height
) 
```





**Parameters:**


* `x` The x-coordinate of the top left corner of the rectangle. 
* `y` The y-coordinate of the top left corner of the rectangle. 
* `width` The width of the rectangle. 
* `height` The height of the rectangle. 




        

<hr>



### function Contains 

_Checks whether the current point is equal to another given point._ 
```C++
inline bool AGE::AGERect::Contains (
    AGEPoint Point
) 
```



This function compares the x and y coordinates of the current point with those of a provided point. If both are identical, it returns true indicating that the points are equivalent. Otherwise, it returns false.




**Parameters:**


* `Point` The [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) object to compare against.



**Returns:**

True if the x and y coordinates of the two points match, False otherwise. 





        

<hr>



### function ~AGERect 

```C++
AGE::AGERect::~AGERect () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

