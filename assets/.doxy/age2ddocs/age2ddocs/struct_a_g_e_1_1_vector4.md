

# Struct AGE::Vector4



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Vector4**](struct_a_g_e_1_1_vector4.md)


























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
|   | [**Vector4**](#function-vector4-17) () <br> |
|   | [**Vector4**](#function-vector4-27) (float a) <br> |
|   | [**Vector4**](#function-vector4-37) (glm::vec4 vec) <br> |
|   | [**Vector4**](#function-vector4-47) (float a, float b, float c, float d) <br> |
|   | [**Vector4**](#function-vector4-57) (uint8\_t a, uint8\_t b, uint8\_t c, uint8\_t d) <br> |
|   | [**Vector4**](#function-vector4-67) (const float \* color) <br> |
|   | [**Vector4**](#function-vector4-77) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Other) <br> |
|  float | [**dot**](#function-dot) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  float | [**magnitude**](#function-magnitude) () const<br> |
|  float | [**norm**](#function-norm) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**normalize**](#function-normalize) () const<br> |
|   | [**string**](#function-string) () <br> |
|   | [**operator uint32\_t**](#function-operator-uint32_t) () <br> |
|   | [**operator uint32\_t \***](#function-operator-uint32_t-*) () <br> |
|  bool | [**operator!=**](#function-operator) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator\***](#function-operator_1) (float scalar) const<br> |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator+**](#function-operator_3) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  void | [**operator+=**](#function-operator_4) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) <br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator-**](#function-operator-) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  void | [**operator-=**](#function-operator-_1) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) <br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator/**](#function-operator_5) (float scalar) const<br> |
|  void | [**operator/=**](#function-operator_6) (float scalar) <br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator=**](#function-operator_7) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Other) <br> |
|  void | [**operator=**](#function-operator_8) ([**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  bool | [**operator==**](#function-operator_9) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br> |
|  float & | [**operator[]**](#function-operator_10) (int i) <br> |
|  const float & | [**operator[]**](#function-operator_11) (int i) const<br> |
|   | [**~Vector4**](#function-vector4) () = default<br> |




























## Public Attributes Documentation




### variable w 

```C++
float AGE::Vector4::w;
```




<hr>



### variable x 

```C++
float AGE::Vector4::x;
```




<hr>



### variable y 

```C++
float AGE::Vector4::y;
```




<hr>



### variable z 

```C++
float AGE::Vector4::z;
```




<hr>
## Public Functions Documentation




### function Vector4 [1/7]

```C++
AGE::Vector4::Vector4 () 
```




<hr>



### function Vector4 [2/7]

```C++
AGE::Vector4::Vector4 (
    float a
) 
```




<hr>



### function Vector4 [3/7]

```C++
AGE::Vector4::Vector4 (
    glm::vec4 vec
) 
```




<hr>



### function Vector4 [4/7]

```C++
AGE::Vector4::Vector4 (
    float a,
    float b,
    float c,
    float d
) 
```




<hr>



### function Vector4 [5/7]

```C++
AGE::Vector4::Vector4 (
    uint8_t a,
    uint8_t b,
    uint8_t c,
    uint8_t d
) 
```




<hr>



### function Vector4 [6/7]

```C++
AGE::Vector4::Vector4 (
    const float * color
) 
```




<hr>



### function Vector4 [7/7]

```C++
inline AGE::Vector4::Vector4 (
    const Vector4 & Other
) 
```




<hr>



### function dot 

```C++
inline float AGE::Vector4::dot (
    const Vector4 & vec
) const
```




<hr>



### function magnitude 

```C++
inline float AGE::Vector4::magnitude () const
```




<hr>



### function norm 

```C++
inline float AGE::Vector4::norm (
    const Vector4 & vec
) const
```




<hr>



### function normalize 

```C++
Vector4 AGE::Vector4::normalize () const
```




<hr>



### function string 

```C++
inline AGE::Vector4::string () 
```




<hr>



### function operator uint32\_t 

```C++
inline AGE::Vector4::operator uint32_t () 
```




<hr>



### function operator uint32\_t \* 

```C++
inline AGE::Vector4::operator uint32_t * () 
```




<hr>



### function operator!= 

```C++
inline bool AGE::Vector4::operator!= (
    const Vector4 & vec
) const
```




<hr>



### function operator\* 

```C++
inline Vector4 AGE::Vector4::operator* (
    float scalar
) const
```




<hr>



### function operator\*= 

```C++
inline void AGE::Vector4::operator*= (
    float scalar
) 
```




<hr>



### function operator+ 

```C++
inline Vector4 AGE::Vector4::operator+ (
    const Vector4 & vec
) const
```




<hr>



### function operator+= 

```C++
inline void AGE::Vector4::operator+= (
    const Vector4 & vec
) 
```




<hr>



### function operator- 

```C++
inline Vector4 AGE::Vector4::operator- (
    const Vector4 & vec
) const
```




<hr>



### function operator-= 

```C++
inline void AGE::Vector4::operator-= (
    const Vector4 & vec
) 
```




<hr>



### function operator/ 

```C++
inline Vector4 AGE::Vector4::operator/ (
    float scalar
) const
```




<hr>



### function operator/= 

```C++
inline void AGE::Vector4::operator/= (
    float scalar
) 
```




<hr>



### function operator= 

```C++
inline Vector4 & AGE::Vector4::operator= (
    const Vector4 & Other
) 
```




<hr>



### function operator= 

```C++
inline void AGE::Vector4::operator= (
    Vector3 & vec
) 
```




<hr>



### function operator== 

```C++
inline bool AGE::Vector4::operator== (
    const Vector4 & vec
) const
```




<hr>



### function operator[] 

```C++
inline float & AGE::Vector4::operator[] (
    int i
) 
```




<hr>



### function operator[] 

```C++
inline const float & AGE::Vector4::operator[] (
    int i
) const
```




<hr>



### function ~Vector4 

```C++
AGE::Vector4::~Vector4 () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector4.h`

