

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
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetNormal**](#function-getnormal) (void) const<br> |
|   | [**Plane**](#function-plane-13) () = default<br> |
|   | [**Plane**](#function-plane-23) (float nx, float ny, float nz, float d) <br> |
|   | [**Plane**](#function-plane-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & n, float d) <br> |




























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

```C++
inline const Vector3 & AGE::Plane::GetNormal (
    void
) const
```




<hr>



### function Plane [1/3]

```C++
AGE::Plane::Plane () = default
```




<hr>



### function Plane [2/3]

```C++
inline AGE::Plane::Plane (
    float nx,
    float ny,
    float nz,
    float d
) 
```




<hr>



### function Plane [3/3]

```C++
inline AGE::Plane::Plane (
    const Vector3 & n,
    float d
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

