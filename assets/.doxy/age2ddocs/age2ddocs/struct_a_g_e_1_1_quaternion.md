

# Struct AGE::Quaternion



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Quaternion**](struct_a_g_e_1_1_quaternion.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**w**](#variable-w)  <br> |
|  float | [**x**](#variable-x)  <br> |
|  float | [**y**](#variable-y)  <br> |
|  float | [**z**](#variable-z)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**GetRotationMatrix**](#function-getrotationmatrix) (void) <br>_Calculates the rotation matrix associated with this quaternion._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetVectorPart**](#function-getvectorpart-12) (void) <br>_Returns a reference to the x component of the vector._  |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetVectorPart**](#function-getvectorpart-22) (void) const<br>_Returns a reference to the first three components of this vector._  |
|   | [**Quaternion**](#function-quaternion-13) () = default<br>_Default constructor for the_ [_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _class._ |
|   | [**Quaternion**](#function-quaternion-23) (float a, float b, float c, float s) <br>[_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _constructor._ |
|   | [**Quaternion**](#function-quaternion-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, float s) <br>_Constructs a_ [_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _from a_[_**Vector3**_](struct_a_g_e_1_1_vector3.md) _and a scalar value._ |
|  void | [**SetRotationMatrix**](#function-setrotationmatrix) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & m) <br>_Sets the orientation from a given rotation matrix._  |




























## Public Attributes Documentation




### variable w 

```C++
float AGE::Quaternion::w;
```




<hr>



### variable x 

```C++
float AGE::Quaternion::x;
```




<hr>



### variable y 

```C++
float AGE::Quaternion::y;
```




<hr>



### variable z 

```C++
float AGE::Quaternion::z;
```




<hr>
## Public Functions Documentation




### function GetRotationMatrix 

_Calculates the rotation matrix associated with this quaternion._ 
```C++
Matrix3D AGE::Quaternion::GetRotationMatrix (
    void
) 
```



The function first calculates various intermediate values that are used in the calculation of the rotation matrix. These include products of the quaternion components and their squares. It then constructs a 3x3 [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object using these calculated values to represent the rotation represented by the quaternion.




**Returns:**

A 3x3 [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) representing the rotation associated with this quaternion.


Computes the rotation matrix associated with this quaternion.


The function calculates a 3D rotation matrix from the quaternion representation of a rotation. This is achieved by converting the quaternion to a 4x4 matrix, and then extracting the upper left 3x3 submatrix which represents the rotation.




**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing the 3D rotation represented by this quaternion. 





        

<hr>



### function GetVectorPart [1/2]

_Returns a reference to the x component of the vector._ 
```C++
inline Vector3 & AGE::Quaternion::GetVectorPart (
    void
) 
```



This function returns a reference to the x component of the vector, which can be used for direct manipulation or read-only access. The returned value is reinterpreted as a [**Vector3**](struct_a_g_e_1_1_vector3.md)& object. 

**Returns:**

A reference to the x component of the vector.


Returns a reference to the first three elements of this vector.


This function returns a reference to the first three elements of the vector. The returned object can be used for modifying these values directly, without needing to access them through other member functions or operators.




**Returns:**

A reference to the first three elements of the vector. 





        

<hr>



### function GetVectorPart [2/2]

_Returns a reference to the first three components of this vector._ 
```C++
inline const Vector3 & AGE::Quaternion::GetVectorPart (
    void
) const
```



This function returns a reference to the first three components of the current vector object. The returned reference can be used for read-only access to these components, or for modifying them directly if desired. 

**Returns:**

A const reference to the first three components of the vector.


Returns a constant reference to the first three elements of the vector.


This function returns a constant reference to the first three elements of the vector. It is used when you want to access these elements without modifying them, and it avoids unnecessary copying. The returned object should not be modified as it directly references internal data of this instance. 

**Returns:**

A constant reference to the first three elements of the vector. 





        

<hr>



### function Quaternion [1/3]

_Default constructor for the_ [_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _class._
```C++
AGE::Quaternion::Quaternion () = default
```



Initializes a new instance of the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) class with all elements set to zero.


Default constructor for the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) class. This function initializes a new instance of the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) class with all elements set to zero. The quaternion is initialized as the identity quaternion, which represents no rotation in 3D space.




**Returns:**

A default constructed [**Quaternion**](struct_a_g_e_1_1_quaternion.md) object. 





        

<hr>



### function Quaternion [2/3]

[_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _constructor._
```C++
inline AGE::Quaternion::Quaternion (
    float a,
    float b,
    float c,
    float s
) 
```



This function is used to initialize a new instance of the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) class with four parameters representing the x, y, z and w components of the quaternion respectively.




**Parameters:**


* `a` The value for the x component of the quaternion. 
* `b` The value for the y component of the quaternion. 
* `c` The value for the z component of the quaternion. 
* `s` The value for the w component of the quaternion.

[**Quaternion**](struct_a_g_e_1_1_quaternion.md) constructor.


This function initializes a new instance of the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) class with given values for x, y, z and w coordinates.




**Parameters:**


* `a` The value to initialize x coordinate. 
* `b` The value to initialize y coordinate. 
* `c` The value to initialize z coordinate. 
* `s` The value to initialize w coordinate. 




        

<hr>



### function Quaternion [3/3]

_Constructs a_ [_**Quaternion**_](struct_a_g_e_1_1_quaternion.md) _from a_[_**Vector3**_](struct_a_g_e_1_1_vector3.md) _and a scalar value._
```C++
inline AGE::Quaternion::Quaternion (
    const Vector3 & v,
    float s
) 
```



This function takes in a [**Vector3**](struct_a_g_e_1_1_vector3.md) and a scalar, which are used to initialize the x, y, z coordinates of the [**Quaternion**](struct_a_g_e_1_1_quaternion.md) and its w (scalar) component respectively.




**Parameters:**


* `v` The input vector that will be used to set the x, y, and z components of the quaternion. 
* `s` The scalar value that will be used to initialize the w component of the quaternion.

[**Quaternion**](struct_a_g_e_1_1_quaternion.md) constructor that takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) and a scalar as input parameters. 

**Parameters:**


* `v` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the vector part of the quaternion. 
* `s` The float value representing the scalar part of the quaternion. 




        

<hr>



### function SetRotationMatrix 

_Sets the orientation from a given rotation matrix._ 
```C++
void AGE::Quaternion::SetRotationMatrix (
    const Matrix3D & m
) 
```



This function converts a 3x3 rotation matrix into a quaternion representation of an orientation. It uses a formula based on the trace of the input matrix to determine which calculation path to take (sum &gt; 0 or max element). The resulting quaternion is stored in this object for later use.




**Parameters:**


* `m` The 3x3 rotation matrix. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

