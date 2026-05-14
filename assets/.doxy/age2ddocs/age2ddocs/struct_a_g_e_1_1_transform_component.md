

# Struct AGE::TransformComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TransformComponent**](struct_a_g_e_1_1_transform_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Rotation**](#variable-rotation)   = `{ 0.f }`<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Scale**](#variable-scale)   = `{ 1.f }`<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Translation**](#variable-translation)   = `{ 0.f }`<br> |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetTransform**](#function-gettransform) () <br>_This function returns the transformation matrix for this object. The transformation is composed of a translation, rotation and scale. It uses GLM (OpenGL Mathematics) library to perform these transformations._  |
|   | [**TransformComponent**](#function-transformcomponent-13) () = default<br>_Default constructor for the_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _class._ |
|   | [**TransformComponent**](#function-transformcomponent-23) (const [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) &) = default<br>_Default copy constructor for the_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _class._ |
|   | [**TransformComponent**](#function-transformcomponent-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & T) <br> |
|   | [**operator Matrix4D**](#function-operator-matrix4d) () <br>_Converts the current object to a 4x4 matrix representation._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) & Data) <br>_This function deserializes data from a serialized format into the given_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) & Data) <br>_This function serializes the given transform component data into a format that can be stored or transmitted._  |


























## Public Attributes Documentation




### variable Rotation 

```C++
Vector3 AGE::TransformComponent::Rotation;
```




<hr>



### variable Scale 

```C++
Vector3 AGE::TransformComponent::Scale;
```




<hr>



### variable Translation 

```C++
Vector3 AGE::TransformComponent::Translation;
```




<hr>



### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::TransformComponent::__pad0__;
```




<hr>
## Public Functions Documentation




### function GetTransform 

_This function returns the transformation matrix for this object. The transformation is composed of a translation, rotation and scale. It uses GLM (OpenGL Mathematics) library to perform these transformations._ 
```C++
inline Matrix4D AGE::TransformComponent::GetTransform () 
```





**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) - Returns the combined transformation matrix. 





        

<hr>



### function TransformComponent [1/3]

_Default constructor for the_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _class._
```C++
AGE::TransformComponent::TransformComponent () = default
```




<hr>



### function TransformComponent [2/3]

_Default copy constructor for the_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _class._
```C++
AGE::TransformComponent::TransformComponent (
    const TransformComponent &
) = default
```



This function is used to create a new instance of the [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) instance to copy. 




        

<hr>



### function TransformComponent [3/3]

```C++
inline AGE::TransformComponent::TransformComponent (
    const Vector3 & T
) 
```




<hr>



### function operator Matrix4D 

_Converts the current object to a 4x4 matrix representation._ 
```C++
inline AGE::TransformComponent::operator Matrix4D () 
```



This function converts the current object into a 4x4 matrix representation by calling the `GetTransform` method and returning its result. The conversion is done implicitly when this object is used in a context that expects a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md), such as passing it to a function or operator that accepts a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) parameter.




**Returns:**

A 4x4 matrix representing the current object's transformation. 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes data from a serialized format into the given_ [_**TransformComponent**_](struct_a_g_e_1_1_transform_component.md) _object._
```C++
static inline void AGE::TransformComponent::Deserialize (
    DataReader * Serializer,
    TransformComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to an instance of [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` The [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_This function serializes the given transform component data into a format that can be stored or transmitted._ 
```C++
static inline void AGE::TransformComponent::Serialize (
    DataWriter * Serializer,
    const TransformComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) which is responsible for writing the serialized data. 
* `Data` The [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) whose data needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

