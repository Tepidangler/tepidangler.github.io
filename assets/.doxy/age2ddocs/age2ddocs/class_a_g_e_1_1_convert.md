

# Class AGE::Convert



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Convert**](class_a_g_e_1_1_convert.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Convert**](#function-convert) () <br>_Converts the input into another format._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  glm::vec3 | [**ToGLM**](#function-toglm-12) ([**Vector3**](struct_a_g_e_1_1_vector3.md) vec) <br>_Converts a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to GLM's vec3 format._ |
|  glm::vec4 | [**ToGLM**](#function-toglm-22) ([**Vector4**](struct_a_g_e_1_1_vector4.md) vec) <br>_Converts a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to a GLM vec4._ |


























## Public Functions Documentation




### function Convert 

_Converts the input into another format._ 
```C++
inline AGE::Convert::Convert () 
```



This function takes an input and converts it to a different format. The exact conversion performed is not specified, as this depends on the implementation details of the [**Convert()**](class_a_g_e_1_1_convert.md#function-convert) function.




**Returns:**

Returns void.


Converts the input into another format.


This function takes an input and converts it to a different format. The exact conversion performed is not specified, as this depends on the implementation details of the [**Convert()**](class_a_g_e_1_1_convert.md#function-convert) function.




**Returns:**

Returns void. 





        

<hr>
## Public Static Functions Documentation




### function ToGLM [1/2]

_Converts a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to GLM's vec3 format._
```C++
static glm::vec3 AGE::Convert::ToGLM (
    Vector3 vec
) 
```



This function takes in a [**Vector3**](struct_a_g_e_1_1_vector3.md) object and returns its equivalent glm::vec3 representation. It directly maps the x, y, and z properties of the input [**Vector3**](struct_a_g_e_1_1_vector3.md) to the respective components of the output glm::vec3.




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) object to be converted. 



**Returns:**

A glm::vec3 object with the same values as the input [**Vector3**](struct_a_g_e_1_1_vector3.md).


Converts a [**Vector3**](struct_a_g_e_1_1_vector3.md) object to a GLM vec3 object.


This function takes in a [**Vector3**](struct_a_g_e_1_1_vector3.md) object and returns its equivalent glm::vec3 representation. The conversion is done by simply copying the x, y, and z values from the input [**Vector3**](struct_a_g_e_1_1_vector3.md) object into the new glm::vec3 object.




**Parameters:**


* `vec` The [**Vector3**](struct_a_g_e_1_1_vector3.md) object to be converted. 



**Returns:**

A glm::vec3 object with the same x, y, and z values as the input [**Vector3**](struct_a_g_e_1_1_vector3.md) object. 





        

<hr>



### function ToGLM [2/2]

_Converts a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to a GLM vec4._
```C++
static glm::vec4 AGE::Convert::ToGLM (
    Vector4 vec
) 
```



This function takes in a [**Vector4**](struct_a_g_e_1_1_vector4.md) object and returns its equivalent glm::vec4 representation. The conversion is done by simply copying the x, y, z, and w values from the input [**Vector4**](struct_a_g_e_1_1_vector4.md) into the corresponding components of the output glm::vec4.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to be converted. 



**Returns:**

A glm::vec4 with the same x, y, z, and w values as the input [**Vector4**](struct_a_g_e_1_1_vector4.md).


Converts a [**Vector4**](struct_a_g_e_1_1_vector4.md) to a GLM vec4.


This function takes in a [**Vector4**](struct_a_g_e_1_1_vector4.md) and returns a glm::vec4 with the same x, y, z, w values. The conversion is done by directly copying the values from the input [**Vector4**](struct_a_g_e_1_1_vector4.md) to the output glm::vec4.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to be converted.



**Returns:**

A GLM vector with the same x, y, z, w values as the input [**Vector4**](struct_a_g_e_1_1_vector4.md). 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/UtilityFunctions.h`

