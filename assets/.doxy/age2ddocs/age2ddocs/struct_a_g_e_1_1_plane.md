

# Struct AGE::Plane



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Plane**](struct_a_g_e_1_1_plane.md)


























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
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetNormal**](#function-getnormal) (void) const<br>_Returns a reference to the normal vector of this object._  |
|   | [**Plane**](#function-plane-13) () = default<br>_Default constructor for the_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _class._ |
|   | [**Plane**](#function-plane-23) (float nx, float ny, float nz, float d) <br>_Constructs a_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _object with the given parameters._ |
|   | [**Plane**](#function-plane-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & n, float d) <br>_Constructs a_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _object with the given normal vector and distance from origin._ |




























## Public Attributes Documentation




### variable w 

```C++
float AGE::Plane::w;
```




<hr>



### variable x 

```C++
float AGE::Plane::x;
```




<hr>



### variable y 

```C++
float AGE::Plane::y;
```




<hr>



### variable z 

```C++
float AGE::Plane::z;
```




<hr>
## Public Functions Documentation




### function GetNormal 

_Returns a reference to the normal vector of this object._ 
```C++
inline const Vector3 & AGE::Plane::GetNormal (
    void
) const
```





**Returns:**

A constant reference to the internal normal vector.


Returns a reference to the normal vector of this object. 

**Returns:**

A constant reference to the internal normal vector. 





        

<hr>



### function Plane [1/3]

_Default constructor for the_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _class._
```C++
AGE::Plane::Plane () = default
```



This function initializes a new instance of the [**Plane**](struct_a_g_e_1_1_plane.md) class with default values. It does not take any parameters and returns no value.


Default constructor for the [**Plane**](struct_a_g_e_1_1_plane.md) class.


This function initializes a new instance of the [**Plane**](struct_a_g_e_1_1_plane.md) class with default values. It is used to create an empty plane object that can be populated with data later.




**Returns:**

A new [**Plane**](struct_a_g_e_1_1_plane.md) object with all fields initialized to their default values. 





        

<hr>



### function Plane [2/3]

_Constructs a_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _object with the given parameters._
```C++
inline AGE::Plane::Plane (
    float nx,
    float ny,
    float nz,
    float d
) 
```



This function initializes a [**Plane**](struct_a_g_e_1_1_plane.md) object with four floating-point values, which represent the coordinates of a plane in 3D space. The first three parameters (nx, ny, nz) define the normal vector of the plane and the fourth parameter (d) is the distance from the origin to the plane along this direction. 

**Parameters:**


* `nx` The x-coordinate of the normal vector of the plane. 
* `ny` The y-coordinate of the normal vector of the plane. 
* `nz` The z-coordinate of the normal vector of the plane. 
* `d` The distance from the origin to the plane along its normal direction.

Constructs a [**Plane**](struct_a_g_e_1_1_plane.md) object with the given parameters.




**Parameters:**


* `nx` The x-coordinate of the plane's normal vector. 
* `ny` The y-coordinate of the plane's normal vector. 
* `nz` The z-coordinate of the plane's normal vector. 
* `d` The distance from the origin to the plane along its normal vector. 




        

<hr>



### function Plane [3/3]

_Constructs a_ [_**Plane**_](struct_a_g_e_1_1_plane.md) _object with the given normal vector and distance from origin._
```C++
inline AGE::Plane::Plane (
    const Vector3 & n,
    float d
) 
```





**Parameters:**


* `n` The normal vector of the plane. 
* `d` The distance from the origin to the plane along its normal direction.

Constructs a [**Plane**](struct_a_g_e_1_1_plane.md) object from a [**Vector3**](struct_a_g_e_1_1_vector3.md) and a float.


The plane is defined by the equation ax + by + cz = w, where (x, y, z) are the components of the input vector and 'w' is the input float.




**Parameters:**


* `n` A [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the direction of the plane. 
* `d` A float representing a point on the plane along the normal from which the distance to the origin is measured. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

