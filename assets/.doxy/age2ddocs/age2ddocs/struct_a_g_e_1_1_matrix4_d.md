

# Struct AGE::Matrix4D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md)










Inherited by the following classes: [AGE::Transform4D](struct_a_g_e_1_1_transform4_d.md)
















## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix4D**](#function-matrix4d-17) () = default<br>_Default constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._ |
|   | [**Matrix4D**](#function-matrix4d-27) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23, float n30, float n31, float n32, float n33) <br> |
|   | [**Matrix4D**](#function-matrix4d-37) (float f) <br>_Constructs a 4x4 matrix with the given value on the diagonal and zeros elsewhere._  |
|   | [**Matrix4D**](#function-matrix4d-47) (glm::mat4 M) <br> |
|   | [**Matrix4D**](#function-matrix4d-57) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & b, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & c, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & d) <br>_Constructs a 4D Matrix from four_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _instances._ |
|   | [**Matrix4D**](#function-matrix4d-67) (void \* Ptr) <br>_Constructs a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _object from an existing pointer to another_[_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _._ |
|   | [**Matrix4D**](#function-matrix4d-77) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & other) = default<br>_Copy constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._ |
|  glm::mat4 | [**ToGLM**](#function-toglm-12) () <br>_Converts the current matrix to a GLM mat4._  |
|  glm::mat4 | [**ToGLM**](#function-toglm-22) () const<br>_Converts the matrix to a GLM mat4._  |
|  float & | [**operator()**](#function-operator) (int i, int j) <br>_Accesses the element at position (i, j) in a two-dimensional array._  |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br>_This function returns a constant reference to the element at position (i, j) in the matrix._  |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](#function-operator_2) (int j) <br>_This function returns a reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object at index 'j' in the array._ |
|  const [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](#function-operator_3) (int j) const<br>_This function returns a constant reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _at index 'j' in the array._ |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  float | [**n**](#variable-n)  <br> |




















## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Matrix4D::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::Matrix4D::__pad1__;
```




<hr>
## Public Functions Documentation




### function Matrix4D [1/7]

_Default constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._
```C++
AGE::Matrix4D::Matrix4D () = default
```



Initializes a new instance of the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) class with all elements set to zero.


Default constructor for the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) class.


Initializes a new instance of the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) class with all elements set to zero. 


        

<hr>



### function Matrix4D [2/7]

```C++
inline AGE::Matrix4D::Matrix4D (
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
    float n23,
    float n30,
    float n31,
    float n32,
    float n33
) 
```




<hr>



### function Matrix4D [3/7]

_Constructs a 4x4 matrix with the given value on the diagonal and zeros elsewhere._ 
```C++
inline AGE::Matrix4D::Matrix4D (
    float f
) 
```





**Parameters:**


* `f` The value to be placed on the diagonal of the matrix.

This constructor initializes a 4x4 matrix where all elements are zero except for the main diagonal, which contains 'f'.


Constructs a 4x4 matrix with the given value on the diagonal and zero elsewhere.




**Parameters:**


* `f` The value to be placed on the diagonal of the matrix. 




        

<hr>



### function Matrix4D [4/7]

```C++
inline AGE::Matrix4D::Matrix4D (
    glm::mat4 M
) 
```




<hr>



### function Matrix4D [5/7]

_Constructs a 4D Matrix from four_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _instances._
```C++
inline AGE::Matrix4D::Matrix4D (
    const Vector4 & a,
    const Vector4 & b,
    const Vector4 & c,
    const Vector4 & d
) 
```



The function takes in four [**Vector4**](struct_a_g_e_1_1_vector4.md) instances, each representing one row of the matrix. It assigns the x, y, z and w components of these vectors to the corresponding elements in the matrix.




**Parameters:**


* `a` First [**Vector4**](struct_a_g_e_1_1_vector4.md) instance representing the first row of the matrix. 
* `b` Second [**Vector4**](struct_a_g_e_1_1_vector4.md) instance representing the second row of the matrix. 
* `c` Third [**Vector4**](struct_a_g_e_1_1_vector4.md) instance representing the third row of the matrix. 
* `d` Fourth [**Vector4**](struct_a_g_e_1_1_vector4.md) instance representing the fourth row of the matrix.

Constructs a 4D matrix using four vectors.


The constructor initializes the 4x4 matrix with values from four [**Vector4**](struct_a_g_e_1_1_vector4.md) objects, each representing one row of the matrix.




**Parameters:**


* `a` First vector to initialize the first row of the matrix. 
* `b` Second vector to initialize the second row of the matrix. 
* `c` Third vector to initialize the third row of the matrix. 
* `d` Fourth vector to initialize the fourth row of the matrix. 




        

<hr>



### function Matrix4D [6/7]

_Constructs a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _object from an existing pointer to another_[_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _._
```C++
inline AGE::Matrix4D::Matrix4D (
    void * Ptr
) 
```



This constructor creates a new [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object that is initialized with the values of the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) pointed to by Ptr. The matrix elements are copied one-by-one, ensuring accurate copying of all data.




**Parameters:**


* `Ptr` A pointer to an existing [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object.

Constructs a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object from a void pointer.


This function takes in a void pointer to an existing [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object, and copies its values into the new [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object. The input is expected to be of type `void*` which can hold any data type but should point to a valid [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object. If the provided pointer does not point to a valid [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object, the behavior is undefined.




**Parameters:**


* `Ptr` A void pointer to an existing [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object. 




        

<hr>



### function Matrix4D [7/7]

_Copy constructor for the_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _class._
```C++
AGE::Matrix4D::Matrix4D (
    const Matrix4D & other
) = default
```



This function creates a new instance of the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) class by copying all data from another existing [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object.




**Parameters:**


* `other` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object to copy from.

Copy constructor for a 4x4 matrix class.


This function creates a deep copy of the input matrix, copying all elements to the newly created object.




**Parameters:**


* `other` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) instance to be copied. 




        

<hr>



### function ToGLM [1/2]

_Converts the current matrix to a GLM mat4._ 
```C++
inline glm::mat4 AGE::Matrix4D::ToGLM () 
```



This function converts the current matrix into a glm::mat4 by directly copying its values into the new object. The order of elements is as follows:
* n[0][0] through n[0][3]
* n[1][0] through n[1][3]
* n[2][0] through n[2][3]
* n[3][0] through n[3][3]






**Returns:**

glm::mat4 The converted matrix.


Converts the current matrix to a GLM mat4.


This function converts the current matrix into a glm::mat4 by directly copying each element from the original matrix to the new one. The resulting matrix will have the same values as the original, but it is in the format used by GLM (OpenGL Mathematics).




**Returns:**

A glm::mat4 containing the same data as the current matrix. 





        

<hr>



### function ToGLM [2/2]

_Converts the matrix to a GLM mat4._ 
```C++
inline glm::mat4 AGE::Matrix4D::ToGLM () const
```



This function converts the current matrix into a glm::mat4 by directly copying each element from the original matrix to the new one. The order of elements is maintained in row-major order (i.e., n[0][0] through n[3][3]).




**Returns:**

A glm::mat4 with the same values as this matrix, but in a format compatible with GLM.


Converts the matrix to a GLM mat4.


This function converts the current matrix into a glm::mat4 by directly copying each element from the original matrix to the new one. The order of elements is as follows: [0][0], [0][1], [0][2], [0][3], [1][0], [1][1], [1][2], [1][3], [2][0], [2][1], [2][2], [2][3], [3][0], [3][1], [3][2], [3][3].




**Returns:**

glm::mat4 The converted matrix. 





        

<hr>



### function operator() 

_Accesses the element at position (i, j) in a two-dimensional array._ 
```C++
inline float & AGE::Matrix4D::operator() (
    int i,
    int j
) 
```



This function allows for accessing and modifying elements of a two-dimensional array using the subscript operator syntax. The indices i and j specify the location of the desired element within the array.




**Parameters:**


* `i` The first index, representing the row in the two-dimensional array. 
* `j` The second index, representing the column in the two-dimensional array.



**Returns:**

A reference to the float value at position (i, j) in the array.


Accesses an element in the matrix using two indices.


This function allows access to a specific element in the matrix by providing two indices, i and j. It returns a reference to this element. The returned value can be used for reading or writing the value of the specified element.




**Parameters:**


* `i` The first index. Must be within the range [0, size1). 
* `j` The second index. Must be within the range [0, size2).



**Returns:**

A reference to the matrix element at position (i,j). 





        

<hr>



### function operator() 

_This function returns a constant reference to the element at position (i, j) in the matrix._ 
```C++
inline const float & AGE::Matrix4D::operator() (
    int i,
    int j
) const
```





**Parameters:**


* `i` The row index of the element to return. 
* `j` The column index of the element to return. 



**Returns:**

A constant reference to the element at position (i, j).


Access the element at position (i, j) in a two-dimensional array.


This function allows for constant access to an element at position (i, j) in a 2D array. The indices i and j should be within the valid range of the array.




**Parameters:**


* `i` The row index of the element to access. 
* `j` The column index of the element to access. 



**Returns:**

A constant reference to the accessed element. 





        

<hr>



### function operator[] 

_This function returns a reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object at index 'j' in the array._
```C++
inline Vector4 & AGE::Matrix4D::operator[] (
    int j
) 
```





**Parameters:**


* `j` The index of the [**Vector4**](struct_a_g_e_1_1_vector4.md) object in the array. 



**Returns:**

A reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) object at index 'j'.


This function returns a reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) object at index 'j' in the array.




**Parameters:**


* `j` The index of the [**Vector4**](struct_a_g_e_1_1_vector4.md) object in the array. 



**Returns:**

A reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) object at index 'j'. 





        

<hr>



### function operator[] 

_This function returns a constant reference to the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _at index 'j' in the array._
```C++
inline const Vector4 & AGE::Matrix4D::operator[] (
    int j
) const
```





**Parameters:**


* `j` The index of the [**Vector4**](struct_a_g_e_1_1_vector4.md) in the array. 



**Returns:**

A constant reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) at index 'j'.


This function returns a constant reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) at index 'j' in the array.




**Parameters:**


* `j` The index of the [**Vector4**](struct_a_g_e_1_1_vector4.md) element to return. 



**Returns:**

A constant reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) at index 'j'. 





        

<hr>
## Protected Attributes Documentation




### variable n 

```C++
float AGE::Matrix4D::n[4][4];
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

