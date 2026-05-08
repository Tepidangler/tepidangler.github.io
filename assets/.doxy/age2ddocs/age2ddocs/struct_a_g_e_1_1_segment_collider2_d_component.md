

# Struct AGE::SegmentCollider2DComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md)


























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
|   | [**SegmentCollider2DComponent**](#function-segmentcollider2dcomponent-12) () = default<br> |
|   | [**SegmentCollider2DComponent**](#function-segmentcollider2dcomponent-22) (const [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md) &) = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable Density 

```C++
float AGE::SegmentCollider2DComponent::Density;
```




<hr>



### variable Friction 

```C++
float AGE::SegmentCollider2DComponent::Friction;
```




<hr>



### variable Offset 

```C++
Vector2 AGE::SegmentCollider2DComponent::Offset;
```




<hr>



### variable Restitution 

```C++
float AGE::SegmentCollider2DComponent::Restitution;
```




<hr>



### variable RestitutionThreshold 

```C++
float AGE::SegmentCollider2DComponent::RestitutionThreshold;
```




<hr>



### variable ShapeID 

```C++
b2ShapeId AGE::SegmentCollider2DComponent::ShapeID;
```




<hr>



### variable Size 

```C++
Vector2 AGE::SegmentCollider2DComponent::Size;
```




<hr>



### variable bGeneratePhysicsEvents 

```C++
bool AGE::SegmentCollider2DComponent::bGeneratePhysicsEvents;
```




<hr>
## Public Functions Documentation




### function SegmentCollider2DComponent [1/2]

```C++
AGE::SegmentCollider2DComponent::SegmentCollider2DComponent () = default
```




<hr>



### function SegmentCollider2DComponent [2/2]

```C++
AGE::SegmentCollider2DComponent::SegmentCollider2DComponent (
    const SegmentCollider2DComponent &
) = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::SegmentCollider2DComponent::Deserialize (
    DataReader * Serializer,
    SegmentCollider2DComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::SegmentCollider2DComponent::Serialize (
    DataWriter * Serializer,
    const SegmentCollider2DComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

