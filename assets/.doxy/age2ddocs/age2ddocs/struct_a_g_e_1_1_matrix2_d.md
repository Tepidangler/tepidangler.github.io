

# Struct AGE::Matrix2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix2D**](#function-matrix2d-13) () = default<br>_Default constructor for the_ [_**Matrix2D**_](struct_a_g_e_1_1_matrix2_d.md) _class._ |
|   | [**Matrix2D**](#function-matrix2d-23) (float n00, float n01, float n10, float n11) <br>_Constructs a 2x2 matrix with the given values._  |
|   | [**Matrix2D**](#function-matrix2d-33) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br>_Constructs a 2D Matrix from two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects._ |
|  float & | [**operator()**](#function-operator) (int i, int j) <br>_Accesses an element in the matrix using two indices._  |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br>_Accesses the element at position (i, j) in a two-dimensional array._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator[]**](#function-operator_2) (int j) <br>_This function is an overloaded operator that allows for accessing_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects as if they were arrays. It returns a reference to the jth element of the vector._ |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator[]**](#function-operator_3) (int j) const<br>_Returns a constant reference to the element at index 'j' in the vector._  |




























## Public Functions Documentation




### function Matrix2D [1/3]

_Default constructor for the_ [_**Matrix2D**_](struct_a_g_e_1_1_matrix2_d.md) _class._
```C++
AGE::Matrix2D::Matrix2D () = default
```



Initializes a new instance of the [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md) class with default values.


Default constructor for the [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md) class.


This function initializes a new instance of the [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md) class with default values. It uses the '= default' syntax to delegate construction to the compiler-generated default constructor.




**Returns:**

A newly constructed [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md) object. 





        

<hr>



### function Matrix2D [2/3]

_Constructs a 2x2 matrix with the given values._ 
```C++
inline AGE::Matrix2D::Matrix2D (
    float n00,
    float n01,
    float n10,
    float n11
) 
```



\| n00, n01 \| \| n10, n11 \| 

**Parameters:**


* `n00` The value to be assigned to the element at row 0, column 0. 
* `n01` The value to be assigned to the element at row 0, column 1. 
* `n10` The value to be assigned to the element at row 1, column 0. 
* `n11` The value to be assigned to the element at row 1, column 1.

Constructs a 2x2 matrix with the given values.




**Parameters:**


* `n00` The value to be assigned to the element at row 0, column 0 of the matrix. 
* `n01` The value to be assigned to the element at row 0, column 1 of the matrix. 
* `n10` The value to be assigned to the element at row 1, column 0 of the matrix. 
* `n11` The value to be assigned to the element at row 1, column 1 of the matrix. 




        

<hr>



### function Matrix2D [3/3]

_Constructs a 2D Matrix from two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects._
```C++
inline AGE::Matrix2D::Matrix2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



\| a[0], a[1]\| \| b[0], b[1]\| 


The constructor initializes the matrix with values from two vectors, `a` and `b`. Each vector is represented as an (x, y) pair where x and y are the coordinates of the vector. The first row of the matrix gets the values from vector a and the second row from vector b.




**Parameters:**


* `a` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the first row of the matrix. 
* `b` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the second row of the matrix.

Constructs a 2x2 matrix from two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects. 

**Parameters:**


* `a` The first vector to use for the construction of the matrix. 
* `b` The second vector to use for the construction of the matrix. 




        

<hr>



### function operator() 

_Accesses an element in the matrix using two indices._ 
```C++
inline float & AGE::Matrix2D::operator() (
    int i,
    int j
) 
```



This function allows access to a single element in the matrix through its two-dimensional coordinates (i, j). It returns a reference to the requested element which can be used for read or write operations.




**Parameters:**


* `i` The first index of the element to access. 
* `j` The second index of the element to access. 



**Returns:**

A reference to the accessed element.


Accesses an element in the matrix using two indices.


This function allows access to a single element in the matrix by providing two indices, i and j. It returns a reference to the element at position (i,j) in the matrix. The indices are zero-based.




**Parameters:**


* `i` The first index of the element to be accessed. 
* `j` The second index of the element to be accessed. 



**Returns:**

A reference to the element at position (i,j). 





        

<hr>



### function operator() 

_Accesses the element at position (i, j) in a two-dimensional array._ 
```C++
inline const float & AGE::Matrix2D::operator() (
    int i,
    int j
) const
```



This function allows you to access an element at a specific location in a 2D array using the subscript operator syntax. The indices i and j specify the position of the desired element.




**Parameters:**


* `i` The index along the first dimension (row). 
* `j` The index along the second dimension (column).



**Returns:**

A constant reference to the element at position (i, j) in the array.


Access the element at a given position in constant time.


This function allows for constant-time access to elements in the matrix. It takes two parameters, i and j, which represent the row and column indices of the desired element respectively. The function returns a reference to the requested element.




**Parameters:**


* `i` The index of the row (starting from 0). 
* `j` The index of the column (starting from 0). 



**Returns:**

A constant reference to the element at position (i,j) in the matrix. 





        

<hr>



### function operator[] 

_This function is an overloaded operator that allows for accessing_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects as if they were arrays. It returns a reference to the jth element of the vector._
```C++
inline Vector2 & AGE::Matrix2D::operator[] (
    int j
) 
```





**Parameters:**


* `j` The index of the element to access. Must be in the range [0, size-1]. 



**Returns:**

A reference to the jth element of the vector.


This function is an overloaded operator [] that returns a reference to the [**Vector2**](struct_a_g_e_1_1_vector2.md) object at index 'j' in the array. 

**Parameters:**


* `j` The index of the element to be accessed in the array. 



**Returns:**

A reference to the [**Vector2**](struct_a_g_e_1_1_vector2.md) object at index 'j'. 





        

<hr>



### function operator[] 

_Returns a constant reference to the element at index 'j' in the vector._ 
```C++
inline const Vector2 & AGE::Matrix2D::operator[] (
    int j
) const
```



This function returns a constant reference to the element at index 'j'. It is used for accessing elements of the vector without modifying them. The returned value should not be modified as it may lead to undefined behavior if the original data is changed elsewhere.




**Parameters:**


* `j` Index of the element to return. Must be a valid index within the range of the vector. 



**Returns:**

A constant reference to the element at index 'j'.


This function returns a reference to the [**Vector2**](struct_a_g_e_1_1_vector2.md) object at index 'j' in an array of [**Vector2**](struct_a_g_e_1_1_vector2.md) objects.




**Parameters:**


* `j` The index of the [**Vector2**](struct_a_g_e_1_1_vector2.md) object in the array. 



**Returns:**

A const reference to the [**Vector2**](struct_a_g_e_1_1_vector2.md) object at index 'j'. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

