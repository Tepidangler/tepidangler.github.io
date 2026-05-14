

# Struct AGE::Transform4D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Transform4D**](struct_a_g_e_1_1_transform4_d.md)








Inherits the following classes: [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |


## Public Attributes inherited from AGE::Matrix4D

See [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](struct_a_g_e_1_1_matrix4_d.md#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](struct_a_g_e_1_1_matrix4_d.md#variable-__pad1__)  <br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & | [**GetTranslation**](#function-gettranslation) (void) const<br>_Returns the translation of this object._  |
|  void | [**SetTranslation**](#function-settranslation) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br>_Sets the translation of the object to a new position specified by a_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object._ |
|   | [**Transform4D**](#function-transform4d-13) () = default<br>_Default constructor for the_ [_**Transform4D**_](struct_a_g_e_1_1_transform4_d.md) _class._ |
|   | [**Transform4D**](#function-transform4d-23) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23) <br>_Constructs a 4x4 transformation matrix from the given parameters._  |
|   | [**Transform4D**](#function-transform4d-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & c, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator) (int j) <br>_This function is an overloaded operator that returns a reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._ |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_1) (int j) const<br>_This function returns a constant reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._ |


## Public Functions inherited from AGE::Matrix4D

See [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)

| Type | Name |
| ---: | :--- |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-17) () = default<br>_Default constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._ |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-27) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23, float n30, float n31, float n32, float n33) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-37) (float f) <br>_Constructs a 4x4 matrix with the given value on the diagonal and zeros elsewhere._  |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-47) (glm::mat4 M) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-57) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & b, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & c, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & d) <br>_Constructs a 4D Matrix from four_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _instances._ |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-67) (void \* Ptr) <br>_Constructs a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _object from an existing pointer to another_[_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _._ |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-77) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & other) = default<br>_Copy constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._ |
|  glm::mat4 | [**ToGLM**](struct_a_g_e_1_1_matrix4_d.md#function-toglm-12) () <br>_Converts the current matrix to a GLM mat4._  |
|  glm::mat4 | [**ToGLM**](struct_a_g_e_1_1_matrix4_d.md#function-toglm-22) () const<br>_Converts the matrix to a GLM mat4._  |
|  float & | [**operator()**](struct_a_g_e_1_1_matrix4_d.md#function-operator) (int i, int j) <br>_Accesses the element at position (i, j) in a two-dimensional array._  |
|  const float & | [**operator()**](struct_a_g_e_1_1_matrix4_d.md#function-operator_1) (int i, int j) const<br>_This function returns a constant reference to the element at position (i, j) in the matrix._  |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](struct_a_g_e_1_1_matrix4_d.md#function-operator_2) (int j) <br>_This function returns a reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object at index 'j' in the array._ |
|  const [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](struct_a_g_e_1_1_matrix4_d.md#function-operator_3) (int j) const<br>_This function returns a constant reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _at index 'j' in the array._ |
















## Protected Attributes inherited from AGE::Matrix4D

See [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)

| Type | Name |
| ---: | :--- |
|  float | [**n**](struct_a_g_e_1_1_matrix4_d.md#variable-n)  <br> |






































## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Transform4D::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::Transform4D::__pad1__;
```




<hr>
## Public Functions Documentation




### function GetTranslation 

_Returns the translation of this object._ 
```C++
inline const Point3D & AGE::Transform4D::GetTranslation (
    void
) const
```



This function returns a reference to the translation component of this object. The returned value is const and should not be modified by the caller.




**Returns:**

A constant reference to the translation component of this object.


Returns the translation of this object.


This function returns a reference to the translation component of this object. The returned value is interpreted as a const [**Point3D**](struct_a_g_e_1_1_point3_d.md)&, meaning that it cannot be modified by the caller.




**Returns:**

A constant reference to the translation component of this object. 





        

<hr>



### function SetTranslation 

_Sets the translation of the object to a new position specified by a_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object._
```C++
inline void AGE::Transform4D::SetTranslation (
    const Point3D & p
) 
```



This function sets the coordinates (x, y, z) of the fourth row and column of the transformation matrix to match those of the input [**Point3D**](struct_a_g_e_1_1_point3_d.md) object 'p'. The purpose of this function is to update the translation component of the transformation matrix based on a new position.




**Parameters:**


* `p` A constant reference to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the new position.

Sets the translation of the object to a new position defined by a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object.


This function sets the coordinates (x, y, z) of the fourth row and columns of the transformation matrix to match those of the input [**Point3D**](struct_a_g_e_1_1_point3_d.md) object 'p'. It is assumed that the transformation matrix 'n' has been properly initialized before this call.




**Parameters:**


* `p` A const reference to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the new position. 




        

<hr>



### function Transform4D [1/3]

_Default constructor for the_ [_**Transform4D**_](struct_a_g_e_1_1_transform4_d.md) _class._
```C++
AGE::Transform4D::Transform4D () = default
```



This function initializes a new instance of the [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) class with default values. The default values are typically set to identity transformations, but this behavior can be overridden in derived classes.




**Returns:**

A new instance of the [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) class with default values.


Default constructor for the [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) class. 


        

<hr>



### function Transform4D [2/3]

_Constructs a 4x4 transformation matrix from the given parameters._ 
```C++
inline AGE::Transform4D::Transform4D (
    float n00,
    float n01,
    float n02,
    float n03,
    float n10,
    float n11,
    float n12,
    float n13,
    float n20,
    float n21,
    float n22,
    float n23
) 
```



The function initializes a 4x4 transformation matrix with the provided values. It assumes that the last row and column are [0, 0, 0, 1] respectively.




**Parameters:**


* `n00` Values for the matrix elements.



**Returns:**

void 





        

<hr>



### function Transform4D [3/3]

```C++
inline AGE::Transform4D::Transform4D (
    const Vector3 & a,
    const Vector3 & b,
    const Vector3 & c,
    const Point3D & p
) 
```




<hr>



### function operator[] 

_This function is an overloaded operator that returns a reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._
```C++
inline Vector3 & AGE::Transform4D::operator[] (
    int j
) 
```





**Parameters:**


* `j` The index of the element in the array to return. 



**Returns:**

A reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j'.


This function is an overloaded operator [] that returns a reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j' in the array. 

**Parameters:**


* `j` The index of the element to be accessed in the array. 



**Returns:**

A reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j'. 





        

<hr>



### function operator[] 

_This function returns a constant reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._
```C++
inline const Vector3 & AGE::Transform4D::operator[] (
    int j
) const
```





**Parameters:**


* `j` The index of the [**Vector3**](struct_a_g_e_1_1_vector3.md) object in the array. 



**Returns:**

A constant reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j'.


This function returns a constant reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j' in the array.




**Parameters:**


* `j` The index of the [**Vector3**](struct_a_g_e_1_1_vector3.md) object in the array. 



**Returns:**

A constant reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j'. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

