

# Struct AGE::Matrix3D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix3D**](#function-matrix3d-14) () = default<br> |
|   | [**Matrix3D**](#function-matrix3d-24) (float n00, float n01, float n02, float n10, float n11, float n12, float n20, float n21, float n22) <br> |
|   | [**Matrix3D**](#function-matrix3d-34) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & c) <br> |
|   | [**Matrix3D**](#function-matrix3d-44) (void \* Ptr) <br> |
|  glm::mat3 | [**ToGLM**](#function-toglm-12) () <br> |
|  glm::mat3 | [**ToGLM**](#function-toglm-22) () const<br> |
|  float & | [**operator()**](#function-operator) (int i, int j) <br> |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_2) (int j) <br> |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**operator[]**](#function-operator_3) (int j) const<br> |




























## Public Functions Documentation




### function Matrix3D [1/4]

```C++
AGE::Matrix3D::Matrix3D () = default
```




<hr>



### function Matrix3D [2/4]

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




<hr>



### function Matrix3D [3/4]

```C++
inline AGE::Matrix3D::Matrix3D (
    const Vector3 & a,
    const Vector3 & b,
    const Vector3 & c
) 
```




<hr>



### function Matrix3D [4/4]

```C++
inline AGE::Matrix3D::Matrix3D (
    void * Ptr
) 
```




<hr>



### function ToGLM [1/2]

```C++
inline glm::mat3 AGE::Matrix3D::ToGLM () 
```




<hr>



### function ToGLM [2/2]

```C++
inline glm::mat3 AGE::Matrix3D::ToGLM () const
```




<hr>



### function operator() 

```C++
inline float & AGE::Matrix3D::operator() (
    int i,
    int j
) 
```




<hr>



### function operator() 

```C++
inline const float & AGE::Matrix3D::operator() (
    int i,
    int j
) const
```




<hr>



### function operator[] 

```C++
inline Vector3 & AGE::Matrix3D::operator[] (
    int j
) 
```




<hr>



### function operator[] 

```C++
inline const Vector3 & AGE::Matrix3D::operator[] (
    int j
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

