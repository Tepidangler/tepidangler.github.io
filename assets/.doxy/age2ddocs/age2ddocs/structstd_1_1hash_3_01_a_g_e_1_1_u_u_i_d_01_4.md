

# Struct std::hash&lt; AGE::UUID &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**std**](namespacestd.md) **>** [**hash&lt; AGE::UUID &gt;**](structstd_1_1hash_3_01_a_g_e_1_1_u_u_i_d_01_4.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  std::size\_t | [**operator()**](#function-operator) (const [**AGE::UUID**](class_a_g_e_1_1_u_u_i_d.md) & uuid) noexcept const<br>_Computes a hash value for the given UUID._  |




























## Public Functions Documentation




### function operator() 

_Computes a hash value for the given UUID._ 
```C++
inline std::size_t std::hash< AGE::UUID >::operator() (
    const AGE::UUID & uuid
) noexcept const
```



This function computes a hash value based on the input UUID using the standard C++ library's `hash` class with `uint64_t` as its template argument. The purpose of this function is to provide a unique identifier for each UUID, which can be useful in certain data structures or algorithms that require unique keys.




**Parameters:**


* `uuid` The UUID to compute the hash value for. 



**Returns:**

A size\_t representing the computed hash value.


Computes a hash value for the given UUID.


This function takes an [**AGE::UUID**](class_a_g_e_1_1_u_u_i_d.md) object as input and returns its corresponding hash value. The hash is computed by converting the UUID to uint64\_t and then using std::hash&lt;uint64\_t&gt;().




**Parameters:**


* `uuid` The UUID for which a hash value is calculated. 



**Returns:**

A size\_t representing the hashed value of the input UUID. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/UUID.h`

