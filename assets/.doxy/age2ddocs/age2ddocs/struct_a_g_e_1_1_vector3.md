

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
|   | [**Vector3**](#function-vector3-16) () <br> |
|   | [**Vector3**](#function-vector3-26) (float a) <br> |
|   | [**Vector3**](#function-vector3-36) (float a, float b, float c) <br> |
|   | [**Vector3**](#function-vector3-46) ([**Vector2**](struct_a_g_e_1_1_vector2.md) a, float c) <br> |
|   | [**Vector3**](#function-vector3-56) (glm::vec3 v) <br> |
|   | [**Vector3**](#function-vector3-66) ([**Vector4**](struct_a_g_e_1_1_vector4.md) v) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**cross**](#function-cross) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float | [**dot**](#function-dot) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float | [**magnitude**](#function-magnitude) () const<br> |
|  float | [**norm**](#function-norm) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**normalize**](#function-normalize) () const<br> |
|   | [**quat**](#function-quat) () <br> |
|   | [**vec3**](#function-vec3) () <br> |
|   | [**string**](#function-string) () <br> |
|  bool | [**operator!=**](#function-operator) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator\***](#function-operator_1) (float scalar) const<br> |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator+**](#function-operator_3) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  void | [**operator+=**](#function-operator_4) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator-**](#function-operator-) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  void | [**operator-=**](#function-operator-_1) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**operator/**](#function-operator_5) (float scalar) const<br> |
|  void | [**operator/=**](#function-operator_6) (float scalar) <br> |
|  bool | [**operator==**](#function-operator_7) ([**Vector3**](struct_a_g_e_1_1_vector3.md) vec) const<br> |
|  bool | [**operator==**](#function-operator_8) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) const<br> |
|  float & | [**operator[]**](#function-operator_9) (int i) <br> |
|  const float & | [**operator[]**](#function-operator_10) (int i) const<br> |




























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

```C++
AGE::Vector3::Vector3 () 
```




<hr>



### function Vector3 [2/6]

```C++
AGE::Vector3::Vector3 (
    float a
) 
```




<hr>



### function Vector3 [3/6]

```C++
AGE::Vector3::Vector3 (
    float a,
    float b,
    float c
) 
```




<hr>



### function Vector3 [4/6]

```C++
AGE::Vector3::Vector3 (
    Vector2 a,
    float c
) 
```




<hr>



### function Vector3 [5/6]

```C++
AGE::Vector3::Vector3 (
    glm::vec3 v
) 
```




<hr>



### function Vector3 [6/6]

```C++
AGE::Vector3::Vector3 (
    Vector4 v
) 
```




<hr>



### function cross 

```C++
inline Vector3 AGE::Vector3::cross (
    const Vector3 & vec
) const
```




<hr>



### function dot 

```C++
inline float AGE::Vector3::dot (
    const Vector3 & vec
) const
```




<hr>



### function magnitude 

```C++
inline float AGE::Vector3::magnitude () const
```




<hr>



### function norm 

```C++
inline float AGE::Vector3::norm (
    const Vector3 & vec
) const
```




<hr>



### function normalize 

```C++
Vector3 AGE::Vector3::normalize () const
```




<hr>



### function quat 

```C++
inline AGE::Vector3::quat () 
```




<hr>



### function vec3 

```C++
inline AGE::Vector3::vec3 () 
```




<hr>



### function string 

```C++
inline AGE::Vector3::string () 
```




<hr>



### function operator!= 

```C++
inline bool AGE::Vector3::operator!= (
    const Vector3 & vec
) 
```




<hr>



### function operator\* 

```C++
inline Vector3 AGE::Vector3::operator* (
    float scalar
) const
```




<hr>



### function operator\*= 

```C++
inline void AGE::Vector3::operator*= (
    float scalar
) 
```




<hr>



### function operator+ 

```C++
inline Vector3 AGE::Vector3::operator+ (
    const Vector3 & vec
) const
```




<hr>



### function operator+= 

```C++
inline void AGE::Vector3::operator+= (
    const Vector3 & vec
) 
```




<hr>



### function operator- 

```C++
inline Vector3 AGE::Vector3::operator- (
    const Vector3 & vec
) const
```




<hr>



### function operator-= 

```C++
inline void AGE::Vector3::operator-= (
    const Vector3 & vec
) 
```




<hr>



### function operator/ 

```C++
inline Vector3 AGE::Vector3::operator/ (
    float scalar
) const
```




<hr>



### function operator/= 

```C++
inline void AGE::Vector3::operator/= (
    float scalar
) 
```




<hr>



### function operator== 

```C++
inline bool AGE::Vector3::operator== (
    Vector3 vec
) const
```




<hr>



### function operator== 

```C++
inline bool AGE::Vector3::operator== (
    const Vector3 & vec
) const
```




<hr>



### function operator[] 

```C++
inline float & AGE::Vector3::operator[] (
    int i
) 
```




<hr>



### function operator[] 

```C++
inline const float & AGE::Vector3::operator[] (
    int i
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector3.h`

