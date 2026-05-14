

# Struct AGE::Vector2



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Vector2**](struct_a_g_e_1_1_vector2.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |
|  COMMENT | [**\_\_pad2\_\_**](#variable-__pad2__)  <br> |
|  COMMENT | [**\_\_pad3\_\_**](#variable-__pad3__)  <br> |
|  COMMENT | [**\_\_pad4\_\_**](#variable-__pad4__)  <br>_Performs element-wise division of this vector by another vector._  |
|  float | [**x**](#variable-x)  <br> |
|  float | [**y**](#variable-y)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Vector2**](#function-vector2-14) () <br>_Default constructor for the_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _class. Initializes x and y to zero._ |
|   | [**Vector2**](#function-vector2-24) (float a) <br>_Constructs a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object with both x and y components set to the same value._ |
|   | [**Vector2**](#function-vector2-34) (float a, float b) <br>_Constructs a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object with given x and y coordinates._ |
|   | [**Vector2**](#function-vector2-44) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Other) <br>_Copy constructor for a 2D vector class._  |
|  float | [**dot**](#function-dot) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Computes the dot product of this vector with another vector._  |
|  float | [**magnitude**](#function-magnitude) () const<br>_Calculates the magnitude of a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object using Euclidean distance formula._ |
|  float | [**norm**](#function-norm) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Calculates the Euclidean norm (magnitude) of a two dimensional vector._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**normalize**](#function-normalize) () const<br>_Normalizes this vector._  |
|   | [**string**](#function-string) () <br>_Converts the object into a string representation._  |
|  bool | [**operator!=**](#function-operator) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Compares two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects for inequality._ |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator\***](#function-operator_1) (float scalar) const<br> |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br>_Multiplies the x and y coordinates of this vector by a given scalar._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator+**](#function-operator_3) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Adds two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects together._ |
|  void | [**operator+=**](#function-operator_4) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) <br>_This function adds the components of a given vector to this vector._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator-**](#function-operator-) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Subtracts another vector from this one._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator-**](#function-operator-_1) (const float val) const<br>_Subtracts a scalar value from both x and y coordinates of the vector._  |
|  void | [**operator-=**](#function-operator-_2) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) <br>_Subtracts another vector from this one._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator/**](#function-operator_5) (float scalar) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator/**](#function-operator_6) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  void | [**operator/=**](#function-operator_7) (float scalar) <br>_Divides the coordinates (x, y) by a given scalar._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator=**](#function-operator_8) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Other) <br>_Assigns the values of another_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _to this one._ |
|  bool | [**operator==**](#function-operator_9) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br>_Compares two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects for equality._ |
|  float & | [**operator[]**](#function-operator_10) (int i) <br>_This function is an overloaded operator that returns a reference to the element at index 'i' in the array._  |
|  const float & | [**operator[]**](#function-operator_11) (int i) const<br>_This function returns a reference to the element at index 'i' in an array._  |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Vector2::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::Vector2::__pad1__;
```




<hr>



### variable \_\_pad2\_\_ 

```C++
COMMENT AGE::Vector2::__pad2__;
```




<hr>



### variable \_\_pad3\_\_ 

```C++
COMMENT AGE::Vector2::__pad3__;
```




<hr>



### variable \_\_pad4\_\_ 

_Performs element-wise division of this vector by another vector._ 
```C++
COMMENT AGE::Vector2::__pad4__;
```





**Parameters:**


* `vec` The vector to divide elements by. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) where each component is the corresponding components of this vector divided by the input vector. 





        

<hr>



### variable x 

```C++
float AGE::Vector2::x;
```




<hr>



### variable y 

```C++
float AGE::Vector2::y;
```




<hr>
## Public Functions Documentation




### function Vector2 [1/4]

_Default constructor for the_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _class. Initializes x and y to zero._
```C++
AGE::Vector2::Vector2 () 
```



Default constructor for [**Vector2**](struct_a_g_e_1_1_vector2.md) class. Initializes x and y to zero. 


        

<hr>



### function Vector2 [2/4]

_Constructs a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object with both x and y components set to the same value._
```C++
explicit AGE::Vector2::Vector2 (
    float a
) 
```





**Parameters:**


* `a` The value to be assigned to both x and y.

Constructs a [**Vector2**](struct_a_g_e_1_1_vector2.md) object with both x and y components set to the same value.




**Parameters:**


* `a` The value to be used for setting both x and y components of the vector. 




        

<hr>



### function Vector2 [3/4]

_Constructs a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object with given x and y coordinates._
```C++
AGE::Vector2::Vector2 (
    float a,
    float b
) 
```





**Parameters:**


* `a` The x-coordinate of the vector. 
* `b` The y-coordinate of the vector.

Constructs a [**Vector2**](struct_a_g_e_1_1_vector2.md) object with given x and y coordinates.




**Parameters:**


* `a` The x-coordinate of the vector. 
* `b` The y-coordinate of the vector. 




        

<hr>



### function Vector2 [4/4]

_Copy constructor for a 2D vector class._ 
```C++
inline AGE::Vector2::Vector2 (
    const Vector2 & Other
) 
```



This function creates a new instance of the [**Vector2**](struct_a_g_e_1_1_vector2.md) class by copying the values from another instance. The parameters are copied to the newly created object.




**Parameters:**


* `Other` A const reference to an existing [**Vector2**](struct_a_g_e_1_1_vector2.md) object. 




        

<hr>



### function dot 

_Computes the dot product of this vector with another vector._ 
```C++
inline float AGE::Vector2::dot (
    const Vector2 & vec
) const
```



The function takes a constant reference to another [**Vector2**](struct_a_g_e_1_1_vector2.md) object and calculates the dot product by multiplying the x-coordinates together, then the y-coordinates, and finally adding these two products together. It returns the result as a float.




**Parameters:**


* `vec` A const reference to the other vector with which to compute the dot product. 



**Returns:**

The computed dot product of this vector and the input vector.


Computes the dot product of this vector with another [**Vector2**](struct_a_g_e_1_1_vector2.md) object.


The function takes a constant reference to another [**Vector2**](struct_a_g_e_1_1_vector2.md) object and calculates the dot product by multiplying the x-coordinates together, then the y-coordinates, and finally adding these two products together. It returns the resulting float value which represents the dot product of this vector with the input vector.




**Parameters:**


* `vec` A constant reference to another [**Vector2**](struct_a_g_e_1_1_vector2.md) object that will be used in the calculation of the dot product.



**Returns:**

The function returns a float representing the dot product of this vector and the input vector. 





        

<hr>



### function magnitude 

_Calculates the magnitude of a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _object using Euclidean distance formula._
```C++
inline float AGE::Vector2::magnitude () const
```





**Returns:**

Returns the magnitude as a float value. If the vector is (0,0), returns 0.


Calculates the magnitude of a [**Vector2**](struct_a_g_e_1_1_vector2.md) object using the Euclidean distance formula. 

**Returns:**

The magnitude (length) of the vector as a float value. If the vector is [0, 0], returns 0. 





        

<hr>



### function norm 

_Calculates the Euclidean norm (magnitude) of a two dimensional vector._ 
```C++
inline float AGE::Vector2::norm (
    const Vector2 & vec
) const
```



This function calculates the length of the given [**Vector2**](struct_a_g_e_1_1_vector2.md) object by applying the formula for the Euclidean distance in a 2D space, which is sqrt(x^2 + y^2). 

**Parameters:**


* `vec` A constant reference to another [**Vector2**](struct_a_g_e_1_1_vector2.md) object whose norm (magnitude) we want to calculate. 



**Returns:**

Returns a float representing the magnitude of the input vector.


Calculates the Euclidean norm (magnitude) of a 2D vector.


This function takes in a constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object and calculates its Euclidean norm, which is defined as the square root of the sum of the squares of its x and y components. 

**Parameters:**


* `vec` A constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the input vector. 



**Returns:**

The Euclidean norm (magnitude) of the input vector. 





        

<hr>



### function normalize 

_Normalizes this vector._ 
```C++
Vector2 AGE::Vector2::normalize () const
```



This function calculates the unit vector (a vector with a length of 1) in the same direction as this vector. If the magnitude of this vector is zero, it returns a vector at origin.




**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the normalized version of this vector.


Normalizes this vector.


This function returns a new vector that is the normalized version of the current one. The resultant vector has its length (magnitude) equal to 1, but it maintains its directionality and orientation relative to the original vector. If the magnitude of the vector is zero, a zero-vector is returned.




**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the normalized version of this vector. 





        

<hr>



### function string 

_Converts the object into a string representation._ 
```C++
inline AGE::Vector2::string () 
```



This function converts the object's x and y coordinates into a string format. The resulting string includes the labels "X:" and "Y:" followed by their respective values.




**Returns:**

A std::string containing the formatted coordinate information.


Converts the object to a string representation.


This function converts the object into its string representation, which includes the x and y coordinates of the object. The format is "X: &lt;x&gt; Y: &lt;y&gt;".




**Returns:**

A std::string containing the formatted coordinates. 





        

<hr>



### function operator!= 

_Compares two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects for inequality._
```C++
inline bool AGE::Vector2::operator!= (
    const Vector2 & vec
) const
```



This function compares the current [**Vector2**](struct_a_g_e_1_1_vector2.md) object with another one to determine if they are not equal. It does this by comparing the x and y coordinates of both vectors.




**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) object to compare with. 



**Returns:**

True if the objects are not equal, false otherwise.


Compares two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects for inequality.


This function compares the x and y coordinates of this [**Vector2**](struct_a_g_e_1_1_vector2.md) object with another [**Vector2**](struct_a_g_e_1_1_vector2.md) object's x and y coordinates. It returns true if any of these values are not equal, false otherwise.




**Parameters:**


* `vec` The other [**Vector2**](struct_a_g_e_1_1_vector2.md) object to compare with. 



**Returns:**

True if the objects are not equal (i.e., their x or y coordinates differ), false otherwise. 





        

<hr>



### function operator\* 

```C++
inline Vector2 AGE::Vector2::operator* (
    float scalar
) const
```




<hr>



### function operator\*= 

_Multiplies the x and y coordinates of this vector by a given scalar._ 
```C++
inline void AGE::Vector2::operator*= (
    float scalar
) 
```



This function multiplies the values of 'x' and 'y' by the provided scalar, effectively scaling the vector. The result is stored back in 'x' and 'y', so no new value is returned.




**Parameters:**


* `scalar` The value to scale this vector by.

Multiplies the x and y coordinates of this vector by a given scalar. 

**Parameters:**


* `scalar` The value to multiply with. 




        

<hr>



### function operator+ 

_Adds two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects together._
```C++
inline Vector2 AGE::Vector2::operator+ (
    const Vector2 & vec
) const
```



This function takes another [**Vector2**](struct_a_g_e_1_1_vector2.md) object as an argument and returns a new [**Vector2**](struct_a_g_e_1_1_vector2.md) that represents the sum of this vector and the input vector. The x-coordinates are added together, while the y-coordinates are also added.




**Parameters:**


* `vec` A constant reference to another [**Vector2**](struct_a_g_e_1_1_vector2.md) object to be added with this one. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the sum of the two vectors.


This function adds two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects together.




**Parameters:**


* `vec` The second [**Vector2**](struct_a_g_e_1_1_vector2.md) object to add to the current one. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object that is the result of adding this vector and the input vector. 





        

<hr>



### function operator+= 

_This function adds the components of a given vector to this vector._ 
```C++
inline void AGE::Vector2::operator+= (
    const Vector2 & vec
) 
```





**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) object whose components are added to this one. 



**Returns:**

Nothing is returned as the result directly modifies the current instance (x and y).


This function adds the components of a given vector to this vector. 

**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) object whose components are added to this one. 




        

<hr>



### function operator- 

_Subtracts another vector from this one._ 
```C++
inline Vector2 AGE::Vector2::operator- (
    const Vector2 & vec
) const
```



This function subtracts the x and y components of the given vector from the corresponding components of this vector. The result is a new [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the difference between the two vectors.




**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) to be subtracted from this one. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) that represents the difference between this and the input [**Vector2**](struct_a_g_e_1_1_vector2.md).


Subtracts another vector from this one and returns the result. 

**Parameters:**


* `vec` The vector to subtract from this one. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the difference between this vector and the input vector. 





        

<hr>



### function operator- 

_Subtracts a scalar value from both x and y coordinates of the vector._ 
```C++
inline Vector2 AGE::Vector2::operator- (
    const float val
) const
```





**Parameters:**


* `val` The scalar value to subtract. 



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object with the result of the subtraction operation. 





        

<hr>



### function operator-= 

_Subtracts another vector from this one._ 
```C++
inline void AGE::Vector2::operator-= (
    const Vector2 & vec
) 
```



This function subtracts the x and y components of the given vector from the corresponding components of this vector. The result is stored in this vector, so it will be modified by this operation.




**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) to subtract from this one.

Subtracts another vector from this one.


This function subtracts the x and y components of the given vector from the corresponding components of this vector. The result is stored in this vector, so it will be modified by this operation.




**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) to subtract from this one. 




        

<hr>



### function operator/ 

```C++
inline Vector2 AGE::Vector2::operator/ (
    float scalar
) const
```




<hr>



### function operator/ 

```C++
inline Vector2 AGE::Vector2::operator/ (
    const Vector2 & vec
) const
```




<hr>



### function operator/= 

_Divides the coordinates (x, y) by a given scalar._ 
```C++
inline void AGE::Vector2::operator/= (
    float scalar
) 
```



This function divides both x and y by the provided scalar. It modifies the object on which it is called.




**Parameters:**


* `scalar` The value to divide the coordinates by. Must not be zero to avoid division by zero.

Divides the coordinates (x, y) by a given scalar. 

**Parameters:**


* `scalar` The value to divide the coordinates by. 




        

<hr>



### function operator= 

_Assigns the values of another_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _to this one._
```C++
inline Vector2 & AGE::Vector2::operator= (
    const Vector2 & Other
) 
```



This operator overload allows for assignment of the x and y coordinates from another [**Vector2**](struct_a_g_e_1_1_vector2.md) object. The function takes a constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) as its parameter, which is then used to set the x and y coordinates of the current [**Vector2**](struct_a_g_e_1_1_vector2.md) object. It returns a reference to the modified [**Vector2**](struct_a_g_e_1_1_vector2.md) object.




**Parameters:**


* `Other` A constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object whose values are to be assigned to this one.



**Returns:**

A reference to the modified [**Vector2**](struct_a_g_e_1_1_vector2.md) object. 





        

<hr>



### function operator== 

_Compares two_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects for equality._
```C++
inline bool AGE::Vector2::operator== (
    const Vector2 & vec
) const
```



This function compares the x and y coordinates of this [**Vector2**](struct_a_g_e_1_1_vector2.md) object with another [**Vector2**](struct_a_g_e_1_1_vector2.md) object's x and y coordinates. It returns true if both are equal, false otherwise.




**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) object to compare against. 



**Returns:**

True if the objects have identical x and y coordinates, false otherwise.


Compares two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects for equality based on their x and y coordinates. 

**Parameters:**


* `vec` The [**Vector2**](struct_a_g_e_1_1_vector2.md) object to compare with the current one. 



**Returns:**

True if both the x and y coordinates of the two vectors are equal, false otherwise. 





        

<hr>



### function operator[] 

_This function is an overloaded operator that returns a reference to the element at index 'i' in the array._ 
```C++
inline float & AGE::Vector2::operator[] (
    int i
) 
```





**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A reference to the element at index 'i'. If 'i' is out of bounds, it will throw an exception.


This function returns a reference to the element at index 'i' in an array. 

**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A reference to the element at index 'i'. If 'i' is out of bounds, it will throw an exception. 





        

<hr>



### function operator[] 

_This function returns a reference to the element at index 'i' in an array._ 
```C++
inline const float & AGE::Vector2::operator[] (
    int i
) const
```



The function takes an integer as input and returns a constant float reference. It is used for accessing elements of an array-like object, such as an array or vector.




**Parameters:**


* `i` An integer representing the index of the desired element in the array-like object. 



**Returns:**

A constant float reference to the element at index 'i' in the array-like object.


This function returns a reference to the element at index 'i' in an array.


The function takes an integer as input and returns a constant float reference. It is used for accessing elements of an array-like object, such as an array or vector.




**Parameters:**


* `i` An integer representing the index of the desired element in the array-like object. 



**Returns:**

A constant float reference to the element at index 'i'. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector2.h`

