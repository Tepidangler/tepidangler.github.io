

# Struct AGE::TransformComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TransformComponent**](struct_a_g_e_1_1_transform_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Rotation**](#variable-rotation)   = `{ 0.f }`<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Scale**](#variable-scale)   = `{ 1.f }`<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Translation**](#variable-translation)   = `{ 0.f }`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetTransform**](#function-gettransform) () <br> |
|   | [**TransformComponent**](#function-transformcomponent-13) () = default<br> |
|   | [**TransformComponent**](#function-transformcomponent-23) (const [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) &) = default<br> |
|   | [**TransformComponent**](#function-transformcomponent-33) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & T) <br> |
|   | [**operator Matrix4D**](#function-operator-matrix4d) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) & Data) <br> |


























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
## Public Functions Documentation




### function GetTransform 

```C++
inline Matrix4D AGE::TransformComponent::GetTransform () 
```




<hr>



### function TransformComponent [1/3]

```C++
AGE::TransformComponent::TransformComponent () = default
```




<hr>



### function TransformComponent [2/3]

```C++
AGE::TransformComponent::TransformComponent (
    const TransformComponent &
) = default
```




<hr>



### function TransformComponent [3/3]

```C++
inline AGE::TransformComponent::TransformComponent (
    const Vector3 & T
) 
```




<hr>



### function operator Matrix4D 

```C++
inline AGE::TransformComponent::operator Matrix4D () 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::TransformComponent::Deserialize (
    DataReader * Serializer,
    TransformComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::TransformComponent::Serialize (
    DataWriter * Serializer,
    const TransformComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

