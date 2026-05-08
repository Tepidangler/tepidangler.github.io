

# Struct AGE::RigidBody2DComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  b2BodyId | [**BodyID**](#variable-bodyid)   = `b2\_nullBodyId`<br> |
|  bool | [**FixedRotation**](#variable-fixedrotation)   = `false`<br> |
|  void \* | [**RuntimeBody**](#variable-runtimebody)   = `nullptr`<br> |
|  BodyType | [**Type**](#variable-type)   = `BodyType::Static`<br> |
|  bool | [**bInteractable**](#variable-binteractable)   = `false`<br> |
|  bool | [**bSimulatePhysics**](#variable-bsimulatephysics)   = `true`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  BodyType | [**GetBodyType**](#function-getbodytype) () <br> |
|   | [**RigidBody2DComponent**](#function-rigidbody2dcomponent-12) () = default<br> |
|   | [**RigidBody2DComponent**](#function-rigidbody2dcomponent-22) (const [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) &) = default<br> |
|  void | [**SetBodyType**](#function-setbodytype) (BodyType type) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable BodyID 

```C++
b2BodyId AGE::RigidBody2DComponent::BodyID;
```




<hr>



### variable FixedRotation 

```C++
bool AGE::RigidBody2DComponent::FixedRotation;
```




<hr>



### variable RuntimeBody 

```C++
void* AGE::RigidBody2DComponent::RuntimeBody;
```




<hr>



### variable Type 

```C++
BodyType AGE::RigidBody2DComponent::Type;
```




<hr>



### variable bInteractable 

```C++
bool AGE::RigidBody2DComponent::bInteractable;
```




<hr>



### variable bSimulatePhysics 

```C++
bool AGE::RigidBody2DComponent::bSimulatePhysics;
```




<hr>
## Public Functions Documentation




### function GetBodyType 

```C++
inline BodyType AGE::RigidBody2DComponent::GetBodyType () 
```




<hr>



### function RigidBody2DComponent [1/2]

```C++
AGE::RigidBody2DComponent::RigidBody2DComponent () = default
```




<hr>



### function RigidBody2DComponent [2/2]

```C++
AGE::RigidBody2DComponent::RigidBody2DComponent (
    const RigidBody2DComponent &
) = default
```




<hr>



### function SetBodyType 

```C++
inline void AGE::RigidBody2DComponent::SetBodyType (
    BodyType type
) 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::RigidBody2DComponent::Deserialize (
    DataReader * Serializer,
    RigidBody2DComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::RigidBody2DComponent::Serialize (
    DataWriter * Serializer,
    const RigidBody2DComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

