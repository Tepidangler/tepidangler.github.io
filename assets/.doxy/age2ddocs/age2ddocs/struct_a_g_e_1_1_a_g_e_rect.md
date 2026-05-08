

# Struct AGE::AGERect



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int32\_t | [**Height**](#variable-height)  <br> |
|  int32\_t | [**Width**](#variable-width)  <br> |
|  [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) | [**XY**](#variable-xy)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGERect**](#function-agerect-13) () = default<br> |
|   | [**AGERect**](#function-agerect-23) ([**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) Point, int32\_t width, int32\_t height) <br> |
|   | [**AGERect**](#function-agerect-33) (int32\_t x, int32\_t y, int32\_t width, int32\_t height) <br> |
|  bool | [**Contains**](#function-contains) ([**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) Point) <br> |
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
## Public Functions Documentation




### function AGERect [1/3]

```C++
AGE::AGERect::AGERect () = default
```




<hr>



### function AGERect [2/3]

```C++
inline AGE::AGERect::AGERect (
    AGEPoint Point,
    int32_t width,
    int32_t height
) 
```




<hr>



### function AGERect [3/3]

```C++
inline AGE::AGERect::AGERect (
    int32_t x,
    int32_t y,
    int32_t width,
    int32_t height
) 
```




<hr>



### function Contains 

```C++
inline bool AGE::AGERect::Contains (
    AGEPoint Point
) 
```




<hr>



### function ~AGERect 

```C++
AGE::AGERect::~AGERect () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

