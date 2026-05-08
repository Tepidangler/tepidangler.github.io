

# Struct AGE::Vector2



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Vector2**](struct_a_g_e_1_1_vector2.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**x**](#variable-x)  <br> |
|  float | [**y**](#variable-y)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Vector2**](#function-vector2-14) () <br> |
|   | [**Vector2**](#function-vector2-24) (float a) <br> |
|   | [**Vector2**](#function-vector2-34) (float a, float b) <br> |
|   | [**Vector2**](#function-vector2-44) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Other) <br> |
|  float | [**dot**](#function-dot) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  float | [**magnitude**](#function-magnitude) () const<br> |
|  float | [**norm**](#function-norm) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**normalize**](#function-normalize) () const<br> |
|   | [**vec2**](#function-vec2) () const<br> |
|   | [**string**](#function-string) () <br> |
|  bool | [**operator!=**](#function-operator) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator\***](#function-operator_1) (float scalar) const<br> |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator+**](#function-operator_3) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  void | [**operator+=**](#function-operator_4) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator-**](#function-operator-) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator-**](#function-operator-_1) (const float val) const<br> |
|  void | [**operator-=**](#function-operator-_2) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator/**](#function-operator_5) (float scalar) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**operator/**](#function-operator_6) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  void | [**operator/=**](#function-operator_7) (float scalar) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator=**](#function-operator_8) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Other) <br> |
|  bool | [**operator==**](#function-operator_9) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & vec) const<br> |
|  float & | [**operator[]**](#function-operator_10) (int i) <br> |
|  const float & | [**operator[]**](#function-operator_11) (int i) const<br> |




























## Public Attributes Documentation




### variable x 

```C++
float AGE::Vector2::x;
```




<hr>



### variable y 

```C++
float AGE::Vector2::y;
```




<hr>
## Public Functions Documentation




### function Vector2 [1/4]

```C++
AGE::Vector2::Vector2 () 
```




<hr>



### function Vector2 [2/4]

```C++
explicit AGE::Vector2::Vector2 (
    float a
) 
```




<hr>



### function Vector2 [3/4]

```C++
AGE::Vector2::Vector2 (
    float a,
    float b
) 
```




<hr>



### function Vector2 [4/4]

```C++
inline AGE::Vector2::Vector2 (
    const Vector2 & Other
) 
```




<hr>



### function dot 

```C++
inline float AGE::Vector2::dot (
    const Vector2 & vec
) const
```




<hr>



### function magnitude 

```C++
inline float AGE::Vector2::magnitude () const
```




<hr>



### function norm 

```C++
inline float AGE::Vector2::norm (
    const Vector2 & vec
) const
```




<hr>



### function normalize 

```C++
Vector2 AGE::Vector2::normalize () const
```




<hr>



### function vec2 

```C++
inline AGE::Vector2::vec2 () const
```




<hr>



### function string 

```C++
inline AGE::Vector2::string () 
```




<hr>



### function operator!= 

```C++
inline bool AGE::Vector2::operator!= (
    const Vector2 & vec
) const
```




<hr>



### function operator\* 

```C++
inline Vector2 AGE::Vector2::operator* (
    float scalar
) const
```




<hr>



### function operator\*= 

```C++
inline void AGE::Vector2::operator*= (
    float scalar
) 
```




<hr>



### function operator+ 

```C++
inline Vector2 AGE::Vector2::operator+ (
    const Vector2 & vec
) const
```




<hr>



### function operator+= 

```C++
inline void AGE::Vector2::operator+= (
    const Vector2 & vec
) 
```




<hr>



### function operator- 

```C++
inline Vector2 AGE::Vector2::operator- (
    const Vector2 & vec
) const
```




<hr>



### function operator- 

```C++
inline Vector2 AGE::Vector2::operator- (
    const float val
) const
```




<hr>



### function operator-= 

```C++
inline void AGE::Vector2::operator-= (
    const Vector2 & vec
) 
```




<hr>



### function operator/ 

```C++
inline Vector2 AGE::Vector2::operator/ (
    float scalar
) const
```




<hr>



### function operator/ 

```C++
inline Vector2 AGE::Vector2::operator/ (
    const Vector2 & vec
) const
```




<hr>



### function operator/= 

```C++
inline void AGE::Vector2::operator/= (
    float scalar
) 
```




<hr>



### function operator= 

```C++
inline Vector2 & AGE::Vector2::operator= (
    const Vector2 & Other
) 
```




<hr>



### function operator== 

```C++
inline bool AGE::Vector2::operator== (
    const Vector2 & vec
) const
```




<hr>



### function operator[] 

```C++
inline float & AGE::Vector2::operator[] (
    int i
) 
```




<hr>



### function operator[] 

```C++
inline const float & AGE::Vector2::operator[] (
    int i
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector2.h`

