

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
|   | [**Point3D**](#function-point3d-12) () = default<br> |
|   | [**Point3D**](#function-point3d-22) (float a, float b, float c) <br> |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) | [**operator()**](#function-operator) ([**Vector3**](struct_a_g_e_1_1_vector3.md) v) const<br> |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) | [**operator=**](#function-operator_1) ([**Vector3**](struct_a_g_e_1_1_vector3.md) v) const<br> |


## Public Functions inherited from AGE::Vector3

See [AGE::Vector3](struct_a_g_e_1_1_vector3.md)

| Type | Name |
| ---: | :--- |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-16) () <br> |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-26) (float a) <br> |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-36) (float a, float b, float c) <br> |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-46) ([**Vector2**](struct_a_g_e_1_1_vector2.md) a, float c) <br> |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-56) (glm::vec3 v) <br> |
|   | [**Vector3**](struct_a_g_e_1_1_vector3.md#function-vector3-66) ([**Vector4**](struct_a_g_e_1_1_vector4.md) v) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**cross**](struct_a_g_e_1_1_vector3.md#function-cross) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float | [**dot**](struct_a_g_e_1_1_vector3.md#function-dot) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float | [**magnitude**](struct_a_g_e_1_1_vector3.md#function-magnitude) () const<br> |
|  float | [**norm**](struct_a_g_e_1_1_vector3.md#function-norm) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**normalize**](struct_a_g_e_1_1_vector3.md#function-normalize) () const<br> |
|   | [**quat**](struct_a_g_e_1_1_vector3.md#function-quat) () <br> |
|   | [**vec3**](struct_a_g_e_1_1_vector3.md#function-vec3) () <br> |
|   | [**string**](struct_a_g_e_1_1_vector3.md#function-string) () <br> |
|  bool | [**operator!=**](struct_a_g_e_1_1_vector3.md#function-operator) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator\***](struct_a_g_e_1_1_vector3.md#function-operator_1) (float scalar) const<br> |
|  void | [**operator\*=**](struct_a_g_e_1_1_vector3.md#function-operator_2) (float scalar) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator+**](struct_a_g_e_1_1_vector3.md#function-operator_3) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  void | [**operator+=**](struct_a_g_e_1_1_vector3.md#function-operator_4) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator-**](struct_a_g_e_1_1_vector3.md#function-operator-) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  void | [**operator-=**](struct_a_g_e_1_1_vector3.md#function-operator-_1) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator/**](struct_a_g_e_1_1_vector3.md#function-operator_5) (float scalar) const<br> |
|  void | [**operator/=**](struct_a_g_e_1_1_vector3.md#function-operator_6) (float scalar) <br> |
|  bool | [**operator==**](struct_a_g_e_1_1_vector3.md#function-operator_7) ([**Vector3**](struct_a_g_e_1_1_vector3.md) vec) const<br> |
|  bool | [**operator==**](struct_a_g_e_1_1_vector3.md#function-operator_8) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float & | [**operator[]**](struct_a_g_e_1_1_vector3.md#function-operator_9) (int i) <br> |
|  const float & | [**operator[]**](struct_a_g_e_1_1_vector3.md#function-operator_10) (int i) const<br> |






















































## Public Functions Documentation




### function Point3D [1/2]

```C++
AGE::Point3D::Point3D () = default
```




<hr>



### function Point3D [2/2]

```C++
inline AGE::Point3D::Point3D (
    float a,
    float b,
    float c
) 
```




<hr>



### function operator() 

```C++
inline const Point3D AGE::Point3D::operator() (
    Vector3 v
) const
```




<hr>



### function operator= 

```C++
inline const Point3D AGE::Point3D::operator= (
    Vector3 v
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

