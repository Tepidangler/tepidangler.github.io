

# Class AGE::Entity



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Entity**](class_a_g_e_1_1_entity.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br> |
|  T & | [**AddOrReplaceComponent**](#function-addorreplacecomponent) (Args &&... args) <br> |
|   | [**Entity**](#function-entity-13) () = default<br> |
|   | [**Entity**](#function-entity-23) (entt::entity Handle, [**Scene**](class_a_g_e_1_1_scene.md) \* ScenePtr) <br> |
|   | [**Entity**](#function-entity-33) (const [**Entity**](class_a_g_e_1_1_entity.md) & other) = default<br> |
|  T & | [**GetComponent**](#function-getcomponent-12) () <br> |
|  T & | [**GetComponent**](#function-getcomponent-22) () const<br> |
|  const std::string & | [**GetName**](#function-getname) () <br> |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetUUID**](#function-getuuid) () <br> |
|  bool | [**HasComponent**](#function-hascomponent-12) () <br> |
|  bool | [**HasComponent**](#function-hascomponent-22) () const<br> |
|  void | [**RemoveComponent**](#function-removecomponent) () <br> |
|   | [**operator bool**](#function-operator-bool) () const<br> |
|   | [**entity**](#function-entity) () const<br> |
|   | [**operator uint32\_t**](#function-operator-uint32_t) () const<br> |
|  bool | [**operator!=**](#function-operator) (const [**Entity**](class_a_g_e_1_1_entity.md) & Other) const<br> |
|  bool | [**operator==**](#function-operator_1) (const [**Entity**](class_a_g_e_1_1_entity.md) & Other) const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Entity**](class_a_g_e_1_1_entity.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Entity**](class_a_g_e_1_1_entity.md) & Data) <br> |


























## Public Functions Documentation




### function AddComponent 

```C++
template<typename T, typename ... Args>
inline T & AGE::Entity::AddComponent (
    Args &&... args
) 
```




<hr>



### function AddOrReplaceComponent 

```C++
template<typename T, typename... Args>
inline T & AGE::Entity::AddOrReplaceComponent (
    Args &&... args
) 
```




<hr>



### function Entity [1/3]

```C++
AGE::Entity::Entity () = default
```




<hr>



### function Entity [2/3]

```C++
AGE::Entity::Entity (
    entt::entity Handle,
    Scene * ScenePtr
) 
```




<hr>



### function Entity [3/3]

```C++
AGE::Entity::Entity (
    const Entity & other
) = default
```




<hr>



### function GetComponent [1/2]

```C++
template<typename T>
inline T & AGE::Entity::GetComponent () 
```




<hr>



### function GetComponent [2/2]

```C++
template<typename T>
inline T & AGE::Entity::GetComponent () const
```




<hr>



### function GetName 

```C++
inline const std::string & AGE::Entity::GetName () 
```




<hr>



### function GetUUID 

```C++
inline UUID AGE::Entity::GetUUID () 
```




<hr>



### function HasComponent [1/2]

```C++
template<typename T>
inline bool AGE::Entity::HasComponent () 
```




<hr>



### function HasComponent [2/2]

```C++
template<typename T>
inline bool AGE::Entity::HasComponent () const
```




<hr>



### function RemoveComponent 

```C++
template<typename T>
inline void AGE::Entity::RemoveComponent () 
```




<hr>



### function operator bool 

```C++
inline AGE::Entity::operator bool () const
```




<hr>



### function entity 

```C++
inline AGE::Entity::entity () const
```




<hr>



### function operator uint32\_t 

```C++
inline AGE::Entity::operator uint32_t () const
```




<hr>



### function operator!= 

```C++
inline bool AGE::Entity::operator!= (
    const Entity & Other
) const
```




<hr>



### function operator== 

```C++
inline bool AGE::Entity::operator== (
    const Entity & Other
) const
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::Entity::Deserialize (
    DataReader * Deserializer,
    Entity & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::Entity::Serialize (
    DataWriter * Serializer,
    const Entity & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Entity.h`

