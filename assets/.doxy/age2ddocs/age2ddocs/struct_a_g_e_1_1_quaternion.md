

# Struct AGE::Quaternion



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Quaternion**](struct_a_g_e_1_1_quaternion.md)


























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
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**GetRotationMatrix**](#function-getrotationmatrix) (void) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetVectorPart**](#function-getvectorpart-12) (void) <br> |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetVectorPart**](#function-getvectorpart-22) (void) const<br> |
|   | [**Quaternion**](#function-quaternion-13) () = default<br> |
|   | [**Quaternion**](#function-quaternion-23) (float a, float b, float c, float s) <br> |
|   | [**Quaternion**](#function-quaternion-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, float s) <br> |
|  void | [**SetRotationMatrix**](#function-setrotationmatrix) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & m) <br> |




























## Public Attributes Documentation




### variable w 

```C++
float AGE::Quaternion::w;
```




<hr>



### variable x 

```C++
float AGE::Quaternion::x;
```




<hr>



### variable y 

```C++
float AGE::Quaternion::y;
```




<hr>



### variable z 

```C++
float AGE::Quaternion::z;
```




<hr>
## Public Functions Documentation




### function GetRotationMatrix 

```C++
Matrix3D AGE::Quaternion::GetRotationMatrix (
    void
) 
```




<hr>



### function GetVectorPart [1/2]

```C++
inline Vector3 & AGE::Quaternion::GetVectorPart (
    void
) 
```




<hr>



### function GetVectorPart [2/2]

```C++
inline const Vector3 & AGE::Quaternion::GetVectorPart (
    void
) const
```




<hr>



### function Quaternion [1/3]

```C++
AGE::Quaternion::Quaternion () = default
```




<hr>



### function Quaternion [2/3]

```C++
inline AGE::Quaternion::Quaternion (
    float a,
    float b,
    float c,
    float s
) 
```




<hr>



### function Quaternion [3/3]

```C++
inline AGE::Quaternion::Quaternion (
    const Vector3 & v,
    float s
) 
```




<hr>



### function SetRotationMatrix 

```C++
void AGE::Quaternion::SetRotationMatrix (
    const Matrix3D & m
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

