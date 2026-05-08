

# Struct AGE::CapsuleCollider2DComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**Density**](#variable-density)   = `1.f`<br> |
|  float | [**Friction**](#variable-friction)   = `1.f`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Offset**](#variable-offset)   = `{ 0.f, 0.f }`<br> |
|  float | [**Radius**](#variable-radius)   = `.5f`<br> |
|  float | [**Restitution**](#variable-restitution)   = `0.f`<br> |
|  float | [**RestitutionThreshold**](#variable-restitutionthreshold)   = `.5f`<br> |
|  b2ShapeId | [**ShapeID**](#variable-shapeid)   = `b2\_nullShapeId`<br> |
|  bool | [**bGeneratePhysicsEvents**](#variable-bgeneratephysicsevents)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**CapsuleCollider2DComponent**](#function-capsulecollider2dcomponent-12) () = default<br> |
|   | [**CapsuleCollider2DComponent**](#function-capsulecollider2dcomponent-22) (const [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md) &) = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable Density 

```C++
float AGE::CapsuleCollider2DComponent::Density;
```




<hr>



### variable Friction 

```C++
float AGE::CapsuleCollider2DComponent::Friction;
```




<hr>



### variable Offset 

```C++
Vector2 AGE::CapsuleCollider2DComponent::Offset;
```




<hr>



### variable Radius 

```C++
float AGE::CapsuleCollider2DComponent::Radius;
```




<hr>



### variable Restitution 

```C++
float AGE::CapsuleCollider2DComponent::Restitution;
```




<hr>



### variable RestitutionThreshold 

```C++
float AGE::CapsuleCollider2DComponent::RestitutionThreshold;
```




<hr>



### variable ShapeID 

```C++
b2ShapeId AGE::CapsuleCollider2DComponent::ShapeID;
```




<hr>



### variable bGeneratePhysicsEvents 

```C++
bool AGE::CapsuleCollider2DComponent::bGeneratePhysicsEvents;
```




<hr>
## Public Functions Documentation




### function CapsuleCollider2DComponent [1/2]

```C++
AGE::CapsuleCollider2DComponent::CapsuleCollider2DComponent () = default
```




<hr>



### function CapsuleCollider2DComponent [2/2]

```C++
AGE::CapsuleCollider2DComponent::CapsuleCollider2DComponent (
    const CapsuleCollider2DComponent &
) = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::CapsuleCollider2DComponent::Deserialize (
    DataReader * Serializer,
    CapsuleCollider2DComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::CapsuleCollider2DComponent::Serialize (
    DataWriter * Serializer,
    const CapsuleCollider2DComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

