

# Struct AGE::AGEPoint



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int32\_t | [**X**](#variable-x)  <br> |
|  int32\_t | [**Y**](#variable-y)  <br> |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEPoint**](#function-agepoint-12) () = default<br>_Default constructor for the_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _class._ |
|   | [**AGEPoint**](#function-agepoint-22) (int32\_t x, int32\_t y) <br> |
|  bool | [**operator!=**](#function-operator) (const [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) & Other) <br>_Compares two_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _objects for inequality._ |
|  bool | [**operator==**](#function-operator_1) (const [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) & Other) <br>_Compares two_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _objects for equality based on their X and Y coordinates._ |
|   | [**~AGEPoint**](#function-agepoint) () = default<br>_Default destructor for the_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _class._ |




























## Public Attributes Documentation




### variable X 

```C++
int32_t AGE::AGEPoint::X;
```




<hr>



### variable Y 

```C++
int32_t AGE::AGEPoint::Y;
```




<hr>



### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::AGEPoint::__pad0__;
```




<hr>
## Public Functions Documentation




### function AGEPoint [1/2]

_Default constructor for the_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _class._
```C++
AGE::AGEPoint::AGEPoint () = default
```




<hr>



### function AGEPoint [2/2]

```C++
inline AGE::AGEPoint::AGEPoint (
    int32_t x,
    int32_t y
) 
```




<hr>



### function operator!= 

_Compares two_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _objects for inequality._
```C++
inline bool AGE::AGEPoint::operator!= (
    const AGEPoint & Other
) 
```



This function compares the X and Y coordinates of two [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) objects for inequality. It returns true if either or both the X and Y coordinates are not equal, otherwise it returns false.




**Parameters:**


* `Other` The [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) object to compare with this one. 



**Returns:**

True if the X and Y coordinates of the two [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) objects are not equal, false otherwise. 





        

<hr>



### function operator== 

_Compares two_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _objects for equality based on their X and Y coordinates._
```C++
inline bool AGE::AGEPoint::operator== (
    const AGEPoint & Other
) 
```



This function compares the X and Y coordinates of two [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) objects for exact match. It returns true if both the X and Y coordinates are equal, otherwise it returns false.




**Parameters:**


* `Other` The other [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) object to compare with. 



**Returns:**

True if this object's X and Y coordinates are exactly equal to the Other object's X and Y coordinates; False otherwise. 





        

<hr>



### function ~AGEPoint 

_Default destructor for the_ [_**AGEPoint**_](struct_a_g_e_1_1_a_g_e_point.md) _class._
```C++
AGE::AGEPoint::~AGEPoint () = default
```



This function is used to clean up any resources that the object may be using, such as memory or file handles. It's important to ensure that all resources are properly released when an object is destroyed to prevent memory leaks or other issues.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

