

# Struct AGE::Line



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Line**](struct_a_g_e_1_1_line.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Direction**](#variable-direction)  <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Moment**](#variable-moment)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Line**](#function-line-13) () = default<br>_Default constructor for the_ [_**Line**_](struct_a_g_e_1_1_line.md) _class._ |
|   | [**Line**](#function-line-23) (float vx, float vy, float vz, float mx, float my, float mz) <br>_Constructs a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object with given direction and moment vectors._ |
|   | [**Line**](#function-line-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & m) <br>_Constructs a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object with given direction and moment vectors._ |




























## Public Attributes Documentation




### variable Direction 

```C++
Vector3 AGE::Line::Direction;
```




<hr>



### variable Moment 

```C++
Vector3 AGE::Line::Moment;
```




<hr>
## Public Functions Documentation




### function Line [1/3]

_Default constructor for the_ [_**Line**_](struct_a_g_e_1_1_line.md) _class._
```C++
AGE::Line::Line () = default
```



This function initializes a new instance of the [**Line**](struct_a_g_e_1_1_line.md) class with default values. It does not take any parameters and returns no value.


Default constructor for the [**Line**](struct_a_g_e_1_1_line.md) class. 


        

<hr>



### function Line [2/3]

_Constructs a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object with given direction and moment vectors._
```C++
inline AGE::Line::Line (
    float vx,
    float vy,
    float vz,
    float mx,
    float my,
    float mz
) 
```





**Parameters:**


* `vx` The x component of the direction vector. 
* `vy` The y component of the direction vector. 
* `vz` The z component of the direction vector. 
* `mx` The x component of the moment vector. 
* `my` The y component of the moment vector. 
* `mz` The z component of the moment vector.

Constructs a [**Line**](struct_a_g_e_1_1_line.md) object with given direction and moment vectors.




**Parameters:**


* `vx` The x component of the direction vector. 
* `vy` The y component of the direction vector. 
* `vz` The z component of the direction vector. 
* `mx` The x component of the moment vector. 
* `my` The y component of the moment vector. 
* `mz` The z component of the moment vector. 




        

<hr>



### function Line [3/3]

_Constructs a_ [_**Line**_](struct_a_g_e_1_1_line.md) _object with given direction and moment vectors._
```C++
inline AGE::Line::Line (
    const Vector3 & v,
    const Vector3 & m
) 
```





**Parameters:**


* `v` The direction vector of the line. 
* `m` The moment vector of the line.

Constructs a [**Line**](struct_a_g_e_1_1_line.md) object with given direction and moment vectors.




**Parameters:**


* `v` The direction vector of the line. 
* `m` The moment vector of the line. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

