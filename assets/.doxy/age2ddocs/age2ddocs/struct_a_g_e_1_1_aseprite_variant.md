

# Struct AGE::AsepriteVariant



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md)








Inherits the following classes: VariantBase


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteVariant**](#function-asepritevariant-13) () = default<br> |
|   | [**AsepriteVariant**](#function-asepritevariant-23) (const [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & v) = default<br> |
|   | [**AsepriteVariant**](#function-asepritevariant-33) (T && v) <br> |
|  [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & | [**operator=**](#function-operator) (const char \*) = delete<br> |
|  [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & | [**operator=**](#function-operator_1) (T && v) <br> |
|  const size\_t | [**type**](#function-type) () const<br> |




























## Public Functions Documentation




### function AsepriteVariant [1/3]

```C++
AGE::AsepriteVariant::AsepriteVariant () = default
```




<hr>



### function AsepriteVariant [2/3]

```C++
AGE::AsepriteVariant::AsepriteVariant (
    const AsepriteVariant & v
) = default
```




<hr>



### function AsepriteVariant [3/3]

```C++
template<typename T>
inline AGE::AsepriteVariant::AsepriteVariant (
    T && v
) 
```




<hr>



### function operator= 

```C++
AsepriteVariant & AGE::AsepriteVariant::operator= (
    const char *
) = delete
```




<hr>



### function operator= 

```C++
template<typename T>
inline AsepriteVariant & AGE::AsepriteVariant::operator= (
    T && v
) 
```




<hr>



### function type 

```C++
inline const size_t AGE::AsepriteVariant::type () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

