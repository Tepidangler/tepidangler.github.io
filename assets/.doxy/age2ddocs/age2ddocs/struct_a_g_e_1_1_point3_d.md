

# Struct AGE::Point3D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Point3D**](struct_a_g_e_1_1_point3_d.md)








Inherits the following classes: [AGE::Vector3](struct_a_g_e_1_1_vector3.md)
























## Public Attributes inherited from AGE::Vector3

See [AGE::Vector3](struct_a_g_e_1_1_vector3.md)

| Type | Name |
| ---: | :--- |
|  float | [**x**](struct_a_g_e_1_1_vector3.md#variable-x)  <br> |
|  float | [**y**](struct_a_g_e_1_1_vector3.md#variable-y)  <br> |
|  float | [**z**](struct_a_g_e_1_1_vector3.md#variable-z)  <br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Point3D**](#function-point3d-12) () = default<br>_Default constructor for the_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _class. This function initializes a new instance of the_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _class with all coordinates set to zero._ |
|   | [**Point3D**](#function-point3d-22) (float a, float b, float c) <br>_Constructs a_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object with the given coordinates._ |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) | [**operator()**](#function-operator) ([**Vector3**](struct_a_g_e_1_1_vector3.md) v) const<br>_This function takes a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _as input and returns a_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object. The returned_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _is constructed from the x, y, z components of the input vector._ |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) | [**operator=**](#function-operator_1) ([**Vector3**](struct_a_g_e_1_1_vector3.md) v) const<br>_Assigns a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _._ |


## Public Functions inherited from AGE::Vector3

See [AGE::Vector3](struct_a_g_e_1_1_vector3.md)

| Type | Name |
| ---: | :--- |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-16) () <br>_Default constructor for_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _class. Initializes x, y and z to zero._ |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-26) (float a) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the same value for x, y and z._ |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-36) (float a, float b, float c) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object with the given x, y and z coordinates._ |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-46) ([**Vector2**](struct_a_g_e_1_1_vector2.md) a, float c) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _and a float. The x and y components of the vector are set to the x component of the input_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _, while z is set to the provided float value._ |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-56) (glm::vec3 v) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object from a glm::vec3 vector._ |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-66) ([**Vector4**](struct_a_g_e_1_1_vector4.md) v) <br>_Constructs a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from another_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _by copying the x, y and z values._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**cross**](struct_a_g_e_1_1_vector3.md#function-cross) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Computes the cross product of this vector with another one._  |
|  float | [**dot**](struct_a_g_e_1_1_vector3.md#function-dot) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Computes the dot product of this vector with another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  float | [**magnitude**](struct_a_g_e_1_1_vector3.md#function-magnitude) () const<br>_Calculates the magnitude of a vector using Euclidean distance formula._  |
|  float | [**norm**](struct_a_g_e_1_1_vector3.md#function-norm) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Calculates the Euclidean norm (magnitude) of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**normalize**](struct_a_g_e_1_1_vector3.md#function-normalize) () const<br>_Normalizes this vector._  |
|   | [**quat**](struct_a_g_e_1_1_vector3.md#function-quat) () <br>_Converts the current instance of_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a quaternion._ |
|   | [**vec3**](struct_a_g_e_1_1_vector3.md#function-vec3) () <br>_Converts the object to a glm::vec3 type._  |
|   | [**string**](struct_a_g_e_1_1_vector3.md#function-string) () <br>_Converts the object into a string representation._  |
|  bool | [**operator!=**](struct_a_g_e_1_1_vector3.md#function-operator) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_Compares this vector with another for inequality._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator\***](struct_a_g_e_1_1_vector3.md#function-operator_1) (float scalar) const<br>_This function returns a new vector that is the result of scaling this vector by a given scalar value._  |
|  void | [**operator\*=**](struct_a_g_e_1_1_vector3.md#function-operator_2) (float scalar) <br>_This function scales the x, y and z coordinates of an object by a given scalar value._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator+**](struct_a_g_e_1_1_vector3.md#function-operator_3) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Adds two vectors together component-wise._  |
|  void | [**operator+=**](struct_a_g_e_1_1_vector3.md#function-operator_4) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_This function adds the components of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to the current vector._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator-**](struct_a_g_e_1_1_vector3.md#function-operator-) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Subtracts another vector from this one and returns the result._  |
|  void | [**operator-=**](struct_a_g_e_1_1_vector3.md#function-operator-_1) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br>_Subtracts another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _from this one._ |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator/**](struct_a_g_e_1_1_vector3.md#function-operator_5) (float scalar) const<br>_Performs division of the vector by a scalar value._  |
|  void | [**operator/=**](struct_a_g_e_1_1_vector3.md#function-operator_6) (float scalar) <br>_Divides the vector's components by a given scalar._  |
|  bool | [**operator==**](struct_a_g_e_1_1_vector3.md#function-operator_7) ([**Vector3**](struct_a_g_e_1_1_vector3.md) vec) const<br>_Compares this_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _with another for equality._ |
|  bool | [**operator==**](struct_a_g_e_1_1_vector3.md#function-operator_8) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br>_Compares this vector with another for equality._  |
|  float & | [**operator[]**](struct_a_g_e_1_1_vector3.md#function-operator_9) (int i) <br>_This function returns a reference to the element at index 'i' in an array of float numbers._  |
|  const float & | [**operator[]**](struct_a_g_e_1_1_vector3.md#function-operator_10) (int i) const<br>_This function returns a reference to the element at index 'i' in an array._  |






















































## Public Functions Documentation




### function Point3D [1/2]

_Default constructor for the_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _class. This function initializes a new instance of the_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _class with all coordinates set to zero._
```C++
AGE::Point3D::Point3D () = default
```





**Returns:**

A new instance of the [**Point3D**](struct_a_g_e_1_1_point3_d.md) class with x, y and z coordinates set to 0.


Default constructor for the [**Point3D**](struct_a_g_e_1_1_point3_d.md) class. Initializes a new instance of the [**Point3D**](struct_a_g_e_1_1_point3_d.md) class with x, y and z coordinates set to zero.




**Returns:**

A new instance of the [**Point3D**](struct_a_g_e_1_1_point3_d.md) class with all coordinates initialized to 0. 





        

<hr>



### function Point3D [2/2]

_Constructs a_ [_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object with the given coordinates._
```C++
inline AGE::Point3D::Point3D (
    float a,
    float b,
    float c
) 
```



This constructor creates a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object by initializing its x, y and z coordinates using the provided arguments. It inherits from [**Vector3**](struct_a_g_e_1_1_vector3.md) class.




**Parameters:**


* `a` The x-coordinate of the point. 
* `b` The y-coordinate of the point. 
* `c` The z-coordinate of the point.

Constructs a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object by initializing its coordinates with the given values.




**Parameters:**


* `a` The x-coordinate of the point. 
* `b` The y-coordinate of the point. 
* `c` The z-coordinate of the point. 




        

<hr>



### function operator() 

_This function takes a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _as input and returns a_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _object. The returned_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _is constructed from the x, y, z components of the input vector._
```C++
inline const Point3D AGE::Point3D::operator() (
    Vector3 v
) const
```





**Parameters:**


* `v` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the coordinates in space. 



**Returns:**

A [**Point3D**](struct_a_g_e_1_1_point3_d.md) object with the same coordinates as the input vector.


This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) as input and returns a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object. The returned [**Point3D**](struct_a_g_e_1_1_point3_d.md) is constructed from the x, y, z components of the input [**Vector3**](struct_a_g_e_1_1_vector3.md).




**Parameters:**


* `v` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the coordinates in space. 



**Returns:**

A [**Point3D**](struct_a_g_e_1_1_point3_d.md) object with the same coordinates as the input [**Vector3**](struct_a_g_e_1_1_vector3.md). 





        

<hr>



### function operator= 

_Assigns a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to a_[_**Point3D**_](struct_a_g_e_1_1_point3_d.md) _._
```C++
inline const Point3D AGE::Point3D::operator= (
    Vector3 v
) const
```



This operator overload allows for the assignment of a [**Vector3**](struct_a_g_e_1_1_vector3.md) to a [**Point3D**](struct_a_g_e_1_1_point3_d.md). It takes in a const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) and returns a new [**Point3D**](struct_a_g_e_1_1_point3_d.md) with the same x, y, and z values as the input [**Vector3**](struct_a_g_e_1_1_vector3.md).




**Parameters:**


* `v` The [**Vector3**](struct_a_g_e_1_1_vector3.md) to be assigned. 



**Returns:**

A new [**Point3D**](struct_a_g_e_1_1_point3_d.md) with the same x, y, and z coordinates as the input [**Vector3**](struct_a_g_e_1_1_vector3.md).


Assigns a [**Vector3**](struct_a_g_e_1_1_vector3.md) to a [**Point3D**](struct_a_g_e_1_1_point3_d.md).


This operator overload allows for the assignment of a [**Vector3**](struct_a_g_e_1_1_vector3.md) to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object. The x, y and z coordinates of the [**Vector3**](struct_a_g_e_1_1_vector3.md) are used to initialize the corresponding members in the [**Point3D**](struct_a_g_e_1_1_point3_d.md) object.




**Parameters:**


* `v` A const reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) that is being assigned. 



**Returns:**

A new [**Point3D**](struct_a_g_e_1_1_point3_d.md) object with the same values as the input [**Vector3**](struct_a_g_e_1_1_vector3.md). 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

