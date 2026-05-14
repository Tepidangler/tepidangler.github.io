

# Struct AGE::AsepriteVariant



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md)








Inherits the following classes: VariantBase


































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteVariant**](#function-asepritevariant-13) () = default<br>_Default constructor for_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _class._ |
|   | [**AsepriteVariant**](#function-asepritevariant-23) (const [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & v) = default<br>_Copy constructor for the_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _class._ |
|   | [**AsepriteVariant**](#function-asepritevariant-33) (T && v) <br>_Constructs a variant object with the given value._  |
|  [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & | [**operator=**](#function-operator) (const char \*) = delete<br>_Overloaded assignment operator that disallows the use of a const char\* as an argument._  |
|  [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) & | [**operator=**](#function-operator_1) (T && v) <br>_Assignment operator for_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _._ |
|  const size\_t | [**type**](#function-type) () const<br>_Returns the value of the 'index' function for this object._  |




























## Public Functions Documentation




### function AsepriteVariant [1/3]

_Default constructor for_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _class._
```C++
AGE::AsepriteVariant::AsepriteVariant () = default
```




<hr>



### function AsepriteVariant [2/3]

_Copy constructor for the_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _class._
```C++
AGE::AsepriteVariant::AsepriteVariant (
    const AsepriteVariant & v
) = default
```



This function creates a new instance of [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) that is a copy of an existing one. It uses the '= default' syntax to delegate the work to the compiler-generated copy constructor.




**Parameters:**


* `v` The existing [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) instance to be copied. 




        

<hr>



### function AsepriteVariant [3/3]

_Constructs a variant object with the given value._ 
```C++
template<typename T>
inline AGE::AsepriteVariant::AsepriteVariant (
    T && v
) 
```



This constructor takes an rvalue reference to construct a variant object from a temporary value. It uses std::forward to ensure that the correct move semantics are used based on whether T is an lvalue or rvalue.




**Template parameters:**


* `T` The type of the value being moved into the variant. 



**Parameters:**


* `v` The value being moved into the variant. 




        

<hr>



### function operator= 

_Overloaded assignment operator that disallows the use of a const char\* as an argument._ 
```C++
AsepriteVariant & AGE::AsepriteVariant::operator= (
    const char *
) = delete
```



This function is marked as deleted to prevent its usage with a const char\*. It will not compile if someone tries to assign a const char\* value to this object.




**Parameters:**


* `str` The string to be assigned, which should not be of type const char\*.



**Returns:**

A reference to the modified [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) object. 





        

<hr>



### function operator= 

_Assignment operator for_ [_**AsepriteVariant**_](struct_a_g_e_1_1_aseprite_variant.md) _._
```C++
template<typename T>
inline AsepriteVariant & AGE::AsepriteVariant::operator= (
    T && v
) 
```



This function overloads the assignment operator to allow for moving of values into an [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) object. It takes a rvalue reference (T&&) as its parameter, which allows it to accept both lvalues and rvalues. The function then calls the assignment operator of VariantBase with std::forward to handle the forwarding of the argument.




**Parameters:**


* `v` The value to be moved into this [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) object. 



**Returns:**

Reference to the modified [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) object. 





        

<hr>



### function type 

_Returns the value of the 'index' function for this object._ 
```C++
inline const size_t AGE::AsepriteVariant::type () const
```



This function is a simple wrapper around another function, 'index', which returns an unsigned integer. It simply calls that function and returns its result. The purpose of this function could be to provide a consistent interface or to add additional functionality in derived classes.




**Returns:**

The value returned by the 'index' function for this object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

