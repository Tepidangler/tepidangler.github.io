

# Struct AGE::Matrix3D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix3D**](#function-matrix3d-14) () = default<br>_Default constructor for the_ [_**Matrix3D**_](struct_a_g_e_1_1_matrix3_d.md) _class._ |
|   | [**Matrix3D**](#function-matrix3d-24) (float n00, float n01, float n02, float n10, float n11, float n12, float n20, float n21, float n22) <br>_Constructs a 3x3 Matrix with the given values._  |
|   | [**Matrix3D**](#function-matrix3d-34) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & c) <br>_Constructs a 3D Matrix from three_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _instances._ |
|   | [**Matrix3D**](#function-matrix3d-44) (void \* Ptr) <br>_Constructs a 3D Matrix from a void pointer._  |
|  glm::mat3 | [**ToGLM**](#function-toglm-12) () <br>_Converts the 3x3 matrix to a GLM mat3._  |
|  glm::mat3 | [**ToGLM**](#function-toglm-22) () const<br>_Converts the 3x3 matrix to a GLM mat3._  |
|  float & | [**operator()**](#function-operator) (int i, int j) <br>_Accesses an element in the matrix using two indices._  |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br>_Returns a constant reference to the element at position (i, j)._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_2) (int j) <br>_This function is an overloaded operator that allows for accessing_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _objects in a vector of void pointers. It returns a reference to the jth element in the vector._ |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_3) (int j) const<br>_This function returns a constant reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._ |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Matrix3D::__pad0__;
```




<hr>
## Public Functions Documentation




### function Matrix3D [1/4]

_Default constructor for the_ [_**Matrix3D**_](struct_a_g_e_1_1_matrix3_d.md) _class._
```C++
AGE::Matrix3D::Matrix3D () = default
```



This function initializes a new instance of the [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) class with all elements set to zero.




**Returns:**

A newly initialized [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object.


Default constructor for the [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) class.


This function initializes a new instance of the [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) class with default values. It is used to create an empty matrix object that can be populated with data later on.




**Returns:**

A new instance of the [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) class with no specific initialization. 





        

<hr>



### function Matrix3D [2/4]

_Constructs a 3x3 Matrix with the given values._ 
```C++
inline AGE::Matrix3D::Matrix3D (
    float n00,
    float n01,
    float n02,
    float n10,
    float n11,
    float n12,
    float n20,
    float n21,
    float n22
) 
```



The function initializes a 3x3 matrix using the provided nine float parameters, each representing an element of the matrix in row-major order (i.e., n[0][0], n[0][1], ..., n[2][2]).




**Parameters:**


* `n00` Value for the first element of the matrix. 
* `n01` Value for the second element of the matrix. 
* `n02` Value for the third element of the matrix. 
* `n10` Value for the fourth element of the matrix. 
* `n11` Value for the fifth element of the matrix. 
* `n12` Value for the sixth element of the matrix. 
* `n20` Value for the seventh element of the matrix. 
* `n21` Value for the eighth element of the matrix. 
* `n22` Value for the ninth element of the matrix. 




        

<hr>



### function Matrix3D [3/4]

_Constructs a 3D Matrix from three_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _instances._
```C++
inline AGE::Matrix3D::Matrix3D (
    const Vector3 & a,
    const Vector3 & b,
    const Vector3 & c
) 
```



The constructor initializes the matrix with the x, y and z components of the input vectors. It sets the first row to correspond to the vector 'a', the second row to 'b' and the third row to 'c'. 

**Parameters:**


* `a` First [**Vector3**](struct_a_g_e_1_1_vector3.md) instance for initialization. 
* `b` Second [**Vector3**](struct_a_g_e_1_1_vector3.md) instance for initialization. 
* `c` Third [**Vector3**](struct_a_g_e_1_1_vector3.md) instance for initialization.

Constructs a 3D Matrix from three [**Vector3**](struct_a_g_e_1_1_vector3.md) instances.


The constructor initializes the matrix with the x, y and z components of the input vectors. This is used to create a 3D transformation matrix for transformations in 3D space.




**Parameters:**


* `a` First vector instance. Contains x, y and z components. 
* `b` Second vector instance. Contains x, y and z components. 
* `c` Third vector instance. Contains x, y and z components. 




        

<hr>



### function Matrix3D [4/4]

_Constructs a 3D Matrix from a void pointer._ 
```C++
inline AGE::Matrix3D::Matrix3D (
    void * Ptr
) 
```



This function takes in a void pointer to an object of type [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md), casts it to the appropriate type, and then copies its values into this [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) instance.




**Parameters:**


* `Ptr` A void pointer to an existing [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object.

Constructs a 3D Matrix from a void pointer.


This function takes in a void pointer to an object of type [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md), casts it to the appropriate type and then copies its values into this instance's matrix data members.




**Parameters:**


* `Ptr` A void pointer to an object of type [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md). 




        

<hr>



### function ToGLM [1/2]

_Converts the 3x3 matrix to a GLM mat3._ 
```C++
inline glm::mat3 AGE::Matrix3D::ToGLM () 
```



This function takes no parameters and returns a glm::mat3 object that represents the same data as the current 3x3 matrix. The returned object is constructed by copying the elements of the current matrix into it, in row-major order.




**Returns:**

A glm::mat3 object representing the same data as the current 3x3 matrix.


Converts the 3x3 matrix to a GLM mat3.


This function takes no parameters and returns a glm::mat3 object that represents the same 3x3 matrix as this one. The elements of the returned mat3 are identical to those in this matrix, with indices running from 0 to 2 for both rows and columns.




**Returns:**

A glm::mat3 representation of the current 3x3 matrix. 





        

<hr>



### function ToGLM [2/2]

_Converts the 3x3 matrix to a GLM mat3._ 
```C++
inline glm::mat3 AGE::Matrix3D::ToGLM () const
```



This function converts the current 3x3 matrix into a glm::mat3 by copying its elements directly. The resulting glm::mat3 is returned.




**Returns:**

A glm::mat3 representation of this 3x3 matrix.


Converts the matrix to a GLM mat3.


This function converts the current matrix into a glm::mat3 by extracting its elements and returning them in a new glm::mat3 object. The returned glm::mat3 will have the same values as this matrix, but it is guaranteed to be of type glm::mat3.




**Returns:**

A glm::mat3 containing the same data as this matrix. 





        

<hr>



### function operator() 

_Accesses an element in the matrix using two indices._ 
```C++
inline float & AGE::Matrix3D::operator() (
    int i,
    int j
) 
```



This function allows access to a single element in the matrix through its two-dimensional indexing scheme. The elements are accessed by their row and column indices, with 0 being the first index for both.




**Parameters:**


* `i` The column index of the element to be accessed. Must be within the range [0, size\_of\_column). 
* `j` The row index of the element to be accessed. Must be within the range [0, size\_of\_row).



**Returns:**

A reference to the float value at position (i,j) in the matrix.




**Exception:**


* `std::out_of_range` if either i or j is out of the valid range for their respective dimensions.

Accesses an element in the matrix using two indices.


This function allows access to a single element of the matrix through its two-dimensional coordinates (i, j). It returns a reference to the requested element.




**Parameters:**


* `i` The first index for accessing the element. 
* `j` The second index for accessing the element. 



**Returns:**

A reference to the accessed element. 





        

<hr>



### function operator() 

_Returns a constant reference to the element at position (i, j)._ 
```C++
inline const float & AGE::Matrix3D::operator() (
    int i,
    int j
) const
```



This function returns a constant reference to the element in the matrix at position (i, j), where i and j are zero-based indices. The returned value cannot be modified by this function. If you need to modify the matrix elements, use other functions provided by the class.




**Parameters:**


* `i` Zero-based index for the row of the element to return. 
* `j` Zero-based index for the column of the element to return.



**Returns:**

Constant reference to the (i, j)-th element in the matrix.


Access the element at position (i, j) in a two-dimensional array.


This function allows you to access an element at a specific location in a two-dimensional array using 0-based indexing. The indices i and j represent the row and column of the desired element respectively.




**Parameters:**


* `i` The row index of the element to be accessed. 
* `j` The column index of the element to be accessed. 



**Returns:**

A constant reference to the element at position (i, j). 





        

<hr>



### function operator[] 

_This function is an overloaded operator that allows for accessing_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _objects in a vector of void pointers. It returns a reference to the jth element in the vector._
```C++
inline Vector3 & AGE::Matrix3D::operator[] (
    int j
) 
```





**Parameters:**


* `j` The index of the element to access. 



**Returns:**

A reference to the jth [**Vector3**](struct_a_g_e_1_1_vector3.md) object.


This function returns a reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j' in the array.




**Parameters:**


* `j` The index of the [**Vector3**](struct_a_g_e_1_1_vector3.md) object in the array. 



**Returns:**

A reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object at index 'j'. 





        

<hr>



### function operator[] 

_This function returns a constant reference to the_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object at index 'j' in the array._
```C++
inline const Vector3 & AGE::Matrix3D::operator[] (
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

