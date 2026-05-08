

# Struct AGE::Matrix4D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md)










Inherited by the following classes: [AGE::Transform4D](struct_a_g_e_1_1_transform4_d.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix4D**](#function-matrix4d-17) () = default<br> |
|   | [**Matrix4D**](#function-matrix4d-27) (float n00, float n01, float n02, float n03, float n10, float n11, float n12, float n13, float n20, float n21, float n22, float n23, float n30, float n31, float n32, float n33) <br> |
|   | [**Matrix4D**](#function-matrix4d-37) (float f) <br> |
|   | [**Matrix4D**](#function-matrix4d-47) (glm::mat4 M) <br> |
|   | [**Matrix4D**](#function-matrix4d-57) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & b, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & c, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & d) <br> |
|   | [**Matrix4D**](#function-matrix4d-67) (void \* Ptr) <br> |
|   | [**Matrix4D**](#function-matrix4d-77) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & other) = default<br> |
|  glm::mat4 | [**ToGLM**](#function-toglm-12) () <br> |
|  glm::mat4 | [**ToGLM**](#function-toglm-22) () const<br> |
|  float & | [**operator()**](#function-operator) (int i, int j) <br> |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](#function-operator_2) (int j) <br> |
|  const [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator[]**](#function-operator_3) (int j) const<br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  float | [**n**](#variable-n)  <br> |




















## Public Functions Documentation




### function Matrix4D [1/7]

```C++
AGE::Matrix4D::Matrix4D () = default
```




<hr>



### function Matrix4D [2/7]

```C++
inline AGE::Matrix4D::Matrix4D (
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
    float n23,
    float n30,
    float n31,
    float n32,
    float n33
) 
```




<hr>



### function Matrix4D [3/7]

```C++
inline AGE::Matrix4D::Matrix4D (
    float f
) 
```




<hr>



### function Matrix4D [4/7]

```C++
inline AGE::Matrix4D::Matrix4D (
    glm::mat4 M
) 
```




<hr>



### function Matrix4D [5/7]

```C++
inline AGE::Matrix4D::Matrix4D (
    const Vector4 & a,
    const Vector4 & b,
    const Vector4 & c,
    const Vector4 & d
) 
```




<hr>



### function Matrix4D [6/7]

```C++
inline AGE::Matrix4D::Matrix4D (
    void * Ptr
) 
```




<hr>



### function Matrix4D [7/7]

```C++
AGE::Matrix4D::Matrix4D (
    const Matrix4D & other
) = default
```




<hr>



### function ToGLM [1/2]

```C++
inline glm::mat4 AGE::Matrix4D::ToGLM () 
```




<hr>



### function ToGLM [2/2]

```C++
inline glm::mat4 AGE::Matrix4D::ToGLM () const
```




<hr>



### function operator() 

```C++
inline float & AGE::Matrix4D::operator() (
    int i,
    int j
) 
```




<hr>



### function operator() 

```C++
inline const float & AGE::Matrix4D::operator() (
    int i,
    int j
) const
```




<hr>



### function operator[] 

```C++
inline Vector4 & AGE::Matrix4D::operator[] (
    int j
) 
```




<hr>



### function operator[] 

```C++
inline const Vector4 & AGE::Matrix4D::operator[] (
    int j
) const
```




<hr>
## Protected Attributes Documentation




### variable n 

```C++
float AGE::Matrix4D::n[4][4];
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

