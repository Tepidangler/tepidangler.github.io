

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
|   | [**BoxCollider2DComponent**](#function-boxcollider2dcomponent-12) () = default<br>_Default constructor for the_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _class._ |
|   | [**BoxCollider2DComponent**](#function-boxcollider2dcomponent-22) (const [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) &) = default<br>_Default copy constructor for the_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _class. This function is used to create a new instance of the class by copying an existing one, which can be useful in certain situations like initializing an object with values from another._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) & Data) <br>_This function deserializes a_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) & Data) <br>_This function serializes the data of a_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























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

_Default constructor for the_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _class._
```C++
AGE::BoxCollider2DComponent::BoxCollider2DComponent () = default
```



This function initializes a new instance of the [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) class with default values. 


        

<hr>



### function BoxCollider2DComponent [2/2]

_Default copy constructor for the_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _class. This function is used to create a new instance of the class by copying an existing one, which can be useful in certain situations like initializing an object with values from another._
```C++
AGE::BoxCollider2DComponent::BoxCollider2DComponent (
    const BoxCollider2DComponent &
) = default
```





**Parameters:**


* `other` The existing instance of the class that will be copied. 




        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes a_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
static inline void AGE::BoxCollider2DComponent::Deserialize (
    DataReader * Serializer,
    BoxCollider2DComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that contains the serialized data. 
* `Data` The [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) to be populated with the deserialized data.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes the data of a_ [_**BoxCollider2DComponent**_](struct_a_g_e_1_1_box_collider2_d_component.md) _into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::BoxCollider2DComponent::Serialize (
    DataWriter * Serializer,
    const BoxCollider2DComponent & Data
) 
```





**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the data will be written. 
* `Data` The [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md) whose data is being serialized.



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

