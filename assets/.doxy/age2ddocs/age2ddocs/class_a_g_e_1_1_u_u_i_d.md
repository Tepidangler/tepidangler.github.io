

# Class AGE::UUID



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UUID**](class_a_g_e_1_1_u_u_i_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**UUID**](#function-uuid-13) () <br> |
|   | [**UUID**](#function-uuid-23) (uint64\_t uuid) <br>_Constructs a_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _object with the given uint64\_t value._ |
|   | [**UUID**](#function-uuid-33) (const [**UUID**](class_a_g_e_1_1_u_u_i_d.md) &) = default<br>_Default copy constructor for the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _class._ |
|   | [**operator uint64\_t**](#function-operator-uint64_t) () const<br>_Converts the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _object to a uint64\_t value._ |




























## Public Functions Documentation




### function UUID [1/3]

```C++
AGE::UUID::UUID () 
```




<hr>



### function UUID [2/3]

_Constructs a_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _object with the given uint64\_t value._
```C++
AGE::UUID::UUID (
    uint64_t uuid
) 
```



This constructor takes an unsigned 64-bit integer and assigns it to the member variable m\_UUID.




**Parameters:**


* `uuid` The uint64\_t value to be assigned to m\_UUID.

Constructs a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object with the given uint64\_t value.




**Parameters:**


* `uuid` The uint64\_t value to be used as the [**UUID**](class_a_g_e_1_1_u_u_i_d.md). 




        

<hr>



### function UUID [3/3]

_Default copy constructor for the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _class._
```C++
AGE::UUID::UUID (
    const UUID &
) = default
```



This function is used to create a new instance of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) class by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this function.




**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object to be copied.

Copy constructor for the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) class.


This function creates a new instance of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) class by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this function using the default copy semantics provided by the language.




**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object to be copied. 




        

<hr>



### function operator uint64\_t 

_Converts the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _object to a uint64\_t value._
```C++
inline AGE::UUID::operator uint64_t () const
```



This function returns the underlying uint64\_t representation of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object, which is its unique identifier.




**Returns:**

The 64-bit unsigned integer representation of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object.


Converts the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) to a uint64\_t value.


This function returns the internal representation of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) as a uint64\_t value. The conversion is done by simply returning the stored m\_UUID member variable.




**Returns:**

A uint64\_t representation of the [**UUID**](class_a_g_e_1_1_u_u_i_d.md). 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/UUID.h`

