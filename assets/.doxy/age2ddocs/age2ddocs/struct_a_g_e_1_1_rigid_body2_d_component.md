

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
|  BodyType | [**GetBodyType**](#function-getbodytype) () <br>_This function returns the body type of an object._  |
|   | [**RigidBody2DComponent**](#function-rigidbody2dcomponent-12) () = default<br>_Default constructor for the_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _class. This function initializes a new instance of the_[_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _with default values. The component is assumed to have no mass, an inertia tensor of zero, and a center of mass at the origin._ |
|   | [**RigidBody2DComponent**](#function-rigidbody2dcomponent-22) (const [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) &) = default<br>_Default copy constructor for the_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _class._ |
|  void | [**SetBodyType**](#function-setbodytype) (BodyType type) <br>_Sets the body type of an object._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) & Data) <br>_This function deserializes the data from a serialized format into an instance of_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) & Data) <br>_This function serializes the data of a_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _._ |


























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

_This function returns the body type of an object._ 
```C++
inline BodyType AGE::RigidBody2DComponent::GetBodyType () 
```





**Returns:**

BodyType The type of the body (e.g., human, animal). 





        

<hr>



### function RigidBody2DComponent [1/2]

_Default constructor for the_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _class. This function initializes a new instance of the_[_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _with default values. The component is assumed to have no mass, an inertia tensor of zero, and a center of mass at the origin._
```C++
AGE::RigidBody2DComponent::RigidBody2DComponent () = default
```





**Returns:**

A new instance of [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) with default properties. 





        

<hr>



### function RigidBody2DComponent [2/2]

_Default copy constructor for the_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _class._
```C++
AGE::RigidBody2DComponent::RigidBody2DComponent (
    const RigidBody2DComponent &
) = default
```



This function is used to create a new instance of the [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) instance to be copied. 




        

<hr>



### function SetBodyType 

_Sets the body type of an object._ 
```C++
inline void AGE::RigidBody2DComponent::SetBodyType (
    BodyType type
) 
```





**Parameters:**


* `type` The new BodyType to set for the object. 




        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes the data from a serialized format into an instance of_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _._
```C++
static inline void AGE::RigidBody2DComponent::Deserialize (
    DataReader * Serializer,
    RigidBody2DComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains the serialized data. 
* `Data` The [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) instance where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes the data of a_ [_**RigidBody2DComponent**_](struct_a_g_e_1_1_rigid_body2_d_component.md) _._
```C++
static inline void AGE::RigidBody2DComponent::Serialize (
    DataWriter * Serializer,
    const RigidBody2DComponent & Data
) 
```



The function takes in two parameters - a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object and a constant reference to a [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) object. It does not return anything as it is a void function.




**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be used for serialization. 
* `Data` The [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md) whose data needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

