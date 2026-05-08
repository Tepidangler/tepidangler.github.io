

# Struct AGE::Matrix2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Matrix2D**](struct_a_g_e_1_1_matrix2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Matrix2D**](#function-matrix2d-13) () = default<br> |
|   | [**Matrix2D**](#function-matrix2d-23) (float n00, float n01, float n10, float n11) <br> |
|   | [**Matrix2D**](#function-matrix2d-33) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br> |
|  float & | [**operator()**](#function-operator) (int i, int j) <br> |
|  const float & | [**operator()**](#function-operator_1) (int i, int j) const<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator[]**](#function-operator_2) (int j) <br> |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**operator[]**](#function-operator_3) (int j) const<br> |




























## Public Functions Documentation




### function Matrix2D [1/3]

```C++
AGE::Matrix2D::Matrix2D () = default
```




<hr>



### function Matrix2D [2/3]

```C++
inline AGE::Matrix2D::Matrix2D (
    float n00,
    float n01,
    float n10,
    float n11
) 
```



\| n00, n01 \| \| n10, n11 \| 


        

<hr>



### function Matrix2D [3/3]

```C++
inline AGE::Matrix2D::Matrix2D (
    const Vector2 & a,
    const Vector2 & b
) 
```



\| a[0], a[1]\| \| b[0], b[1]\| 


        

<hr>



### function operator() 

```C++
inline float & AGE::Matrix2D::operator() (
    int i,
    int j
) 
```




<hr>



### function operator() 

```C++
inline const float & AGE::Matrix2D::operator() (
    int i,
    int j
) const
```




<hr>



### function operator[] 

```C++
inline Vector2 & AGE::Matrix2D::operator[] (
    int j
) 
```




<hr>



### function operator[] 

```C++
inline const Vector2 & AGE::Matrix2D::operator[] (
    int j
) const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

