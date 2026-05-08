

# Struct AGE::Transform4D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Transform4D**](struct_a_g_e_1_1_transform4_d.md)








Inherits the following classes: [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & | [**GetTranslation**](#function-gettranslation) (void) const<br> |
|  void | [**SetTranslation**](#function-settranslation) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br> |
|   | [**Transform4D**](#function-transform4d-13) () = default<br> |
|   | [**Transform4D**](#function-transform4d-23) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23) <br> |
|   | [**Transform4D**](#function-transform4d-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & c, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator) (int j) <br> |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_1) (int j) const<br> |


## Public Functions inherited from AGE::Matrix4D

See [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)

| Type | Name |
| ---: | :--- |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-17) () = default<br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-27) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23, float n30, float n31, float n32, float n33) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-37) (float f) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-47) (glm::mat4 M) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-57) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & b, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & c, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & d) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-67) (void \* Ptr) <br> |
|   | [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md#function-matrix4d-77) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & other) = default<br> |
|  glm::mat4 | [**ToGLM**](struct_a_g_e_1_1_matrix4_d.md#function-toglm-12) () <br> |
|  glm::mat4 | [**ToGLM**](struct_a_g_e_1_1_matrix4_d.md#function-toglm-22) () const<br> |
|  float & | [**operator()**](struct_a_g_e_1_1_matrix4_d.md#function-operator) (int i, int j) <br> |
|  const float & | [**operator()**](struct_a_g_e_1_1_matrix4_d.md#function-operator_1) (int i, int j) const<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](struct_a_g_e_1_1_matrix4_d.md#function-operator_2) (int j) <br> |
|  const [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](struct_a_g_e_1_1_matrix4_d.md#function-operator_3) (int j) const<br> |
















## Protected Attributes inherited from AGE::Matrix4D

See [AGE::Matrix4D](struct_a_g_e_1_1_matrix4_d.md)

| Type | Name |
| ---: | :--- |
|  float | [**n**](struct_a_g_e_1_1_matrix4_d.md#variable-n)  <br> |






































## Public Functions Documentation




### function GetTranslation 

```C++
inline const Point3D & AGE::Transform4D::GetTranslation (
    void
) const
```




<hr>



### function SetTranslation 

```C++
inline void AGE::Transform4D::SetTranslation (
    const Point3D & p
) 
```




<hr>



### function Transform4D [1/3]

```C++
AGE::Transform4D::Transform4D () = default
```




<hr>



### function Transform4D [2/3]

```C++
inline AGE::Transform4D::Transform4D (
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
    float n23
) 
```




<hr>



### function Transform4D [3/3]

```C++
inline AGE::Transform4D::Transform4D (
    const Vector3 & a,
    const Vector3 & b,
    const Vector3 & c,
    const Point3D & p
) 
```




<hr>



### function operator[] 

```C++
inline Vector3 & AGE::Transform4D::operator[] (
    int j
) 
```




<hr>



### function operator[] 

```C++
inline const Vector3 & AGE::Transform4D::operator[] (
    int j
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

