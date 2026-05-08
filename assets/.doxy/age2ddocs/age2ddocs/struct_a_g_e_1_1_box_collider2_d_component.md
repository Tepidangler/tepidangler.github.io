

# Struct AGE::BoxCollider2DComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**Density**](#variable-density)   = `1.f`<br> |
|  float | [**Friction**](#variable-friction)   = `1.f`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Offset**](#variable-offset)   = `{ 0.f, 0.f }`<br> |
|  float | [**Restitution**](#variable-restitution)   = `0.f`<br> |
|  float | [**RestitutionThreshold**](#variable-restitutionthreshold)   = `.5f`<br> |
|  b2ShapeId | [**ShapeID**](#variable-shapeid)   = `b2\_nullShapeId`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Size**](#variable-size)   = `{ .5f,.5f }`<br> |
|  bool | [**bGeneratePhysicsEvents**](#variable-bgeneratephysicsevents)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BoxCollider2DComponent**](#function-boxcollider2dcomponent-12) () = default<br> |
|   | [**BoxCollider2DComponent**](#function-boxcollider2dcomponent-22) (const [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) &) = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable Density 

```C++
float AGE::BoxCollider2DComponent::Density;
```




<hr>



### variable Friction 

```C++
float AGE::BoxCollider2DComponent::Friction;
```




<hr>



### variable Offset 

```C++
Vector2 AGE::BoxCollider2DComponent::Offset;
```




<hr>



### variable Restitution 

```C++
float AGE::BoxCollider2DComponent::Restitution;
```




<hr>



### variable RestitutionThreshold 

```C++
float AGE::BoxCollider2DComponent::RestitutionThreshold;
```




<hr>



### variable ShapeID 

```C++
b2ShapeId AGE::BoxCollider2DComponent::ShapeID;
```




<hr>



### variable Size 

```C++
Vector2 AGE::BoxCollider2DComponent::Size;
```




<hr>



### variable bGeneratePhysicsEvents 

```C++
bool AGE::BoxCollider2DComponent::bGeneratePhysicsEvents;
```




<hr>
## Public Functions Documentation




### function BoxCollider2DComponent [1/2]

```C++
AGE::BoxCollider2DComponent::BoxCollider2DComponent () = default
```




<hr>



### function BoxCollider2DComponent [2/2]

```C++
AGE::BoxCollider2DComponent::BoxCollider2DComponent (
    const BoxCollider2DComponent &
) = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::BoxCollider2DComponent::Deserialize (
    DataReader * Serializer,
    BoxCollider2DComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::BoxCollider2DComponent::Serialize (
    DataWriter * Serializer,
    const BoxCollider2DComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

