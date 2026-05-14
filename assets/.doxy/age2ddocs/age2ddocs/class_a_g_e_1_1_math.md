

# Class AGE::Math



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Math**](class_a_g_e_1_1_math.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  float | [**ACos**](#function-acos) (float a) <br>_Computes the arc cosine of input value._  |
|  T | [**Add**](#function-add) (T a, T b) <br>_This function adds two generic type parameters and returns the result._  |
|  float | [**Cos**](#function-cos) (float a) <br>_Computes the cosine of an angle in radians._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**CrossProduct**](#function-crossproduct) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br>_Computes the cross product of two vectors._  |
|  float | [**CrossProduct2D**](#function-crossproduct2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br>_Compute the cross product of two 2D vectors._  |
|  float | [**CubeRoot**](#function-cuberoot) (float a) <br>_Calculates the cube root of a number._  |
|  bool | [**DecomposeTransform**](#function-decomposetransform) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br>_Decomposes a transformation matrix into translation, rotation and scale components._  |
|  float | [**DegreeToRadians**](#function-degreetoradians) (float Deg) <br>_Converts an angle from degrees to radians._  |
|  float | [**Degrees**](#function-degrees-12) (const float Rad) <br>_Converts a given angle from radians to degrees._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Degrees**](#function-degrees-22) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) Vec) <br>_Converts radians to degrees for a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  float | [**Determinant**](#function-determinant) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & M) <br>_Calculates the determinant of a 3x3 matrix._  |
|  float | [**DistLineLine2D**](#function-distlineline2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & p1, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & v1) <br>_Computes the shortest distance between two lines in 2D space._  |
|  float | [**DistLineLine3D**](#function-distlineline3d) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p1, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v1, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p2, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v2) <br>_Calculates the distance between two lines in 3D space._  |
|  float | [**DistPointLine2D**](#function-distpointline2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & q, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & p) <br>_Computes the distance between a point and a line in 2D space._  |
|  float | [**DistPointLine3D**](#function-distpointline3d) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & q, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br>_Computes the distance between a point and a line in 3-dimensional space._  |
|  T | [**Divide**](#function-divide) (T a, T b) <br>_Performs division operation on two numbers of type T._  |
|  float | [**DotProduct2D**](#function-dotproduct2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br>_Computes the dot product of two 2D vectors._  |
|  float | [**DotProduct3D**](#function-dotproduct3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br>_Computes the dot product of two_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _objects._ |
|  float | [**DotProductPlanePoint**](#function-dotproductplanepoint) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br>_Computes the dot product of a plane and a point in 3D space._  |
|  float | [**DotProductPlaneVector**](#function-dotproductplanevector) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br>_Computes the dot product of a plane and a vector in three-dimensional space._  |
|  bool | [**IntersectLinePlane**](#function-intersectlineplane) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, const [**Plane**](struct_a_g_e_1_1_plane.md) & f, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* q) <br>_This function calculates the intersection point of a line and plane._  |
|  bool | [**IntersectThreePlanes**](#function-intersectthreeplanes) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f1, const [**Plane**](struct_a_g_e_1_1_plane.md) & f2, const [**Plane**](struct_a_g_e_1_1_plane.md) & f3, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* p) <br>_Computes the intersection point of three planes in a 3D space._  |
|  bool | [**IntersectTwoPlanes**](#function-intersecttwoplanes) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f1, const [**Plane**](struct_a_g_e_1_1_plane.md) & f2, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* p, [**Vector3**](struct_a_g_e_1_1_vector3.md) \* v) <br>_Computes the intersection point and direction vector of two planes in a 3D space._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**Inverse**](#function-inverse-13) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & M) <br>_Computes the inverse of a 3x3 matrix._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**Inverse**](#function-inverse-23) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & M) <br>_Computes the inverse of a 4x4 matrix._  |
|  [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) | [**Inverse**](#function-inverse-33) (const [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) & H) <br>_Computes the inverse of a homogeneous transformation matrix._  |
|  float | [**Magnitude**](#function-magnitude) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br>_Calculates the magnitude of a three-dimensional vector._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeInvolution**](#function-makeinvolution) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br>_Creates an involution matrix from a vector._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeReflection**](#function-makereflection-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br>_Creates a reflection matrix for a given vector._  |
|  [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) | [**MakeReflection**](#function-makereflection-22) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f) <br>_Reflects a plane in 4D space._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotation**](#function-makerotation-12) (float t, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br>_Creates a rotation matrix for a given angle and axis._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeRotation**](#function-makerotation-22) (float t, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br>_Creates a rotation matrix based on an angle and axis of rotation._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationX**](#function-makerotationx) (float t) <br>_Creates a rotation matrix around the X axis._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationY**](#function-makerotationy) (float t) <br>_Creates a rotation matrix around the Y axis._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationZ**](#function-makerotationz) (float t) <br>_Creates a rotation matrix around the Z axis._  |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeScale**](#function-makescale-12) (float s, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br>_Creates a scaling matrix from a scale factor and a vector._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeScale**](#function-makescale-22) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) M, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br>_This function scales a given_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _by the x, y and z components of a_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _._ |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeSkew**](#function-makeskew) (float t, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br>_Creates a skew symmetric matrix from given parameters._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeTransform**](#function-maketransform) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Position, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br>_Creates a transformation matrix from position, rotation and scale vectors._  |
|  double | [**Modulo**](#function-modulo) (double a, double b) <br>_Computes the modulus of two numbers using fmod function from cmath library._  |
|  T | [**Multiply**](#function-multiply) (T a, T b) <br>_This function multiplies two values of type T and returns the result._  |
|  float | [**Pow**](#function-pow) (float a, float b=2.f) <br>_Computes the power of a number._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Project2D**](#function-project2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br>_Computes the projection of a vector on another._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Project3D**](#function-project3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br>_Projects a vector 'a' onto another vector 'b'._  |
|  float | [**Radians**](#function-radians-12) (const float Deg) <br>_Converts an angle from degrees to radians._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Radians**](#function-radians-22) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) Vec) <br>_Converts degrees to radians for each component of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Reject2D**](#function-reject2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br>_Computes the rejection of one vector from another in a 2D space._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Reject3D**](#function-reject3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br>_Rejects a vector from another in three dimensions._  |
|  float | [**Sin**](#function-sin) (float a) <br>_Computes the sine of an angle in radians._  |
|  float | [**Sqrt**](#function-sqrt) (float a) <br>_Calculates the square root of a given number._  |
|  T | [**Subtract**](#function-subtract) (T a, T b) <br>_This function subtracts two values of type T and returns the result._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Transform**](#function-transform-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, const [**Quaternion**](struct_a_g_e_1_1_quaternion.md) & q) <br>_This function applies a transformation to a vector using a quaternion._  |
|  [**Line**](struct_a_g_e_1_1_line.md) | [**Transform**](#function-transform-22) (const [**Line**](struct_a_g_e_1_1_line.md) & line, const [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) & H) <br>_This function applies a 4x4 homogeneous transformation matrix to a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object. The transformation is performed in 3D space and the resultant line is returned._ |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**Translate**](#function-translate) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) M, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br>_Translates a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _by a_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _._ |


























## Public Static Functions Documentation




### function ACos 

_Computes the arc cosine of input value._ 
```C++
static inline float AGE::Math::ACos (
    float a
) 
```



This function takes in a floating-point number and returns its arc cosine, which is the angle in radians whose cosine is the specified number. The result will be between 0 and pi (inclusive). If the argument is not within the range [-1,1], then NaN is returned.




**Parameters:**


* `a` Floating-point value for which to compute arc cosine. 



**Returns:**

Arc cosine of input value in radians.


Computes the arc cosine of a value.


This function takes in a floating-point number and returns its arc cosine, which is equivalent to the inverse of the standard C++ std::acos() function. The input should be between -1 and 1 (inclusive), as it represents the ratio of the hypotenuse to the side of a right triangle whose angle you want to find. If the input is not within this range, the behavior is undefined.




**Parameters:**


* `a` A floating-point number representing the cosine of an angle in radians.



**Returns:**

The arc cosine of 'a', in the range [0, pi]. 





        

<hr>



### function Add 

_This function adds two generic type parameters and returns the result._ 
```C++
template<typename T>
static inline T AGE::Math::Add (
    T a,
    T b
) 
```





**Parameters:**


* `a` The first parameter to add. 
* `b` The second parameter to add. 



**Returns:**

Returns the sum of 'a' and 'b'.


This function adds two values of the same type together. 

**Parameters:**


* `a` The first value to be added. 
* `b` The second value to be added. 



**Returns:**

The sum of the two input values. 





        

<hr>



### function Cos 

_Computes the cosine of an angle in radians._ 
```C++
static inline float AGE::Math::Cos (
    float a
) 
```



This function takes an input parameter 'a' which represents an angle in radians and returns the cosine of that angle. The result is a floating-point number representing the cosine of the input angle.




**Parameters:**


* `a` An angle in radians. 



**Returns:**

A float value representing the cosine of the input angle.


Computes the cosine of an angle in radians.


This function takes an input parameter 'a' which represents an angle in radians and returns the cosine of that angle. The result is a floating-point number representing the cosine of the input angle.




**Parameters:**


* `a` Angle in radians to compute the cosine for. 



**Returns:**

Floating point value representing the cosine of 'a'. 





        

<hr>



### function CrossProduct 

_Computes the cross product of two vectors._ 
```C++
static inline Vector3 AGE::Math::CrossProduct (
    const Vector3 & a,
    const Vector3 & b
) 
```



The function takes two [**Vector3**](struct_a_g_e_1_1_vector3.md) objects as input and returns their cross product. It uses the standard mathematical formula for calculating the cross product of three-dimensional vectors, which is (a2\*b3 - a3\*b2, a3\*b1 - a1\*b3, a1\*b2 - a2\*b1).




**Parameters:**


* `a` The first vector. 
* `b` The second vector. 



**Returns:**

[**Vector3**](struct_a_g_e_1_1_vector3.md) The cross product of the two input vectors.


Computes the cross product of two vectors.


The function takes in two [**Vector3**](struct_a_g_e_1_1_vector3.md) objects, `a` and `b`, representing three dimensional vectors. It returns a new [**Vector3**](struct_a_g_e_1_1_vector3.md) object which represents the cross product of these two input vectors.




**Parameters:**


* `a` First vector for cross product calculation. 
* `b` Second vector for cross product calculation. 



**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) object that is the result of the cross product operation. 





        

<hr>



### function CrossProduct2D 

_Compute the cross product of two 2D vectors._ 
```C++
static inline float AGE::Math::CrossProduct2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



This function calculates the cross product of two 2D vectors, which is a scalar value representing the z-component of the vector formed by taking the cross product in three dimensions. The result is returned as a float. 

**Parameters:**


* `a` First Vector for Cross Product operation. 
* `b` Second Vector for Cross Product operation. 



**Returns:**

A float that represents the cross product of two 2D vectors.


Compute the cross product of two 2D vectors.


This function calculates the 2D cross product by multiplying the components of the first vector with the second one's y-component and vice versa, then subtracting the result. The resulting value is a scalar that represents the magnitude of the cross product and its direction relative to the x and y axes respectively. 

**Parameters:**


* `a` First 2D vector. 
* `b` Second 2D vector. 



**Returns:**

A float representing the 2D cross product. 





        

<hr>



### function CubeRoot 

_Calculates the cube root of a number._ 
```C++
static inline float AGE::Math::CubeRoot (
    float a
) 
```



This function takes in a single parameter, 'a', and returns its cube root using the standard library's `std::cbrtf` function. The input should be greater than or equal to zero; attempting to calculate the cube root of negative numbers will result in undefined behavior.




**Parameters:**


* `a` A float number for which we want to find its cube root. 



**Returns:**

Returns the cube root of 'a'.


Calculates the cube root of a number.


This function takes in a floating-point number and returns its cube root value. It uses the standard library function std::cbrtf to calculate the cube root.




**Parameters:**


* `a` The input floating-point number for which we want to find the cube root. 



**Returns:**

Returns the cube root of the input number 'a'. 





        

<hr>



### function DecomposeTransform 

_Decomposes a transformation matrix into translation, rotation and scale components._ 
```C++
static bool AGE::Math::DecomposeTransform (
    const Matrix4D & Transform,
    Vector3 & Translation,
    Vector3 & Rotation,
    Vector3 & Scale
) 
```



This function takes an input transformation matrix and decomposes it into its individual components - translation, rotation and scale. The decomposition is performed using the glm library's functions for matrix operations. It first isolates perspective by clearing the last column of the matrix, then calculates translation, scale and rotation from the remaining rows.




**Parameters:**


* `Transform` The input transformation matrix to be decomposed. 
* `Translation` Output parameter where the translation component will be stored. 
* `Rotation` Output parameter where the rotation component will be stored in Euler angles (in radians). 
* `Scale` Output parameter where the scale component will be stored.



**Returns:**

Returns true if successful, false otherwise. If the input matrix is not invertible or has no perspective, this function returns false. 





        

<hr>



### function DegreeToRadians 

_Converts an angle from degrees to radians._ 
```C++
static inline float AGE::Math::DegreeToRadians (
    float Deg
) 
```



This function takes a float value representing the degree and returns its equivalent in radians. It uses the std::acosf() function, which is expected to return the arc cosine of the input value, converted into radians by dividing it by 180.




**Parameters:**


* `Deg` The angle in degrees to be converted. 



**Returns:**

The angle in radians equivalent to the input degree.


Converts an angle from degrees to radians.


This function takes a float representing the degree value and returns its equivalent in radians. It uses the std::acosf() function, which is expected to return values between 0 and pi (3.14159), so we divide by 180 to convert from degrees to radians.




**Parameters:**


* `Deg` The angle in degrees to be converted. 



**Returns:**

The equivalent of the input degree value in radians. 





        

<hr>



### function Degrees [1/2]

_Converts a given angle from radians to degrees._ 
```C++
static inline float AGE::Math::Degrees (
    const float Rad
) 
```



This function takes an input in radians and converts it into degrees using the formula (Rad / pi) \* 180. The result is then returned as output in degrees.




**Parameters:**


* `Rad` Angle in radians to be converted to degrees. 



**Returns:**

float Converted angle in degrees.


Converts an angle from radians to degrees.


This function takes a float value representing the angle in radians and converts it to degrees. The conversion is done by multiplying the input radian value with 180, then dividing by pi (approximately 3.14159). Note that this function assumes that the input is within the range of a full circle in radians (-pi to +pi), as it does not handle negative values or values greater than 2\*pi.




**Parameters:**


* `Rad` The angle in radians to be converted. 



**Returns:**

float The corresponding angle in degrees. 





        

<hr>



### function Degrees [2/2]

_Converts radians to degrees for a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._
```C++
static inline Vector3 AGE::Math::Degrees (
    const Vector3 Vec
) 
```



This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object as input and returns a new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component is the equivalent angle in degrees. The conversion formula used here is th / pi \* 180, where 'th' represents the radian angle.




**Parameters:**


* `Vec` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the angles in radians to be converted to degrees. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object with each component being the equivalent angle in degrees.


Converts a [**Vector3**](struct_a_g_e_1_1_vector3.md) object from radians to degrees.


This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object in radians and converts it into degrees by multiplying each component of the vector with 180/pi (the conversion factor). The result is then returned as another [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the same angle but in degrees. 

**Parameters:**


* `Vec` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object to be converted from radians to degrees. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component represents the corresponding component of the input vector, now in degrees. 





        

<hr>



### function Determinant 

_Calculates the determinant of a 3x3 matrix._ 
```C++
static float AGE::Math::Determinant (
    const Matrix3D & M
) 
```



This function calculates the determinant of a 3x3 matrix using the formula for calculating the determinant of a 3x3 matrix. The input is a const reference to a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object, which represents the matrix whose determinant we want to calculate.




**Parameters:**


* `M` A const reference to a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing the matrix whose determinant we want to calculate.



**Returns:**

Returns a float value representing the determinant of the input 3x3 matrix. If the input matrix is not a 3x3 matrix, the behavior is undefined.


Calculates the determinant of a 3x3 matrix.


The function takes as input a constant reference to a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object and returns its determinant. It uses the formula for calculating the determinant of a 3x3 matrix, which involves the dot product of the row vectors with the cross products of other row vectors.




**Parameters:**


* `M` A const reference to the input [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object. 



**Returns:**

The determinant of the input [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) as a float value. 





        

<hr>



### function DistLineLine2D 

_Computes the shortest distance between two lines in 2D space._ 
```C++
static float AGE::Math::DistLineLine2D (
    const Vector2 & p1,
    const Vector2 & v1
) 
```



This function calculates the shortest distance between any point on line1 and any point on line2. The result is a float value representing this minimum distance.




**Parameters:**


* `p1` A constant reference to [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing one point on the first line. 
* `v1` A constant reference to [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing direction vector of the first line.



**Returns:**

Returns a float value representing the shortest distance between two lines in 2D space.


Calculates the distance between two lines in a 2D space.


This function calculates the shortest distance between any point on line segment AB and CD, where A = p1 and B = p1 + v1. The result is the perpendicular distance from one of the points to the other line.




**Parameters:**


* `p1` First point defining the first line. 
* `v1` Direction vector for the first line.



**Returns:**

Returns a float representing the shortest distance between two lines in a 2D space. If the lines are parallel, returns Unknown. 





        

<hr>



### function DistLineLine3D 

_Calculates the distance between two lines in 3D space._ 
```C++
static float AGE::Math::DistLineLine3D (
    const Point3D & p1,
    const Vector3 & v1,
    const Point3D & p2,
    const Vector3 & v2
) 
```



The function calculates the shortest distance between two lines defined by points and directions. It uses the method of calculating the intersection point of the two lines, which is then used to calculate the distance from that point to either of the original line's points. If the determinant of the matrix formed by the direction vectors of the two lines is zero (i.e., the lines are parallel), it calculates a perpendicular distance using cross product instead.




**Parameters:**


* `p1` The first point on the first line. 
* `v1` The direction vector of the first line. 
* `p2` The first point on the second line. 
* `v2` The direction vector of the second line.



**Returns:**

The shortest distance between the two lines. If the determinant is zero, it returns the perpendicular distance.


Calculates the distance between two lines in 3D space.


The function calculates the shortest distance between two lines in 3-dimensional space defined by points and directions. It uses the method of least squares to find the closest points on each line, which minimizes the sum of the squares of the distances.




**Parameters:**


* `p1` First point on the first line. 
* `v1` Direction vector for the first line. 
* `p2` First point on the second line. 
* `v2` Direction vector for the second line.



**Returns:**

The shortest distance between the two lines. 





        

<hr>



### function DistPointLine2D 

_Computes the distance between a point and a line in 2D space._ 
```C++
static float AGE::Math::DistPointLine2D (
    const Vector2 & q,
    const Vector2 & p
) 
```



This function calculates the shortest distance from a given point to a line defined by two points. The line is represented as an origin (v) and a direction vector (q).




**Parameters:**


* `q` A [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the direction of the line. 
* `v` A [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the origin of the line. 



**Returns:**

float Returns the distance between the point and the line in 2D space. If the input parameters are invalid, it returns NaN (Not a Number).


Computes the distance between a point and a line in 2D space.


This function calculates the shortest distance from a given point to a line defined by two points. The line is represented as a vector, which starts at the origin (0,0).




**Parameters:**


* `q` A const reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the point in 2D space. 
* `v` A const reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the direction of the line from the origin.



**Returns:**

Returns a float value representing the distance between the input point and the line. If the inputs are invalid, it returns NaN (Not a Number). 





        

<hr>



### function DistPointLine3D 

_Computes the distance between a point and a line in 3-dimensional space._ 
```C++
static float AGE::Math::DistPointLine3D (
    const Point3D & q,
    const Point3D & p,
    const Vector3 & v
) 
```



The function calculates the shortest distance from a given point to a line defined by an origin point (p) and a direction vector (v). It uses the formula for the distance between two points, which is sqrt((x2 - x1)^2 + (y2 - y1)^2 + (z2 - z1)^2), where (x1, y1, z1) are the coordinates of the first point and (x2, y2, z2) are the coordinates of the second point.




**Parameters:**


* `q` The [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the point for which we want to compute the distance from the line. 
* `p` The [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the origin point of the line. 
* `v` The [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the direction vector of the line.



**Returns:**

A float value representing the shortest distance between the given point and the line. If the direction vector is zero, it returns Unknown.


Computes the distance between a point and a line in 3D space.


The function calculates the shortest distance from a given point to a line defined by an origin point (p) and a direction vector (v). It uses cross product, dot product, and square root functions for calculations.




**Parameters:**


* `q` A constant reference to the [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the query point. 
* `p` A constant reference to the [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the origin of the line. 
* `v` A constant reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the direction vector of the line.



**Returns:**

The function returns a float value representing the distance from the point to the line. If the direction vector is zero, it means the line is degenerate and the function will return NaN (not a number). 





        

<hr>



### function Divide 

_Performs division operation on two numbers of type T._ 
```C++
template<typename T>
static inline T AGE::Math::Divide (
    T a,
    T b
) 
```



This function takes in two parameters of the same type T and returns their quotient when they are divided. If the divisor is zero, it will throw an exception to avoid undefined behavior.




**Parameters:**


* `a` The first number of type T for division operation. 
* `b` The second number of type T for division operation. 



**Returns:**

Returns the result of the division operation on two numbers. 




**Exception:**


* `std::invalid_argument` if divisor is zero to avoid undefined behavior.

Performs division operation on two numbers of type T.


This function takes two parameters of the same type T and returns their quotient when they are divided. If the divisor is zero, it will throw an exception to avoid undefined behavior.




**Parameters:**


* `a` The first number of type T. 
* `b` The second number of type T. It should not be zero to prevent division by zero. 



**Returns:**

Returns the quotient when 'a' and 'b' are divided. 




**Exception:**


* `std::invalid_argument` If 'b' is zero. 




        

<hr>



### function DotProduct2D 

_Computes the dot product of two 2D vectors._ 
```C++
static inline float AGE::Math::DotProduct2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



This function takes two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects as input and returns their dot product. The dot product is calculated by multiplying the corresponding elements from each vector together (a[0]\*b[0] + a[1]\*b[1]) and summing these products up.




**Parameters:**


* `a` First [**Vector2**](struct_a_g_e_1_1_vector2.md) object to use in the dot product calculation. 
* `b` Second [**Vector2**](struct_a_g_e_1_1_vector2.md) object to use in the dot product calculation. 



**Returns:**

The result of the dot product operation.


Computes the dot product of two 2D vectors.


This function takes two [**Vector2**](struct_a_g_e_1_1_vector2.md) objects as input and returns their dot product. The dot product is calculated by multiplying the corresponding elements from each vector together (a[0]\*b[0] + a[1]\*b[1]) and summing these products up. 

**Parameters:**


* `a` First 2D vector. 
* `b` Second 2D vector. 



**Returns:**

The dot product of vectors a and b. 





        

<hr>



### function DotProduct3D 

_Computes the dot product of two_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _objects._
```C++
static inline float AGE::Math::DotProduct3D (
    const Vector3 & a,
    const Vector3 & b
) 
```



The function takes in two [**Vector3**](struct_a_g_e_1_1_vector3.md) objects, 'a' and 'b', and returns their dot product. This is calculated as the sum of the products of corresponding elements from each vector. For example, for vectors [a1, a2, a3] and [b1, b2, b3], the dot product would be (a1\*b1 + a2\*b2 + a3\*b3).




**Parameters:**


* `a` The first [**Vector3**](struct_a_g_e_1_1_vector3.md) object. 
* `b` The second [**Vector3**](struct_a_g_e_1_1_vector3.md) object.



**Returns:**

A float representing the dot product of 'a' and 'b'.


Computes the dot product of two [**Vector3**](struct_a_g_e_1_1_vector3.md) objects.


This function takes two [**Vector3**](struct_a_g_e_1_1_vector3.md) objects as input and returns their dot product. The dot product is calculated by summing up the products of corresponding elements in both vectors. For example, for [**Vector3**](struct_a_g_e_1_1_vector3.md) a = [1,2,3] and [**Vector3**](struct_a_g_e_1_1_vector3.md) b = [4,5,6], the dot product would be (1\*4 + 2\*5 + 3\*6) = 32.




**Parameters:**


* `a` The first [**Vector3**](struct_a_g_e_1_1_vector3.md) object. 
* `b` The second [**Vector3**](struct_a_g_e_1_1_vector3.md) object.



**Returns:**

A float representing the dot product of the two input vectors. 





        

<hr>



### function DotProductPlanePoint 

_Computes the dot product of a plane and a point in 3D space._ 
```C++
static inline float AGE::Math::DotProductPlanePoint (
    const Plane & f,
    const Point3D & p
) 
```



The function takes as input a [**Plane**](struct_a_g_e_1_1_plane.md) object (consisting of four components x, y, z, w) and a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object (consisting of three components [0], [1], [2]). It returns the dot product of these two vectors which is calculated as follows: f.x\*p[0] + f.y\*p[1] + f.z\*p[2] + f.w. The [**Plane**](struct_a_g_e_1_1_plane.md) object represents a plane in 3D space, and the [**Point3D**](struct_a_g_e_1_1_point3_d.md) object represents a point on that same plane.




**Parameters:**


* `f` A const reference to a [**Plane**](struct_a_g_e_1_1_plane.md) object representing a plane in 3D space. 
* `p` A const reference to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing a point on the plane.



**Returns:**

The dot product of the plane and the point as a float value.


Computes the dot product of a plane and a point in 3D space.


The function takes as input a [**Plane**](struct_a_g_e_1_1_plane.md) object (consisting of four components x, y, z, w) and a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object (consisting of three components). It returns the result of the dot product calculation between the plane and the point.




**Parameters:**


* `f` A const reference to the [**Plane**](struct_a_g_e_1_1_plane.md) object representing the plane in 3D space. 
* `p` A const reference to the [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing the point in 3D space.



**Returns:**

The result of the dot product calculation between the plane and the point as a float value. 





        

<hr>



### function DotProductPlaneVector 

_Computes the dot product of a plane and a vector in three-dimensional space._ 
```C++
static inline float AGE::Math::DotProductPlaneVector (
    const Plane & f,
    const Vector3 & v
) 
```



This function takes two parameters, a [**Plane**](struct_a_g_e_1_1_plane.md) object (consisting of x, y, z coordinates) and a [**Vector3**](struct_a_g_e_1_1_vector3.md) object (also consisting of x, y, z coordinates). It returns the dot product of these two sets of coordinates. 

**Parameters:**


* `f` The [**Plane**](struct_a_g_e_1_1_plane.md) for which to compute the dot product. 
* `v` The [**Vector3**](struct_a_g_e_1_1_vector3.md) for which to compute the dot product. 



**Returns:**

float The computed dot product.


Computes the dot product of a plane and a vector in three-dimensional space.


This function takes two parameters, a [**Plane**](struct_a_g_e_1_1_plane.md) object (consisting of x, y, z coordinates) and a [**Vector3**](struct_a_g_e_1_1_vector3.md) object (also consisting of x, y, z coordinates). It returns the result of the dot product calculation which is essentially the sum of the products of corresponding elements from the two input vectors.




**Parameters:**


* `f` The [**Plane**](struct_a_g_e_1_1_plane.md) for which to compute the dot product. 
* `v` The [**Vector3**](struct_a_g_e_1_1_vector3.md) for which to compute the dot product. 



**Returns:**

float The result of the dot product calculation. 





        

<hr>



### function IntersectLinePlane 

_This function calculates the intersection point of a line and plane._ 
```C++
static bool AGE::Math::IntersectLinePlane (
    const Point3D & p,
    const Vector3 & v,
    const Plane & f,
    Point3D * q
) 
```



The function takes in three parameters - a point 'p' on the line, a direction vector 'v', and a plane 'f'. It computes the intersection point 'q' where the line intersects with the plane. If there is an intersection, it returns true; otherwise, false.




**Parameters:**


* `p` A const reference to [**Point3D**](struct_a_g_e_1_1_point3_d.md) object representing a point on the line. 
* `v` A const reference to [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the direction of the line. 
* `f` A const reference to [**Plane**](struct_a_g_e_1_1_plane.md) object representing the plane. 
* `q` Pointer to [**Point3D**](struct_a_g_e_1_1_point3_d.md) object where the intersection point will be stored if there is an intersection.



**Returns:**

Returns true if a valid intersection exists, false otherwise.


Intersects a line with a plane.


This function calculates the intersection point of a line defined by a starting point and direction vector, and a plane. The result is stored in the output parameter `q`.




**Parameters:**


* `p` A constant reference to the starting point of the line. 
* `v` A constant reference to the direction vector of the line. 
* `f` A constant reference to the plane. 
* `q` Pointer to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object where the intersection point will be stored.



**Returns:**

Returns true if there is an intersection, false otherwise. If no intersection exists, `q` remains unchanged. 





        

<hr>



### function IntersectThreePlanes 

_Computes the intersection point of three planes in a 3D space._ 
```C++
static bool AGE::Math::IntersectThreePlanes (
    const Plane & f1,
    const Plane & f2,
    const Plane & f3,
    Point3D * p
) 
```



Given three planes, this function computes and returns their intersection point if they are not parallel (i.e., have a non-zero determinant). The intersection point is calculated using Cramer's rule.




**Parameters:**


* `f1` First plane to intersect with. 
* `f2` Second plane to intersect with. 
* `f3` Third plane to intersect with. 
* `p` Pointer to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object where the intersection point will be stored if it exists.



**Returns:**

True if planes are not parallel (determinant is non-zero), false otherwise.


Computes the intersection point of three planes in a 3D space.


Given three planes, this function computes and returns their intersection point if they are not parallel (i.e., have a non-zero determinant). The intersection point is calculated using Cramer's rule.




**Parameters:**


* `f1` First plane to intersect with. 
* `f2` Second plane to intersect with. 
* `f3` Third plane to intersect with. 
* `p` Pointer to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) object where the intersection point will be stored if it exists.



**Returns:**

True if planes are not parallel (determinant is non-zero), false otherwise. 





        

<hr>



### function IntersectTwoPlanes 

_Computes the intersection point and direction vector of two planes in a 3D space._ 
```C++
static bool AGE::Math::IntersectTwoPlanes (
    const Plane & f1,
    const Plane & f2,
    Point3D * p,
    Vector3 * v
) 
```



The function calculates the intersection line defined by its direction vector `v` and any point on this line is given by `p`. It takes as input two plane objects, each represented by a normal vector and a constant term (w). If the planes are not parallel (i.e., their normals are linearly independent), it computes the intersection point and direction vector. The function returns true if the planes intersect, false otherwise.




**Parameters:**


* `f1` First plane object with normal `n1` and constant term `f1.w`. 
* `f2` Second plane object with normal `n2` and constant term `f2.w`. 
* `p` Pointer to a [**Point3D**](struct_a_g_e_1_1_point3_d.md) where the intersection point will be stored. 
* `v` Pointer to a [**Vector3**](struct_a_g_e_1_1_vector3.md) where the direction vector of the intersection line will be stored.



**Returns:**

True if planes intersect, false otherwise. 





        

<hr>



### function Inverse [1/3]

_Computes the inverse of a 3x3 matrix._ 
```C++
static Matrix3D AGE::Math::Inverse (
    const Matrix3D & M
) 
```



Computes the inverse of a 3x3 matrix.


The function takes as input a const reference to a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object and returns an instance of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) that represents the inverse of the input matrix. It uses linear algebra methods, specifically the method of calculating the inverse of a matrix.




**Parameters:**


* `M` A const reference to the 3x3 matrix to be inverted. 



**Returns:**

An instance of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) representing the inverse of the input matrix. 


This function takes as input a const reference to a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object and returns an instance of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) that represents the inverse of the input matrix. The computation is based on the formula for finding the inverse of a 3x3 matrix, which involves cross product and dot product operations.




**Parameters:**


* `M` A const reference to the [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object whose inverse we want to compute. 



**Returns:**

An instance of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) that represents the inverse of the input matrix. 





        

<hr>



### function Inverse [2/3]

_Computes the inverse of a 4x4 matrix._ 
```C++
static Matrix4D AGE::Math::Inverse (
    const Matrix4D & M
) 
```



This function takes as input a constant reference to a 4x4 matrix and returns its inverse. The function uses various mathematical operations such as cross product and dot product to compute the inverse.




**Parameters:**


* `M` A constant reference to the 4x4 matrix to be inverted. 



**Returns:**

The inverse of the input matrix. If the determinant of the input matrix is zero, this function returns an identity matrix.


Computes the inverse of a 4x4 matrix.


This function takes as input a const reference to a 4x4 matrix and returns its inverse. The implementation is based on the formula for calculating the inverse of a 4x4 matrix, which involves cross products and dot products.




**Parameters:**


* `M` A const reference to the 4x4 matrix to be inverted. 



**Returns:**

The inverse of the input matrix. If the determinant of the input matrix is zero or negative, this function returns an identity matrix. 





        

<hr>



### function Inverse [3/3]

_Computes the inverse of a homogeneous transformation matrix._ 
```C++
static Transform4D AGE::Math::Inverse (
    const Transform4D & H
) 
```



This function takes as input a constant reference to a [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) object which represents a homogeneous transformation matrix. It then computes and returns the inverse of this matrix.




**Parameters:**


* `H` A const reference to the [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) object to be inverted. 



**Returns:**

The inverse of the input [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) object. Computes the inverse of a 4x4 homogeneous transformation matrix.


Given a 4x4 homogeneous transformation matrix, this function computes and returns its inverse. The inverse is computed by first extracting the rotation and translation components from H, then computing the cross product of these to obtain a scale vector s, and finally inverting the determinant of the upper-left 3x3 submatrix of H.




**Parameters:**


* `H` The homogeneous transformation matrix to invert. 



**Returns:**

The inverse of the input matrix. 





        

<hr>



### function Magnitude 

_Calculates the magnitude of a three-dimensional vector._ 
```C++
static inline float AGE::Math::Magnitude (
    const Vector3 & v
) 
```



This function takes a const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object and returns its magnitude by calculating the square root of the sum of the squares of each component (x, y, z).




**Parameters:**


* `v` A constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the vector for which we want to calculate the magnitude. 



**Returns:**

float The magnitude of the input vector.


Calculates the magnitude (length) of a three-dimensional vector.


This function takes a constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object and returns its magnitude by calculating the square root of the sum of the squares of each component in the vector.




**Parameters:**


* `v` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the vector for which we want to calculate the magnitude.



**Returns:**

The magnitude (length) of the input vector as a float value. 





        

<hr>



### function MakeInvolution 

_Creates an involution matrix from a vector._ 
```C++
static Matrix3D AGE::Math::MakeInvolution (
    const Vector3 & a
) 
```



This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object as input and returns a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object that represents the involution matrix corresponding to the given vector. The input vector is multiplied by 2 before being used in the calculations, which may affect the resulting matrix if the original values of the vector were not zero or one.




**Parameters:**


* `a` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the basis vectors for the transformation. 



**Returns:**

[**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) Returns a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object that represents the involution matrix corresponding to the input vector.


Creates an involution matrix from a vector.


This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object as input and returns a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object that represents the involution matrix corresponding to the input vector. The input vector is multiplied by two, and then used in the construction of the resulting matrix. 

**Parameters:**


* `a` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the input vector. 



**Returns:**

Returns a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing the involution matrix for the given input vector. 





        

<hr>



### function MakeReflection [1/2]

_Creates a reflection matrix for a given vector._ 
```C++
static Matrix3D AGE::Math::MakeReflection (
    const Vector3 & a
) 
```



This function takes in a [**Vector3**](struct_a_g_e_1_1_vector3.md) object and returns a [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object that represents the reflection of the input vector across an arbitrary axis. The returned matrix is calculated based on the formula for reflection matrices, which involves negating the components of the input vector multiplied by 2 and then adding 1 to each component.




**Parameters:**


* `a` A const reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the vector to be reflected. 



**Returns:**

[**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) The reflection matrix corresponding to the input vector. 





        

<hr>



### function MakeReflection [2/2]

_Reflects a plane in 4D space._ 
```C++
static Transform4D AGE::Math::MakeReflection (
    const Plane & f
) 
```



This function takes a [**Plane**](struct_a_g_e_1_1_plane.md) object and returns a [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) that represents the reflection of the plane across the origin. The transformation matrix is calculated based on the equation for reflection in 4 dimensions, which involves negating each component of the plane's normal vector (x, y, z) and scaling it by -1.




**Parameters:**


* `f` [**Plane**](struct_a_g_e_1_1_plane.md) object to be reflected. 



**Returns:**

[**Transform4D**](struct_a_g_e_1_1_transform4_d.md) representing the reflection transformation.


Reflects a plane in 4D space.


This function takes a [**Plane**](struct_a_g_e_1_1_plane.md) object and returns a [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) that represents the reflection of the plane across the origin. The transformation matrix is calculated based on the equation for reflection in 4D space, which involves negating each component of the plane's normal vector (x, y, z) and scaling it by -1.




**Parameters:**


* `f` [**Plane**](struct_a_g_e_1_1_plane.md) object to be reflected. 



**Returns:**

[**Transform4D**](struct_a_g_e_1_1_transform4_d.md) representing the reflection transformation. 





        

<hr>



### function MakeRotation [1/2]

_Creates a rotation matrix for a given angle and axis._ 
```C++
static Matrix3D AGE::Math::MakeRotation (
    float t,
    const Vector3 & a
) 
```



This function creates a 3x3 rotation matrix based on the provided angle (in radians) and axis vector. The resulting matrix can be used to rotate vectors or points in 3D space.




**Parameters:**


* `t` The rotation angle in radians. 
* `a` The rotation axis as a [**Vector3**](struct_a_g_e_1_1_vector3.md) object. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing the created rotation matrix. 





        

<hr>



### function MakeRotation [2/2]

_Creates a rotation matrix based on an angle and axis of rotation._ 
```C++
static Matrix4D AGE::Math::MakeRotation (
    float t,
    const Vector4 & a
) 
```



Creates a rotation matrix based on the given angle and axis.


The function creates a 4x4 rotation matrix using Rodrigues' rotation formula. It takes an angle 't' in radians and a [**Vector4**](struct_a_g_e_1_1_vector4.md) 'a', representing the axis of rotation.




**Parameters:**


* `t` Angle of rotation in radians. 
* `a` Axis of rotation represented as a [**Vector4**](struct_a_g_e_1_1_vector4.md).



**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) representing the rotation matrix. 


This function creates a 4x4 rotation matrix that rotates an object by the specified angle around the given axis. The axis is represented as a [**Vector4**](struct_a_g_e_1_1_vector4.md), where the first three components are the x, y, and z coordinates of the vector, respectively.




**Parameters:**


* `t` The angle of rotation in radians. 
* `a` A [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the axis of rotation. The first three elements represent the x, y, and z coordinates of the vector, respectively.



**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object that represents the created rotation matrix. 





        

<hr>



### function MakeRotationX 

_Creates a rotation matrix around the X axis._ 
```C++
static Matrix3D AGE::Math::MakeRotationX (
    float t
) 
```



This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the X-axis. The cosine and sine functions are used to calculate the values in the matrix, based on the input parameter 't'.




**Parameters:**


* `t` The angle of rotation in radians. 



**Returns:**

A 3x3 [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) representing a rotation transformation.


Creates a rotation matrix around the X axis.


This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the X-axis. The cosine and sine functions are used to calculate the values for the matrix elements, ensuring the correct rotation.




**Parameters:**


* `t` The angle of rotation in radians. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing a 3x3 rotation matrix. 





        

<hr>



### function MakeRotationY 

_Creates a rotation matrix around the Y axis._ 
```C++
static Matrix3D AGE::Math::MakeRotationY (
    float t
) 
```



This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the Y-axis. The cosine and sine of 't' are used to calculate the values in the matrix.




**Parameters:**


* `t` The angle of rotation, in radians. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing a 3x3 rotation matrix.


Creates a rotation matrix around the Y axis.


This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the Y-axis. The cosine and sine of 't' are used to calculate the values in the matrix.




**Parameters:**


* `t` The angle of rotation, in radians. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing a 3x3 rotation matrix. 





        

<hr>



### function MakeRotationZ 

_Creates a rotation matrix around the Z axis._ 
```C++
static Matrix3D AGE::Math::MakeRotationZ (
    float t
) 
```



This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the Z-axis. The cosine and sine of 't' are used to calculate the values in the matrix.




**Parameters:**


* `t` The angle (in radians) by which to rotate. 



**Returns:**

A 3x3 [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) representing a rotation of 't' radians about the Z-axis.


Creates a rotation matrix around the Z axis.


This function creates and returns a 3x3 rotation matrix that represents a rotation of 't' radians about the Z-axis. The cosine and sine of 't' are used to calculate the values in the matrix.




**Parameters:**


* `t` The angle of rotation, in radians. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) object representing a 3x3 rotation matrix. 





        

<hr>



### function MakeScale [1/2]

_Creates a scaling matrix from a scale factor and a vector._ 
```C++
static Matrix3D AGE::Math::MakeScale (
    float s,
    const Vector3 & a
) 
```



This function takes in a scale factor `s` and a [**Vector3**](struct_a_g_e_1_1_vector3.md) `a`, then it creates a 3D scaling matrix based on these inputs. The scale factor is subtracted by 1 to ensure the resulting matrix remains orthogonal.




**Parameters:**


* `s` The scale factor. 
* `a` The vector used for scaling. 



**Returns:**

A [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) representing the created scaling matrix.


Creates a scaling matrix from a scale factor and a vector.


This function creates a 3x3 scaling matrix based on the given scale factor (s) and vector (a). The resulting matrix is used to scale vectors in homogeneous coordinates, which allows for easy transformation of objects in 3D space.




**Parameters:**


* `s` The scale factor by which to multiply each component of the input vector. 
* `a` The vector whose components are multiplied by the scale factor to create the diagonal elements of the resulting matrix.



**Returns:**

A 3x3 scaling matrix that scales vectors in homogeneous coordinates according to the given scale factor and vector. 





        

<hr>



### function MakeScale [2/2]

_This function scales a given_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _by the x, y and z components of a_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _._
```C++
static Matrix4D AGE::Math::MakeScale (
    Matrix4D M,
    const Vector4 & a
) 
```





**Parameters:**


* `M` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be scaled. 
* `a` A reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) containing the scaling factors.



**Returns:**

Returns the scaled [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md).


This function scales a given [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) by the x, y and z components of a [**Vector4**](struct_a_g_e_1_1_vector4.md).




**Parameters:**


* `M` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be scaled. 
* `a` A reference to a constant [**Vector4**](struct_a_g_e_1_1_vector4.md) containing the scaling factors in x, y and z.



**Returns:**

The resulting [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) after being scaled by the input [**Vector4**](struct_a_g_e_1_1_vector4.md). 





        

<hr>



### function MakeSkew 

_Creates a skew symmetric matrix from given parameters._ 
```C++
static Matrix3D AGE::Math::MakeSkew (
    float t,
    const Vector3 & a,
    const Vector3 & b
) 
```



This function takes three parameters, two vectors and one scalar. The scalar is first converted to its tangent value using the tan() function. Then it multiplies each component of the first vector by this tangent value. These results are used to construct a skew symmetric matrix.




**Parameters:**


* `t` Scalar input which is first converted to its tangent value. 
* `a` Vector for multiplication with the tangent value. 
* `b` Vector for further multiplication in the construction of the resulting 3x3 Matrix.



**Returns:**

A 3x3 Matrix that represents skew symmetric transformation.


Creates a skew symmetric matrix from given parameters.


This function takes three parameters, two vectors and one scalar. It calculates the skew-symmetric matrix for the vector 'a' scaled by tan(t) and multiplies it with the third vector 'b'. The resulting [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) is returned.




**Parameters:**


* `t` Scalar value to scale the vector 'a'. 
* `a` Vector to be scaled and used in the skew-symmetric matrix calculation. 
* `b` Third vector which will be multiplied with the result of the skew-symmetric matrix calculation.



**Returns:**

The resulting [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) after performing the required calculations. 





        

<hr>



### function MakeTransform 

_Creates a transformation matrix from position, rotation and scale vectors._ 
```C++
static Matrix4D AGE::Math::MakeTransform (
    const Vector3 & Position,
    const Vector3 & Rotation,
    const Vector3 & Scale
) 
```



This function takes in three vectors representing the position, rotation, and scale of an object respectively. It uses these vectors to create a transformation matrix that can be used for transformations in 3D space. The rotation is expected to be provided as Euler angles (pitch, yaw, roll).




**Parameters:**


* `Position` A [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the position of the object. 
* `Rotation` A [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the rotation of the object in Euler angles (pitch, yaw, roll). 
* `Scale` A [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the scale of the object.



**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The transformation matrix created from the input vectors.


Creates a transformation matrix from position, rotation and scale vectors.


This function takes three Vector3D objects as input representing the position, rotation and scale of an object in 3D space. It converts these into a single [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object that represents the complete transformation of the object. The resulting matrix is created by first applying a translation to the identity matrix based on the Position vector, then rotating this translated matrix using the Rotation vector, and finally scaling the rotated matrix with the Scale vector.




**Parameters:**


* `Position` A Vector3D representing the position of the object in 3D space. 
* `Rotation` A Vector3D representing the rotation of the object in 3D space (in degrees). 
* `Scale` A Vector3D representing the scale of the object in 3D space.



**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) that represents the complete transformation of the object. 





        

<hr>



### function Modulo 

_Computes the modulus of two numbers using fmod function from cmath library._ 
```C++
static inline double AGE::Math::Modulo (
    double a,
    double b
) 
```





**Parameters:**


* `a` The first number in the operation. 
* `b` The second number in the operation. Must be non-zero to avoid division by zero.



**Returns:**

Returns the remainder of the division of 'a' by 'b'. If 'b' is zero, returns NaN (Not a Number).


Computes the modulus of two numbers using the fmod function from cmath.




**Parameters:**


* `a` The first number. 
* `b` The second number. Must not be zero to avoid division by zero.



**Returns:**

The remainder of the division of 'a' by 'b'. If 'b' is zero, returns NaN (not a number). 





        

<hr>



### function Multiply 

_This function multiplies two values of type T and returns the result._ 
```C++
template<typename T>
static inline T AGE::Math::Multiply (
    T a,
    T b
) 
```





**Parameters:**


* `a` The first value to multiply. 
* `b` The second value to multiply. 



**Returns:**

The product of a and b.


This function multiplies two values of type T and returns the result. 

**Parameters:**


* `a` The first value to multiply. 
* `b` The second value to multiply. 



**Returns:**

The product of 'a' and 'b'. 





        

<hr>



### function Pow 

_Computes the power of a number._ 
```C++
static inline float AGE::Math::Pow (
    float a,
    float b=2.f
) 
```



This function takes two parameters and returns the result of raising the first parameter to the power of the second. If no exponent is provided, it defaults to 2.0.




**Parameters:**


* `a` The base number. 
* `b` The exponent. Defaults to 2.0 if not specified. 



**Returns:**

Returns the result of raising 'a' to the power of 'b'.


Computes the power of a number.


This function takes two parameters and returns the result of raising the first parameter to the power of the second. If no exponent is provided (i.e., it defaults to 2), then the function behaves as if the exponent was 2.




**Parameters:**


* `a` The base number. 
* `b` The exponent. Defaults to 2. 



**Returns:**

Returns the result of raising 'a' to the power of 'b'. 





        

<hr>



### function Project2D 

_Computes the projection of a vector on another._ 
```C++
static inline Vector2 AGE::Math::Project2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



This function takes two vectors as input and returns their projection. The projection is calculated by multiplying the first vector (a) with the ratio of its dot product with the second vector (b) divided by the square of the magnitude of the second vector (b).




**Parameters:**


* `a` The vector to be projected. 
* `b` The vector onto which the projection is computed. 



**Returns:**

The projection of vector 'a' on vector 'b'.


Projects a vector onto another.


This function takes two vectors as input and projects the first one onto the second one. The projection is calculated by dividing the dot product of the first vector (a) and the second vector (b) by the square of the magnitude of the second vector (b).




**Parameters:**


* `a` The vector to be projected. 
* `b` The vector that 'a' will be projected onto. 



**Returns:**

[**Vector2**](struct_a_g_e_1_1_vector2.md) The projection of vector 'a' onto vector 'b'. 





        

<hr>



### function Project3D 

_Projects a vector 'a' onto another vector 'b'._ 
```C++
static inline Vector3 AGE::Math::Project3D (
    const Vector3 & a,
    Vector3 & b
) 
```



This function takes two vectors as input. The first one is the vector to be projected (a) and the second one is the vector onto which we want to project (b). It returns a new [**Vector3**](struct_a_g_e_1_1_vector3.md) that results from projection of vector 'a' on 'b'.




**Parameters:**


* `a` The vector to be projected. 
* `b` The vector onto which we want to project. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) resulting from the projection of vectors 'a' and 'b'.


Projects a vector onto another.


This function takes two vectors as input and projects the first one (a) onto the second one (b). The projection is calculated by dividing the dot product of a and b by the dot product of b with itself.




**Parameters:**


* `a` Vector to be projected. 
* `b` Base vector for projection. 



**Returns:**

[**Vector3**](struct_a_g_e_1_1_vector3.md) Resulting projection. 





        

<hr>



### function Radians [1/2]

_Converts an angle from degrees to radians._ 
```C++
static inline float AGE::Math::Radians (
    const float Deg
) 
```



This function takes a degree value and converts it into radians by multiplying the degree value with pi (3.14159) and dividing by 180. The result is then returned as a float.




**Parameters:**


* `Deg` The angle in degrees to be converted. 



**Returns:**

The equivalent angle in radians.


Converts an angle from degrees to radians.


This function takes a degree value and converts it into radians by multiplying the degree value with pi (3.14159) divided by 180. The result is then returned as the output.




**Parameters:**


* `Deg` The angle in degrees to be converted to radians. 



**Returns:**

The input angle in radians. 





        

<hr>



### function Radians [2/2]

_Converts degrees to radians for each component of a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _object._
```C++
static inline Vector3 AGE::Math::Radians (
    const Vector3 Vec
) 
```



This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object as input and returns a new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component is the original value converted from degrees to radians. The conversion formula used here is: radian = degree \* pi / 180.




**Parameters:**


* `Vec` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object containing the values in degrees that need to be converted to radians. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component has been converted from degrees to radians.


Converts degrees to radians for each component of a [**Vector3**](struct_a_g_e_1_1_vector3.md) object.


This function takes a [**Vector3**](struct_a_g_e_1_1_vector3.md) object as input and returns a new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component is the original value converted from degrees to radians. The conversion formula used is: radian = degree \* pi / 180.




**Parameters:**


* `Vec` A [**Vector3**](struct_a_g_e_1_1_vector3.md) object containing the values in degrees that need to be converted to radians. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) object where each component has been converted from degrees to radians. 





        

<hr>



### function Reject2D 

_Computes the rejection of one vector from another in a 2D space._ 
```C++
static inline Vector2 AGE::Math::Reject2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



This function takes two vectors 'a' and 'b', computes their dot product (DotProduct2D(a, b)) and divides it by the square of the magnitude of vector 'b'. The result is then subtracted from vector 'a' to yield a new vector.




**Parameters:**


* `a` First input vector. 
* `b` Second input vector. 



**Returns:**

[**Vector2**](struct_a_g_e_1_1_vector2.md) Resulting rejection vector.


Computes the rejection of a vector 'a' along another vector 'b'.


This function takes two vectors as input and returns a new vector which is the result of rejecting vector 'a' along vector 'b'. The operation essentially subtracts from vector 'a' the projection of vector 'b' on to itself, scaled by its dot product with itself.




**Parameters:**


* `a` [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the vector to be rejected. 
* `b` [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the vector along which 'a' is being rejected.



**Returns:**

A new [**Vector2**](struct_a_g_e_1_1_vector2.md) object resulting from the rejection of 'a' along 'b'. 





        

<hr>



### function Reject3D 

_Rejects a vector from another in three dimensions._ 
```C++
static inline Vector3 AGE::Math::Reject3D (
    const Vector3 & a,
    Vector3 & b
) 
```



This function calculates the rejection of one vector (`a`) from another (`b`). The rejection is calculated as `a - b * ((a . b) / (b . b))`, where '.' denotes dot product.




**Parameters:**


* `a` Vector to be rejected. 
* `b` Vector to reject from. 



**Returns:**

Vector resulting from the rejection of vector `a` from `b`.


Rejects a vector from another in three dimensions.


This function calculates the rejection of one vector (`a`) from another (`b`). The result is calculated as `a - b * ((DotProduct3D(a, b)) / DotProduct3D(b, b))`.




**Parameters:**


* `a` Vector to be rejected. 
* `b` Vector that will reject from it. 



**Returns:**

Vector resulting from the rejection of vector `a` by `b`. 





        

<hr>



### function Sin 

_Computes the sine of an angle in radians._ 
```C++
static inline float AGE::Math::Sin (
    float a
) 
```



This function takes an input parameter 'a' which represents an angle in radians and returns its sine value. The result is computed using the standard C++ library function std::sin().




**Parameters:**


* `a` Angle in radians to compute the sine of. 



**Returns:**

Sine of the input angle.


Computes the sine of an angle in radians.


This function takes an input parameter 'a' which represents an angle in radians and returns its sine value. The result is computed using the standard C++ library function std::sin().




**Parameters:**


* `a` Angle in radians to compute the sine of. 



**Returns:**

Sine of the input angle. 





        

<hr>



### function Sqrt 

_Calculates the square root of a given number._ 
```C++
static inline float AGE::Math::Sqrt (
    float a
) 
```



This function takes in a single parameter, 'a', which is the number to calculate the square root for. It returns the square root of 'a' as a float value. If 'a' is negative, it will return NaN (Not a Number).




**Parameters:**


* `a` The input number whose square root needs to be calculated. 



**Returns:**

Returns the square root of 'a'.


Computes the square root of a given number.


This function takes in a single parameter, 'a', which is the number for which we want to compute the square root. It returns the square root of 'a' as a float value. If 'a' is negative, it will return NaN (Not a Number).




**Parameters:**


* `a` The input number whose square root is to be computed. 



**Returns:**

Returns the square root of 'a'. 





        

<hr>



### function Subtract 

_This function subtracts two values of type T and returns the result._ 
```C++
template<typename T>
static inline T AGE::Math::Subtract (
    T a,
    T b
) 
```





**Parameters:**


* `a` The first value to be subtracted. 
* `b` The second value to be subtracted from the first one. 



**Returns:**

The result of the subtraction operation. If the inputs are invalid, it may return an incorrect result or throw an exception.


This function subtracts two values of type T and returns the result. 

**Parameters:**


* `a` The first value to be subtracted. 
* `b` The second value to be subtracted from the first one. 



**Returns:**

The result of the subtraction operation. If the inputs are invalid, it may return an incorrect result or throw an exception. 





        

<hr>



### function Transform [1/2]

_This function applies a transformation to a vector using a quaternion._ 
```C++
static Vector3 AGE::Math::Transform (
    const Vector3 & v,
    const Quaternion & q
) 
```



The transformation is defined by the formula: result = v \* (q.w^2 - \|b\|^2) + b \* (2 \* dot(v, b)) + cross(b, v) \* (2 \* q.w) where 'v' is the input vector, 'q' is the quaternion representing the transformation, and 'b' is the vector part of 'q'.




**Parameters:**


* `v` The input vector to be transformed. 
* `q` The quaternion that defines the transformation. 



**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the transformed vector.


Transforms a vector using a quaternion rotation.


This function applies the rotation defined by the given quaternion to the input vector. The transformation is performed according to the standard mathematical formula for transforming vectors with quaternions, which involves multiplication of the vector and quaternion, followed by cross product and scalar multiplication.




**Parameters:**


* `v` The input vector to be transformed. 
* `q` The rotation defined as a quaternion. 



**Returns:**

A new [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the result of the transformation. 





        

<hr>



### function Transform [2/2]

_This function applies a 4x4 homogeneous transformation matrix to a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object. The transformation is performed in 3D space and the resultant line is returned._
```C++
static inline Line AGE::Math::Transform (
    const Line & line,
    const Transform4D & H
) 
```





**Parameters:**


* `line` - A const reference to the [**Line**](struct_a_g_e_1_1_line.md) object that needs to be transformed. 
* `H` - A const reference to the [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) object representing the homogeneous transformation matrix.



**Returns:**

The function returns a new [**Line**](struct_a_g_e_1_1_line.md) object which is the result of applying the 4x4 transformation matrix to the input line.


Transforms a [**Line**](struct_a_g_e_1_1_line.md) object using a 4x4 transformation matrix.


This function takes in a [**Line**](struct_a_g_e_1_1_line.md) and a 4x4 transformation matrix ([**Transform4D**](struct_a_g_e_1_1_transform4_d.md)), applies the transformation to the line, and returns the transformed [**Line**](struct_a_g_e_1_1_line.md). The transformation is performed by multiplying the direction vector of the line with the upper-left 3x3 portion of the transformation matrix, and then calculating the moment using the adjugate of this matrix and the translation part of the transformation matrix.




**Parameters:**


* `line` - The [**Line**](struct_a_g_e_1_1_line.md) object to be transformed. 
* `H` - The 4x4 transformation matrix. 



**Returns:**

A new [**Line**](struct_a_g_e_1_1_line.md) object that is the result of the transformation. 





        

<hr>



### function Translate 

_Translates a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _by a_[_**Vector4**_](struct_a_g_e_1_1_vector4.md) _._
```C++
static Matrix4D AGE::Math::Translate (
    Matrix4D M,
    const Vector4 & a
) 
```



This function takes in an existing [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) and a [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the translation vector. It adds the x, y, and z components of the [**Vector4**](struct_a_g_e_1_1_vector4.md) to the corresponding elements in the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md), effectively translating it. The modified [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) is then returned.




**Parameters:**


* `M` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be translated. 
* `a` The translation vector.



**Returns:**

The translated [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md).


Translates a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) by a [**Vector4**](struct_a_g_e_1_1_vector4.md).


This function takes in a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) and a [**Vector4**](struct_a_g_e_1_1_vector4.md) as parameters. It adds the x, y, and z components of the [**Vector4**](struct_a_g_e_1_1_vector4.md) to the corresponding elements in the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md). The modified [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) is then returned.




**Parameters:**


* `M` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be translated. 
* `a` The [**Vector4**](struct_a_g_e_1_1_vector4.md) that specifies the translation. 



**Returns:**

The translated [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md). 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Math.h`

