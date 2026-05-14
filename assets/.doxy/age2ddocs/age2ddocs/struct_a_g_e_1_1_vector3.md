

# Struct AGE::Vector3



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Vector3**](struct_a_g_e_1_1_vector3.md)










Inherited by the following classes: [AGE::Point3D](struct_a_g_e_1_1_point3_d.md)
















## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**x**](#variable-x)  <br> |
|  float | [**y**](#variable-y)  <br> |
|  float | [**z**](#variable-z)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Vector3**](#function-vector3-16) () <br>_Default constructor for_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _class. Initializes x, y and z to zero._ |
|   | [**Vector3**](#function-vector3-26) (float a) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the same value for x, y and z._ |
|   | [**Vector3**](#function-vector3-36) (float a, float b, float c) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the given x, y and z coordinates._ |
|   | [**Vector3**](#function-vector3-46) ([**Vector2**](struct_a_g_e_1_1_vector2.md) a, float c) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _and a float. The x and y components of the vector are set to the x component of the input_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _, while z is set to the provided float value._ |
|   | [**Vector3**](#function-vector3-56) (glm::vec3 v) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a glm::vec3 vector._ |
|   | [**Vector3**](#function-vector3-66) ([**Vector4**](struct_a_g_e_1_1_vector4.md) v) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from another_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _by copying the x, y and z values._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**cross**](#function-cross) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Computes the cross product of this vector with another one._  |
|  float | [**dot**](#function-dot) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Computes the dot product of this vector with another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  float | [**magnitude**](#function-magnitude) () const<br>_Calculates the magnitude of a vector using Euclidean distance formula._  |
|  float | [**norm**](#function-norm) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Calculates the Euclidean norm (magnitude) of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**normalize**](#function-normalize) () const<br>_Normalizes this vector._  |
|   | [**quat**](#function-quat) () <br>_Converts the current instance of_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a quaternion._ |
|   | [**vec3**](#function-vec3) () <br>_Converts the object to a glm::vec3 type._  |
|   | [**string**](#function-string) () <br>_Converts the object into a string representation._  |
|  bool | [**operator!=**](#function-operator) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_Compares this vector with another for inequality._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator\***](#function-operator_1) (float scalar) const<br>_This function returns a new vector that is the result of scaling this vector by a given scalar value._  |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br>_This function scales the x, y and z coordinates of an object by a given scalar value._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator+**](#function-operator_3) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Adds two vectors together component-wise._  |
|  void | [**operator+=**](#function-operator_4) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_This function adds the components of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to the current vector._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator-**](#function-operator-) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Subtracts another vector from this one and returns the result._  |
|  void | [**operator-=**](#function-operator-_1) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_Subtracts another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from this one._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator/**](#function-operator_5) (float scalar) const<br>_Performs division of the vector by a scalar value._  |
|  void | [**operator/=**](#function-operator_6) (float scalar) <br>_Divides the vector's components by a given scalar._  |
|  bool | [**operator==**](#function-operator_7) ([**Vector3**](struct_a_g_e_1_1_vector3.md) vec) const<br>_Compares this_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _with another for equality._ |
|  bool | [**operator==**](#function-operator_8) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Compares this vector with another for equality._  |
|  float & | [**operator[]**](#function-operator_9) (int i) <br>_This function returns a reference to the element at index 'i' in an array of float numbers._  |
|  const float & | [**operator[]**](#function-operator_10) (int i) const<br>_This function returns a reference to the element at index 'i' in an array._  |




























## Public Attributes Documentation




### variable x 

```C++
float AGE::Vector3::x;
```




<hr>



### variable y 

```C++
float AGE::Vector3::y;
```




<hr>



### variable z 

```C++
float AGE::Vector3::z;
```




<hr>
## Public Functions Documentation




### function Vector3 [1/6]

_Default constructor for_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _class. Initializes x, y and z to zero._
```C++
AGE::Vector3::Vector3 () 
```



Default constructor for the [**Vector3**](struct_a_g_e_1_1_vector3.md) class. Initializes a vector with x, y and z components set to zero. 


        

<hr>



### function Vector3 [2/6]

_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the same value for x, y and z._
```C++
AGE::Vector3::Vector3 (
    float a
) 
```



This constructor initializes all three components of the vector to the given scalar value 'a'. The resulting vector will have equal values in each component (x = a, y = a, z = a).




**Parameters:**


* `a` The scalar value used for initialization.

Constructs a [**Vector3**](struct_a_g_e_1_1_vector3.md) with equal components. 

**Parameters:**


* `a` The value to set x, y and z to. 




        

<hr>



### function Vector3 [3/6]

_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the given x, y and z coordinates._
```C++
AGE::Vector3::Vector3 (
    float a,
    float b,
    float c
) 
```





**Parameters:**


* `a` The x-coordinate of the vector. 
* `b` The y-coordinate of the vector. 
* `c` The z-coordinate of the vector.

Constructs a [**Vector3**](struct_a_g_e_1_1_vector3.md) object with the given x, y and z coordinates.




**Parameters:**


* `a` The x-coordinate of the vector. 
* `b` The y-coordinate of the vector. 
* `c` The z-coordinate of the vector. 




        

<hr>



### function Vector3 [4/6]

_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _and a float. The x and y components of the vector are set to the x component of the input_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _, while z is set to the provided float value._
```C++
AGE::Vector3::Vector3 (
    Vector2 a,
    float c
) 
```





**Parameters:**


* `a` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the x and y components of the new [**Vector3**](struct_a_g_e_1_1_vector3.md). 
* `c` A float value representing the z component of the new [**Vector3**](struct_a_g_e_1_1_vector3.md).

Constructs a [**Vector3**](struct_a_g_e_1_1_vector3.md) object from another [**Vector2**](struct_a_g_e_1_1_vector2.md) and a third float value. The x and y components of the new [**Vector3**](struct_a_g_e_1_1_vector3.md) are set to be equal to the x component of the input [**Vector2**](struct_a_g_e_1_1_vector2.md), while z is set to the provided float value.




**Parameters:**


* `a` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the first two dimensions of the vector. 
* `c` A float value representing the third dimension of the vector. 




        

<hr>



### function Vector3 [5/6]

_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a glm::vec3 vector._
```C++
AGE::Vector3::Vector3 (
    glm::vec3 v
) 
```



This constructor takes a glm::vec3 vector and assigns its x, y, and z components to the corresponding members of this [**Vector3**](struct_a_g_e_1_1_vector3.md) object.




**Parameters:**


* `v` The input glm::vec3 vector.

Constructs a [**Vector3**](struct_a_g_e_1_1_vector3.md) object from a glm::vec3 vector.


This constructor takes a glm::vec3 vector and assigns its x, y, and z components to the corresponding members of this [**Vector3**](struct_a_g_e_1_1_vector3.md) object.




**Parameters:**


* `v` The input glm::vec3 vector. 




        

<hr>



### function Vector3 [6/6]

_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from another_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _by copying the x, y and z values._
```C++
AGE::Vector3::Vector3 (
    Vector4 v
) 
```





**Parameters:**


* `v` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to copy data from. 




        

<hr>



### function cross 

_Computes the cross product of this vector with another one._ 
```C++
inline Vector3 AGE::Vector3::cross (
    const Vector3 & vec
) const
```



The cross product is a vector that is perpendicular to both given vectors and points in the direction from the first to the second. It has a length equal to the area of the parallelogram with edges being the two input vectors. 

**Parameters:**


* `vec` The other vector for the cross product operation. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the result of the cross product. 





        

<hr>



### function dot 

_Computes the dot product of this vector with another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._
```C++
inline float AGE::Vector3::dot (
    const Vector3 & vec
) const
```



The function takes a constant reference to another [**Vector3**](struct_a_g_e_1_1_vector3.md) object and calculates the dot product by multiplying each corresponding component of both vectors together (x\*vec.x, y\*vec.y, z\*vec.z) and summing these products up.




**Parameters:**


* `vec` The other [**Vector3**](struct_a_g_e_1_1_vector3.md) object to compute the dot product with. 



**Returns:**

float Returns the computed dot product as a floating-point number. 





        

<hr>



### function magnitude 

_Calculates the magnitude of a vector using Euclidean distance formula._ 
```C++
inline float AGE::Vector3::magnitude () const
```





**Returns:**

The magnitude (float) of the vector. If the vector is zero, returns 0.0. 





        

<hr>



### function norm 

_Calculates the Euclidean norm (magnitude) of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._
```C++
inline float AGE::Vector3::norm (
    const Vector3 & vec
) const
```



This function calculates the length of the vector from the origin to the point defined by its x, y and z coordinates. It does this by taking the square root of the sum of the squares of differences in each coordinate: sqrtf((x - vec.x)^2 + (y - vec.y)^2 + (z - vec.z)^2).




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) object for which to calculate the norm.



**Returns:**

A float representing the Euclidean norm of the input vector. 





        

<hr>



### function normalize 

_Normalizes this vector._ 
```C++
Vector3 AGE::Vector3::normalize () const
```



This function calculates the magnitude of the vector and divides each component by that magnitude to normalize it. If the magnitude is zero, a zero vector is returned.




**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the normalized version of this vector.


Normalizes this vector.


This function calculates the unit vector (a vector with a length of one) in the same direction as the original vector. If the magnitude of the vector is zero, it returns a vector with all components set to zero.




**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the normalized version of this vector. 





        

<hr>



### function quat 

_Converts the current instance of_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a quaternion._
```C++
inline AGE::Vector3::quat () 
```



This function converts the x, y and z values of this vector into a glm::quat object. The resulting quaternion represents the same rotation as this vector.




**Returns:**

A new glm::quat that represents the same rotation as this [**Vector3**](struct_a_g_e_1_1_vector3.md). 





        

<hr>



### function vec3 

_Converts the object to a glm::vec3 type._ 
```C++
inline AGE::Vector3::vec3 () 
```



This operator overload allows for implicit conversion of an object into a glm::vec3 type. It returns a new vector with x, y and z coordinates set as per the current object's values. 

**Returns:**

A glm::vec3 object containing the x, y and z coordinates of the current object. 





        

<hr>



### function string 

_Converts the object into a string representation._ 
```C++
inline AGE::Vector3::string () 
```



This function converts the object's x, y and z coordinates into a formatted string. The resulting string includes each coordinate prefixed with "X: ", "Y: ", and "Z: ".




**Returns:**

A std::string containing the formatted coordinates. 





        

<hr>



### function operator!= 

_Compares this vector with another for inequality._ 
```C++
inline bool AGE::Vector3::operator!= (
    const Vector3 & vec
) 
```



This function compares the x, y and z components of this vector with those of the provided vector. It returns true if any of these components are not equal, false otherwise.




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to compare against. 



**Returns:**

True if any component is different, false otherwise. 





        

<hr>



### function operator\* 

_This function returns a new vector that is the result of scaling this vector by a given scalar value._ 
```C++
inline Vector3 AGE::Vector3::operator* (
    float scalar
) const
```





**Parameters:**


* `scalar` The value to scale the vector by. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the scaled vector. 





        

<hr>



### function operator\*= 

_This function scales the x, y and z coordinates of an object by a given scalar value._ 
```C++
inline void AGE::Vector3::operator*= (
    float scalar
) 
```





**Parameters:**


* `scalar` The value to scale the coordinates with.



**Returns:**

void 





        

<hr>



### function operator+ 

_Adds two vectors together component-wise._ 
```C++
inline Vector3 AGE::Vector3::operator+ (
    const Vector3 & vec
) const
```



This function takes another vector as an argument and adds its components to the current vector's components. The result is a new [**Vector3**](struct_a_g_e_1_1_vector3.md) object with the sum of the x, y, and z coordinates.




**Parameters:**


* `vec` A constant reference to another [**Vector3**](struct_a_g_e_1_1_vector3.md) object whose components will be added to this one. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object resulting from adding the x, y, and z components of the two vectors together. 





        

<hr>



### function operator+= 

_This function adds the components of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to the current vector._
```C++
inline void AGE::Vector3::operator+= (
    const Vector3 & vec
) 
```





**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to add to this one. 




        

<hr>



### function operator- 

_Subtracts another vector from this one and returns the result._ 
```C++
inline Vector3 AGE::Vector3::operator- (
    const Vector3 & vec
) const
```





**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to subtract from this instance. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) that is the difference between this instance and the provided [**Vector3**](struct_a_g_e_1_1_vector3.md). 





        

<hr>



### function operator-= 

_Subtracts another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from this one._
```C++
inline void AGE::Vector3::operator-= (
    const Vector3 & vec
) 
```



This function subtracts the x, y and z values of the provided [**Vector3**](struct_a_g_e_1_1_vector3.md) from the corresponding values in this [**Vector3**](struct_a_g_e_1_1_vector3.md).




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to be subtracted from this one. 




        

<hr>



### function operator/ 

_Performs division of the vector by a scalar value._ 
```C++
inline Vector3 AGE::Vector3::operator/ (
    float scalar
) const
```





**Parameters:**


* `scalar` The float value to divide each component of the vector by. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) where each component is the result of dividing the corresponding component of this vector by the given scalar. 





        

<hr>



### function operator/= 

_Divides the vector's components by a given scalar._ 
```C++
inline void AGE::Vector3::operator/= (
    float scalar
) 
```



This function divides each of the vector's components (x, y, z) by the provided scalar. It modifies the vector in-place and returns it for convenience.




**Parameters:**


* `scalar` The value to divide the vector's components by. Must not be zero to avoid division by zero.



**Returns:**

A reference to this [**Vector3**](struct_a_g_e_1_1_vector3.md) object after the operation. 





        

<hr>



### function operator== 

_Compares this_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _with another for equality._
```C++
inline bool AGE::Vector3::operator== (
    Vector3 vec
) const
```



This function compares the x, y and z coordinates of this vector with those of the provided one. It returns true if all three are equal, false otherwise.




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to compare against. 



**Returns:**

True if the vectors are equal (i.e., their x, y, and z values are all identical), false otherwise. 





        

<hr>



### function operator== 

_Compares this vector with another for equality._ 
```C++
inline bool AGE::Vector3::operator== (
    const Vector3 & vec
) const
```



The comparison is done component-wise, i.e., it checks if the x, y and z components of both vectors are equal.




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to compare against.



**Returns:**

True if all components of this vector match those of the provided one; false otherwise. 





        

<hr>



### function operator[] 

_This function returns a reference to the element at index 'i' in an array of float numbers._ 
```C++
inline float & AGE::Vector3::operator[] (
    int i
) 
```





**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A reference to the element at index 'i'. If 'i' is out of bounds, it will throw an exception. 





        

<hr>



### function operator[] 

_This function returns a reference to the element at index 'i' in an array._ 
```C++
inline const float & AGE::Vector3::operator[] (
    int i
) const
```





**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A constant reference to the element at index 'i'. If 'i' is out of bounds, it will throw an exception. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector3.h`

