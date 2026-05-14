

# Class AGE::Entity



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Entity**](class_a_g_e_1_1_entity.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br>_Adds a component of type T to the entity._  |
|  T & | [**AddOrReplaceComponent**](#function-addorreplacecomponent) (Args &&... args) <br>_Adds or replaces a component of type T in the scene._  |
|   | [**Entity**](#function-entity-13) () = default<br>_Default constructor for the_ [_**Entity**_](class_a_g_e_1_1_entity.md) _class._ |
|   | [**Entity**](#function-entity-23) (entt::entity Handle, [**Scene**](class_a_g_e_1_1_scene.md) \* ScenePtr) <br>_Constructs an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _object with the given handle and scene pointer._ |
|   | [**Entity**](#function-entity-33) (const [**Entity**](class_a_g_e_1_1_entity.md) & other) = default<br>_Copy constructor for the_ [_**Entity**_](class_a_g_e_1_1_entity.md) _class._ |
|  T & | [**GetComponent**](#function-getcomponent-12) () <br>_Get the Component object of type T associated with this_ [_**Entity**_](class_a_g_e_1_1_entity.md) _._ |
|  T & | [**GetComponent**](#function-getcomponent-22) () const<br>_Get the Component object of type T associated with this entity._  |
|  const std::string & | [**GetName**](#function-getname) () <br>_This function returns the name of a component associated with this object._  |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetUUID**](#function-getuuid) () <br>_This function returns the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _of an object._ |
|  bool | [**HasComponent**](#function-hascomponent-12) () <br>_Checks if the entity has a specific component in its registry._  |
|  bool | [**HasComponent**](#function-hascomponent-22) () const<br>_Checks if the entity has a specific component._  |
|  void | [**RemoveComponent**](#function-removecomponent) () <br>_Removes a component of type T from the entity associated with this handle in the scene's registry._  |
|   | [**operator bool**](#function-operator-bool) () const<br>_Checks whether the entity handle is not null._  |
|   | [**entity**](#function-entity) () const<br>_Converts the entity handle to an_ `entt` _entity._ |
|   | [**operator uint32\_t**](#function-operator-uint32_t) () const<br>_Converts the entity handle to a uint32\_t value._  |
|  bool | [**operator!=**](#function-operator) (const [**Entity**](class_a_g_e_1_1_entity.md) & Other) const<br>_Compares two entities for inequality._  |
|  bool | [**operator==**](#function-operator_1) (const [**Entity**](class_a_g_e_1_1_entity.md) & Other) const<br>_Compares two entities for equality based on their entity handle and scene._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Entity**](class_a_g_e_1_1_entity.md) & Data) <br>_This function deserializes data from a source into an entity object._  |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Entity**](class_a_g_e_1_1_entity.md) & Data) <br>_This function serializes an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object. The data includes the ID, Tag,_[_**Camera**_](class_a_g_e_1_1_camera.md) _, Transform, Sprite, TileMap, Circle, NativeScript,_[_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _, RigidBody2D, BoxCollider2D, CapsuleCollider2D, and SegmentCollider2D of the_[_**Entity**_](class_a_g_e_1_1_entity.md) _. If an entity does not contain a certain component, it will skip writing that data to avoid errors._ |


























## Public Functions Documentation




### function AddComponent 

_Adds a component of type T to the entity._ 
```C++
template<typename T, typename ... Args>
inline T & AGE::Entity::AddComponent (
    Args &&... args
) 
```



This function adds a new component of type T to the entity represented by m\_EntityHandle. The arguments are forwarded to the emplace function, allowing for variadic template parameters.




**Template parameters:**


* `T` The type of the component to be added. 
* `Args` The types of the arguments to be passed to the emplace function. 



**Parameters:**


* `args` The arguments to be passed to the emplace function.



**Returns:**

A reference to the newly created component.




**Precondition:**

The entity does not already have a component of type T. 




**Postcondition:**

The new component is added to the entity and an OnComponentAdded event is triggered for this scene.


Adds a component of type T to the entity.


This function adds a new component of type T to the entity represented by m\_EntityHandle. The arguments are forwarded to the emplace function, allowing for variadic template parameters. If the entity already has a component of this type, an assertion will fail.




**Template parameters:**


* `T` Type of the component to be added. 
* `Args` Variadic template parameter representing the types and/or values of arguments that are forwarded to emplace function. 



**Parameters:**


* `args` Arguments to be forwarded to emplace function. 



**Returns:**

Reference to the newly created component. 





        

<hr>



### function AddOrReplaceComponent 

_Adds or replaces a component of type T in the scene._ 
```C++
template<typename T, typename... Args>
inline T & AGE::Entity::AddOrReplaceComponent (
    Args &&... args
) 
```



This function emplaces an instance of type T into the registry associated with the entity represented by m\_EntityHandle, using variadic template arguments for constructor parameters. If a component of type T already exists for this entity, it will be replaced; otherwise, a new one is created. After adding or replacing the component, OnComponentAdded function from the scene class is called to notify any listeners about the change in component state.




**Template parameters:**


* `T` The type of the component to add or replace. 
* `Args` The types of arguments for constructing a new instance of T. 



**Parameters:**


* `args` Variadic template parameters forwarded to emplace\_or\_replace function. 



**Returns:**

A reference to the added/replaced component.


Adds or replaces a component of type T in the scene.


This function emplaces or replaces a component of type T with given arguments into the entity represented by m\_EntityHandle. It then calls OnComponentAdded for this component type and returns a reference to it. 

**Template parameters:**


* `T` The type of the component to be added or replaced. 
* `Args` The types of the arguments to be forwarded to emplace\_or\_replace function. 



**Parameters:**


* `args` The arguments to be forwarded to emplace\_or\_replace function. 



**Returns:**

A reference to the newly added or replaced component. 





        

<hr>



### function Entity [1/3]

_Default constructor for the_ [_**Entity**_](class_a_g_e_1_1_entity.md) _class._
```C++
AGE::Entity::Entity () = default
```



Default constructor for the [**Entity**](class_a_g_e_1_1_entity.md) class. 


        

<hr>



### function Entity [2/3]

_Constructs an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _object with the given handle and scene pointer._
```C++
AGE::Entity::Entity (
    entt::entity Handle,
    Scene * ScenePtr
) 
```





**Parameters:**


* `Handle` The entity handle to be associated with this [**Entity**](class_a_g_e_1_1_entity.md). 
* `ScenePtr` Pointer to the [**Scene**](class_a_g_e_1_1_scene.md) that this [**Entity**](class_a_g_e_1_1_entity.md) belongs to.

Constructs an [**Entity**](class_a_g_e_1_1_entity.md) object with the given handle and scene pointer.


This constructor initializes a new [**Entity**](class_a_g_e_1_1_entity.md) instance with the provided entt::entity handle and Scene\* pointer. The entity handle is used to identify this entity within its parent scene, while the Scene\* pointer allows access to the rest of the scene's data. 

**Parameters:**


* `Handle` The unique identifier for this entity. 
* `ScenePtr` A pointer to the scene that contains this entity. 




        

<hr>



### function Entity [3/3]

_Copy constructor for the_ [_**Entity**_](class_a_g_e_1_1_entity.md) _class._
```C++
AGE::Entity::Entity (
    const Entity & other
) = default
```



This function creates a new instance of an [**Entity**](class_a_g_e_1_1_entity.md) by copying all data from another existing [**Entity**](class_a_g_e_1_1_entity.md) object. It uses the '= default' syntax to delegate the copy construction task to the compiler, which is efficient and safe.




**Parameters:**


* `other` The [**Entity**](class_a_g_e_1_1_entity.md) object to be copied.

Copy constructor for the [**Entity**](class_a_g_e_1_1_entity.md) class.


This function creates a new instance of an [**Entity**](class_a_g_e_1_1_entity.md) by copying all data from another existing [**Entity**](class_a_g_e_1_1_entity.md) object. It uses the 'default' keyword to allow the compiler to generate its own copy constructor if one is not provided.




**Parameters:**


* `other` The [**Entity**](class_a_g_e_1_1_entity.md) object to be copied. 




        

<hr>



### function GetComponent [1/2]

_Get the Component object of type T associated with this_ [_**Entity**_](class_a_g_e_1_1_entity.md) _._
```C++
template<typename T>
inline T & AGE::Entity::GetComponent () 
```



This function retrieves a component of type T from the entity. If the entity does not have such a component, an assertion will fail and the program will terminate. The returned reference can be used to modify or access the component's data.




**Returns:**

T& Reference to the Component object of type T associated with this [**Entity**](class_a_g_e_1_1_entity.md).


Get the Component object of type T associated with this [**Entity**](class_a_g_e_1_1_entity.md).


This function retrieves a component of type T from the entity. It first checks if the entity has such a component, and throws an exception if it doesn't. The retrieved component is then returned by reference.




**Returns:**

T& Reference to the Component object. 





        

<hr>



### function GetComponent [2/2]

_Get the Component object of type T associated with this entity._ 
```C++
template<typename T>
inline T & AGE::Entity::GetComponent () const
```



This function retrieves a component of type T from the entity. If the entity does not have such a component, an assertion will be triggered and the program will terminate.




**Returns:**

const reference to the component of type T


Get the Component object of type T associated with this entity.


This function retrieves a component of type T from the entity. If the entity does not have such a component, an assertion will fail and the program will terminate.




**Returns:**

T& Reference to the component of type T. 





        

<hr>



### function GetName 

_This function returns the name of a component associated with this object._ 
```C++
inline const std::string & AGE::Entity::GetName () 
```





**Returns:**

A constant reference to the tag string of the [**TagComponent**](struct_a_g_e_1_1_tag_component.md) attached to this object. If no such component exists, an empty string is returned.


Returns the name of the component associated with this object. 

**Returns:**

A constant reference to a string representing the name of the component. 





        

<hr>



### function GetUUID 

_This function returns the_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _of an object._
```C++
inline UUID AGE::Entity::GetUUID () 
```



The function uses a component-based system where each object has components associated with it. It retrieves the [**IDComponent**](struct_a_g_e_1_1_i_d_component.md) from the object and then returns its [**UUID**](class_a_g_e_1_1_u_u_i_d.md).




**Returns:**

A [**UUID**](class_a_g_e_1_1_u_u_i_d.md) value representing the unique identifier of the object.


This function returns the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the object. 

**Returns:**

The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the object as a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) type. 





        

<hr>



### function HasComponent [1/2]

_Checks if the entity has a specific component in its registry._ 
```C++
template<typename T>
inline bool AGE::Entity::HasComponent () 
```



This function uses the any\_of method from entt's registry to check if an entity has a certain type of component. It returns true if the entity has at least one instance of the specified component, and false otherwise.




**Returns:**

True if the entity has the component, False otherwise.


Checks if the entity has a specific component of type T.


This function uses the any\_of method from entt's registry to check if an entity has a certain component of type T. It returns true if the entity has at least one instance of the specified component, and false otherwise.




**Returns:**

True if the entity has the component, False otherwise. 





        

<hr>



### function HasComponent [2/2]

_Checks if the entity has a specific component._ 
```C++
template<typename T>
inline bool AGE::Entity::HasComponent () const
```



This function checks whether an entity in the scene possesses a certain type of component. It does this by using the any\_of method from the entt library, which returns true if at least one instance of the given component is associated with the entity.




**Returns:**

A boolean value indicating whether or not the entity has the specified component. True means it possesses the component, while false signifies its absence.


Checks if the entity has a specific component.


This function checks whether an entity in the scene possesses a certain type of component. It does this by using the `any_of` method from the registry associated with the scene, specifically checking for the presence of the specified template parameter 'T' within the components attached to the entity represented by m\_EntityHandle.




**Returns:**

A boolean value indicating whether or not the entity has the component. True if it does, false otherwise. 





        

<hr>



### function RemoveComponent 

_Removes a component of type T from the entity associated with this handle in the scene's registry._ 
```C++
template<typename T>
inline void AGE::Entity::RemoveComponent () 
```



This function removes a component of type T from the entity represented by m\_EntityHandle within the scene's ECS (entity-component-system) registry. The removal is performed using the remove() method provided by the entt library, which expects an instance of the [**Entity**](class_a_g_e_1_1_entity.md) class and a type to be removed.




**Returns:**

void


Removes a component of type T from the entity associated with this handle in the scene's registry.


This function removes a specific instance of a component of type T from the entity represented by m\_EntityHandle within the scene's ECS (entity-component system). The removal is performed using the remove function provided by the entt library, which ensures that the component is properly removed and no memory leaks occur.




**Returns:**

void 





        

<hr>



### function operator bool 

_Checks whether the entity handle is not null._ 
```C++
inline AGE::Entity::operator bool () const
```



This function returns true if the entity handle is not equal to `entt::null`, indicating that an entity exists in the system.




**Returns:**

True if the entity handle is not null (i.e., an entity exists), false otherwise.


Checks whether the entity handle is valid (i.e., not null).


This function checks if the `m_EntityHandle` member variable of the current object is different from `entt::null`, which represents an invalid or non-existent entity in some context. The function returns true if the handle is valid and false otherwise.




**Returns:**

True if the entity handle is not null; false otherwise. 





        

<hr>



### function entity 

_Converts the entity handle to an_ `entt` _entity._
```C++
inline AGE::Entity::entity () const
```



This function returns the underlying `entt::entity` object that this EntityHandle wraps around. It is used internally by various parts of the codebase and should not be called directly by user code.




**Returns:**

The wrapped `entt::entity` object.


Converts the entity handle to an entt::entity object.


This function returns the underlying `entt::entity` object that this EntityWrapper is wrapping. It provides a direct access to the actual entity, allowing for operations and manipulations on it.




**Returns:**

The wrapped `entt::entity` object. 





        

<hr>



### function operator uint32\_t 

_Converts the entity handle to a uint32\_t value._ 
```C++
inline AGE::Entity::operator uint32_t () const
```



This function returns the underlying uint32\_t representation of the entity handle. It is used for interoperability with other systems that expect uint32\_t values, such as rendering engines or physics engines.




**Returns:**

The uint32\_t representation of the entity handle.


Converts the entity handle to a uint32\_t value.


This function returns the `m_EntityHandle` member variable as a `uint32_t` value. It is used for casting or conversion purposes, allowing it to be treated like an unsigned 32-bit integer.




**Returns:**

The `m_EntityHandle` member variable casted to a uint32\_t. 





        

<hr>



### function operator!= 

_Compares two entities for inequality._ 
```C++
inline bool AGE::Entity::operator!= (
    const Entity & Other
) const
```



This function compares the current entity with another one to determine if they are not equal. It uses the '==' operator to compare the entities and returns the opposite result.




**Parameters:**


* `Other` The other [**Entity**](class_a_g_e_1_1_entity.md) object to be compared with this one. 



**Returns:**

True if the two entities are not equal, false otherwise.


Compares two entities for inequality.


This function compares the current entity with another one to determine if they are not equal. It uses the equality operator (`operator==`) to perform the comparison and returns the opposite result.




**Parameters:**


* `Other` The other entity to compare with. 



**Returns:**

True if the entities are not equal, false otherwise. 





        

<hr>



### function operator== 

_Compares two entities for equality based on their entity handle and scene._ 
```C++
inline bool AGE::Entity::operator== (
    const Entity & Other
) const
```





**Parameters:**


* `Other` The [**Entity**](class_a_g_e_1_1_entity.md) to compare with this one. 



**Returns:**

True if the other entity has the same entity handle and scene as this one, false otherwise.


Compares two entities for equality based on their entity handle and scene. 

**Parameters:**


* `Other` The [**Entity**](class_a_g_e_1_1_entity.md) to compare with this one. 



**Returns:**

True if the other entity has the same entity handle and scene as this one, false otherwise. 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes data from a source into an entity object._ 
```C++
static inline void AGE::Entity::Deserialize (
    DataReader * Deserializer,
    Entity & Data
) 
```



The function takes in a pointer to a `DataReader` and a reference to an `Entity` object. It does not return anything, but it modifies the `Entity` object by reading its state from the `DataReader`.




**Parameters:**


* `Deserializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` The [**Entity**](class_a_g_e_1_1_entity.md) object which will be populated with deserialized data.

This function deserializes data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) into an [**Entity**](class_a_g_e_1_1_entity.md) object.


The function reads the necessary information from the [**DataReader**](class_a_g_e_1_1_data_reader.md) and populates the [**Entity**](class_a_g_e_1_1_entity.md) object with it. It does not return anything as it directly modifies the passed [**Entity**](class_a_g_e_1_1_entity.md) object.




**Parameters:**


* `Deserializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains the serialized data. 
* `Data` The [**Entity**](class_a_g_e_1_1_entity.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_This function serializes an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object. The data includes the ID, Tag,_[_**Camera**_](class_a_g_e_1_1_camera.md) _, Transform, Sprite, TileMap, Circle, NativeScript,_[_**AudioComponent**_](struct_a_g_e_1_1_audio_component.md) _, RigidBody2D, BoxCollider2D, CapsuleCollider2D, and SegmentCollider2D of the_[_**Entity**_](class_a_g_e_1_1_entity.md) _. If an entity does not contain a certain component, it will skip writing that data to avoid errors._
```C++
static inline void AGE::Entity::Serialize (
    DataWriter * Serializer,
    const Entity & Data
) 
```





**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the serialized data will be written. 
* `Data` The [**Entity**](class_a_g_e_1_1_entity.md) object to be serialized.

This function is responsible for writing entity data into a serialization format. It checks if the entity has certain components and writes their data if they exist.




**Parameters:**


* `Serializer` Pointer to an object that can write raw data types. 
* `Data` Const reference to an [**Entity**](class_a_g_e_1_1_entity.md) object which contains various components. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Entity.h`

