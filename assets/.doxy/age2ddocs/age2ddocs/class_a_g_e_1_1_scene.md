

# Class AGE::Scene



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Scene**](class_a_g_e_1_1_scene.md)








Inherits the following classes: std::enable_shared_from_this< Scene >


































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**BroadcastEvent**](#function-broadcastevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br>_This function broadcasts an event to the scene._  |
|  void | [**BuildScene**](#function-buildscene) (const std::filesystem::path & ProjectPath) <br>_Builds a scene and saves it in a file within the "BuiltScenes" directory._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**Copy**](#function-copy) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Other) <br> |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**CreateEntity**](#function-createentity) (const std::string Name="") <br>_Creates an entity with a given name and assigns it a_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._ |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**CreateEntityWithUUID**](#function-createentitywithuuid) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) uuid, const std::string & Name=std::string()) <br>_Creates an entity with a specific_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _and name._ |
|  void | [**DestoryEntity**](#function-destoryentity) ([**Entity**](class_a_g_e_1_1_entity.md) E) <br>_Destroys an entity from the scene's registry._  |
|  void | [**DuplicateEntity**](#function-duplicateentity) ([**Entity**](class_a_g_e_1_1_entity.md) entity) <br>_Duplicates an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _in the_[_**Scene**_](class_a_g_e_1_1_scene.md) _._ |
|  auto | [**GetAllEntitiesWith**](#function-getallentitieswith) () <br>_Returns a view of all entities that have the specified components in the registry._  |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br>_Gets the Asset ID of the object._  |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**GetEntityFromUUID**](#function-getentityfromuuid) (const uint64\_t uuid) <br>_Retrieves an entity from the scene using its_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._ |
|  std::string & | [**GetName**](#function-getname) () <br>_Returns the name of the object._  |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**GetPrimaryCameraEntity**](#function-getprimarycameraentity) () <br>_This function returns the primary camera entity in the scene._  |
|  void | [**OnEditorUpdate**](#function-oneditorupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime, [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br> |
|  void | [**OnRuntimeStart**](#function-onruntimestart) () <br> |
|  void | [**OnRuntimeStop**](#function-onruntimestop) () <br>_This function is called when the runtime of the application stops. It unloads sounds, destroys the physics world and resets all native script instances._  |
|  void | [**OnRuntimeUpdate**](#function-onruntimeupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**OnViewportResize**](#function-onviewportresize) (uint32\_t Width, uint32\_t Height) <br>_This function is called when the viewport size changes. It updates all camera components to reflect the new viewport dimensions._  |
|   | [**Scene**](#function-scene-14) () <br> |
|   | [**Scene**](#function-scene-24) (const [**Scene**](class_a_g_e_1_1_scene.md) & Other) = delete<br>_Copy constructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class is deleted to prevent copying of objects._ |
|   | [**Scene**](#function-scene-34) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Constructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._ |
|   | [**Scene**](#function-scene-44) (const std::string & Name) <br>_Constructs a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object with the given name and generates an unique asset ID._ |
|  void | [**SetEventCallback**](#function-seteventcallback) (const std::function&lt; void([**Event**](class_a_g_e_1_1_event.md) &)&gt; & Callback) <br>_This function sets the callback for handling events._  |
|  void | [**SetSceneName**](#function-setscenename) (const std::string & Name) <br>_Sets the name of the scene._  |
|  void | [**operator=**](#function-operator) (const [**Scene**](class_a_g_e_1_1_scene.md) & Other) <br>_Copy assignment operator for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._ |
|   | [**~Scene**](#function-scene) () <br>_Destructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BuildAllScenes**](#function-buildallscenes) () <br> |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Scene**](class_a_g_e_1_1_scene.md) & Data) <br>_Deserialize a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Path) <br>_Loads a scene from the specified file path._  |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Scene**](class_a_g_e_1_1_scene.md) & Data) <br>_This function serializes a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























## Public Functions Documentation




### function BroadcastEvent 

_This function broadcasts an event to the scene._ 
```C++
inline void AGE::Scene::BroadcastEvent (
    Event & Event
) 
```





**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event that is being broadcasted. 



**Returns:**

void No return value expected.


This function broadcasts an event to the scene.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event to be broadcasted. 



**Returns:**

void 





        

<hr>



### function BuildScene 

_Builds a scene and saves it in a file within the "BuiltScenes" directory._ 
```C++
void AGE::Scene::BuildScene (
    const std::filesystem::path & ProjectPath
) 
```



Checks if the "BuiltScenes" directory exists at the parent path of the project path. If not, creates this directory. Then writes the current scene object to a file with name equal to the scene's name and extension ".abs". Finally logs an info message indicating that the scene has been successfully built.




**Parameters:**


* `ProjectPath` The path of the project used to determine where to save the built scene files.

Builds the scene and saves it to a file in the "BuiltScenes" directory.


The function builds the current scene by writing its data into an abstract syntax tree (AST) format. The AST is saved as a file with the name of the scene, followed by ".abs". If the "BuiltScenes" directory does not exist, it will be created. 


        

<hr>



### function Copy 

```C++
Ref< Scene > AGE::Scene::Copy (
    Ref< Scene > Other
) 
```




<hr>



### function CreateEntity 

_Creates an entity with a given name and assigns it a_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._
```C++
Entity AGE::Scene::CreateEntity (
    const std::string Name=""
) 
```



This function creates an [**Entity**](class_a_g_e_1_1_entity.md) object with the provided name, generates a unique [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for it using the `UUID()` function, and then adds this new entity to the scene's list of entities. The newly created entity is returned by the function.




**Parameters:**


* `Name` A string representing the name of the entity to be created. 



**Returns:**

An [**Entity**](class_a_g_e_1_1_entity.md) object with a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) that has been assigned.


Creates an entity with a given name and assigns it a [**UUID**](class_a_g_e_1_1_u_u_i_d.md).


This function creates an [**Entity**](class_a_g_e_1_1_entity.md) object with the provided name, generates a unique [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for it using the `UUID()` function, and then adds this new entity to the scene's list of entities. The newly created entity is returned by the function.




**Parameters:**


* `Name` A string representing the name of the entity to be created.



**Returns:**

An [**Entity**](class_a_g_e_1_1_entity.md) object with a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) that has been assigned. 





        

<hr>



### function CreateEntityWithUUID 

_Creates an entity with a specific_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _and name._
```C++
Entity AGE::Scene::CreateEntityWithUUID (
    UUID uuid,
    const std::string & Name=std::string()
) 
```



This function creates an entity, assigns it a unique ID ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)), adds [**TransformComponent**](struct_a_g_e_1_1_transform_component.md) to the entity, and sets its tag to either the provided name or "UnnamedEntity" if no name is provided. The created entity is then returned. 

**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for the new entity. 
* `Name` The optional name of the new entity. If not provided, it will default to "UnnamedEntity". 



**Returns:**

[**Entity**](class_a_g_e_1_1_entity.md) The newly created entity.


Creates an entity with a specific [**UUID**](class_a_g_e_1_1_u_u_i_d.md) and name.


This function creates an [**Entity**](class_a_g_e_1_1_entity.md) object, adds [**IDComponent**](struct_a_g_e_1_1_i_d_component.md), [**TransformComponent**](struct_a_g_e_1_1_transform_component.md), and [**TagComponent**](struct_a_g_e_1_1_tag_component.md) to it, sets the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the [**IDComponent**](struct_a_g_e_1_1_i_d_component.md), initializes the tag of the [**TagComponent**](struct_a_g_e_1_1_tag_component.md) using the provided Name parameter (or "UnnamedEntity" if the Name is empty), and returns the created entity.




**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) for the new [**Entity**](class_a_g_e_1_1_entity.md). 
* `Name` The name for the new [**Entity**](class_a_g_e_1_1_entity.md). If this is an empty string, the tag of the [**TagComponent**](struct_a_g_e_1_1_tag_component.md) will be set to "UnnamedEntity".



**Returns:**

An [**Entity**](class_a_g_e_1_1_entity.md) object representing the newly created entity. 





        

<hr>



### function DestoryEntity 

_Destroys an entity from the scene's registry._ 
```C++
void AGE::Scene::DestoryEntity (
    Entity E
) 
```



This function removes an [**Entity**](class_a_g_e_1_1_entity.md) from the Registry of the [**Scene**](class_a_g_e_1_1_scene.md) object. It takes as input a reference to an [**Entity**](class_a_g_e_1_1_entity.md), and destroys it by removing it from the Registry.




**Parameters:**


* `E` A reference to the [**Entity**](class_a_g_e_1_1_entity.md) that is to be destroyed. 



**Returns:**

void


Destroys an entity from the scene's registry. 

**Parameters:**


* `E` The [**Entity**](class_a_g_e_1_1_entity.md) to be destroyed. 




        

<hr>



### function DuplicateEntity 

_Duplicates an_ [_**Entity**_](class_a_g_e_1_1_entity.md) _in the_[_**Scene**_](class_a_g_e_1_1_scene.md) _._
```C++
void AGE::Scene::DuplicateEntity (
    Entity entity
) 
```



This function duplicates a given [**Entity**](class_a_g_e_1_1_entity.md) by creating a new one with the same name and copying all its components from the original [**Entity**](class_a_g_e_1_1_entity.md) to the new one. The components copied are [**TransformComponent**](struct_a_g_e_1_1_transform_component.md), [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md), [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md), [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md), [**AudioComponent**](struct_a_g_e_1_1_audio_component.md), [**CameraComponent**](struct_a_g_e_1_1_camera_component.md), [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md), [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md), [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md), [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md) and [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md).




**Parameters:**


* `entity` The [**Entity**](class_a_g_e_1_1_entity.md) to be duplicated.

Duplicates an [**Entity**](class_a_g_e_1_1_entity.md) in the [**Scene**](class_a_g_e_1_1_scene.md).


This function duplicates an existing [**Entity**](class_a_g_e_1_1_entity.md) by creating a new one with the same name and copying all its components from the original [**Entity**](class_a_g_e_1_1_entity.md). The copied components include [**TransformComponent**](struct_a_g_e_1_1_transform_component.md), [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md), [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md), [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md), [**AudioComponent**](struct_a_g_e_1_1_audio_component.md), [**CameraComponent**](struct_a_g_e_1_1_camera_component.md), [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md), [**RigidBody2DComponent**](struct_a_g_e_1_1_rigid_body2_d_component.md), [**BoxCollider2DComponent**](struct_a_g_e_1_1_box_collider2_d_component.md), [**SegmentCollider2DComponent**](struct_a_g_e_1_1_segment_collider2_d_component.md) and [**CapsuleCollider2DComponent**](struct_a_g_e_1_1_capsule_collider2_d_component.md).




**Parameters:**


* `entity` The [**Entity**](class_a_g_e_1_1_entity.md) to be duplicated. 




        

<hr>



### function GetAllEntitiesWith 

_Returns a view of all entities that have the specified components in the registry._ 
```C++
template<typename... Components>
inline auto AGE::Scene::GetAllEntitiesWith () 
```



The function returns a view containing all entities that possess the types `Components...` as their component types. This can be useful for iterating over these entities and performing operations on them.




**Returns:**

A range of entity handles representing all entities with the specified components.


This function returns a view of all entities in the registry that have the specified components.




**Template parameters:**


* `Components` The types of components to check for. 



**Returns:**

auto A range-based for loop can be used to iterate over the returned view, which contains all entities with the specified components. 





        

<hr>



### function GetAssetID 

_Gets the Asset ID of the object._ 
```C++
inline UUID & AGE::Scene::GetAssetID () 
```



This function returns a reference to the private member variable 'm\_AssetID'. It provides access to this data, but does not allow modification.




**Returns:**

A reference to [**UUID**](class_a_g_e_1_1_u_u_i_d.md)& representing the Asset ID.


Gets the Asset ID of the object.


This function returns a reference to the private member variable 'm\_AssetID'. It provides access to this data, but does not allow modification.




**Returns:**

A reference to [**UUID**](class_a_g_e_1_1_u_u_i_d.md)& representing the Asset ID. 





        

<hr>



### function GetEntityFromUUID 

_Retrieves an entity from the scene using its_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._
```C++
Entity AGE::Scene::GetEntityFromUUID (
    const uint64_t uuid
) 
```



This function iterates over all entities in the registry and checks if their [**IDComponent**](struct_a_g_e_1_1_i_d_component.md) has a matching [**UUID**](class_a_g_e_1_1_u_u_i_d.md). If found, it returns the corresponding [**Entity**](class_a_g_e_1_1_entity.md) object.




**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the entity to retrieve. 



**Returns:**

An [**Entity**](class_a_g_e_1_1_entity.md) object representing the entity with the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md), or an empty [**Entity**](class_a_g_e_1_1_entity.md) if no such entity exists in the scene.


Retrieves an entity from the scene using its [**UUID**](class_a_g_e_1_1_u_u_i_d.md).


This function iterates over all entities in the scene and checks if their [**IDComponent**](struct_a_g_e_1_1_i_d_component.md) has the same [**UUID**](class_a_g_e_1_1_u_u_i_d.md) as the input parameter 'uuid'. If a match is found, it returns that entity. Otherwise, it returns an empty entity. 

**Parameters:**


* `uuid` The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the entity to retrieve. 



**Returns:**

[**Entity**](class_a_g_e_1_1_entity.md) The matching entity or an empty entity if no match was found. 





        

<hr>



### function GetName 

_Returns the name of the object._ 
```C++
inline std::string & AGE::Scene::GetName () 
```



This function returns a reference to the internal string that holds the name of the object. The returned value can be modified by the caller, allowing for dynamic changes in the name.




**Returns:**

A reference to the internal string holding the name.


Gets the name of the object.


This function returns a reference to the internal string that holds the name of the object. The caller can modify this string, and the changes will be reflected in the object's state.




**Returns:**

A reference to the internal string holding the name. 





        

<hr>



### function GetPrimaryCameraEntity 

_This function returns the primary camera entity in the scene._ 
```C++
Entity AGE::Scene::GetPrimaryCameraEntity () 
```



The function iterates over all entities with a [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) and checks if any of them is marked as primary. If it finds one, it returns that entity. Otherwise, it returns an empty entity.




**Returns:**

[**Entity**](class_a_g_e_1_1_entity.md) - The primary camera entity in the scene. Returns an empty entity if no primary camera exists.


This function returns the primary camera entity in the scene.


The function iterates over all entities with a [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) and checks if any of them is marked as primary. If it finds one, it returns that entity. Otherwise, it returns an empty entity.




**Returns:**

[**Entity**](class_a_g_e_1_1_entity.md) - The primary camera entity in the scene. Returns an empty entity if no primary camera exists. 





        

<hr>



### function OnEditorUpdate 

```C++
void AGE::Scene::OnEditorUpdate (
    TimeStep DeltaTime,
    EditorCamera & Camera
) 
```




<hr>



### function OnRuntimeStart 

```C++
void AGE::Scene::OnRuntimeStart () 
```




<hr>



### function OnRuntimeStop 

_This function is called when the runtime of the application stops. It unloads sounds, destroys the physics world and resets all native script instances._ 
```C++
void AGE::Scene::OnRuntimeStop () 
```





**Parameters:**


* `None` 



**Returns:**

void


This function is called when the runtime of the application stops. It unloads sounds, destroys the physics world and resets all native script instances.




**Parameters:**


* `None` 



**Returns:**

void 





        

<hr>



### function OnRuntimeUpdate 

```C++
void AGE::Scene::OnRuntimeUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function OnViewportResize 

_This function is called when the viewport size changes. It updates all camera components to reflect the new viewport dimensions._ 
```C++
void AGE::Scene::OnViewportResize (
    uint32_t Width,
    uint32_t Height
) 
```





**Parameters:**


* `Width` The new width of the viewport. 
* `Height` The new height of the viewport.



**Returns:**

None


This function is called when the viewport size changes. It updates all camera components with a fixed aspect ratio to match the new viewport size.




**Parameters:**


* `Width` The new width of the viewport. 
* `Height` The new height of the viewport. 




        

<hr>



### function Scene [1/4]

```C++
AGE::Scene::Scene () 
```




<hr>



### function Scene [2/4]

_Copy constructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class is deleted to prevent copying of objects._
```C++
AGE::Scene::Scene (
    const Scene & Other
) = delete
```



The copy constructor for the [**Scene**](class_a_g_e_1_1_scene.md) class is explicitly marked as deleted in order to prevent accidental copying of [**Scene**](class_a_g_e_1_1_scene.md) objects. This is because the [**Scene**](class_a_g_e_1_1_scene.md) class represents a complex data structure that should not be copied unintentionally, leading to unnecessary memory usage and potential issues with object state management.




**Parameters:**


* `Other` The [**Scene**](class_a_g_e_1_1_scene.md) object to copy from.

Copy constructor for the [**Scene**](class_a_g_e_1_1_scene.md) class is deleted to prevent copying of objects.


This function is marked as deleted in order to prevent accidental copy of objects. It's important because it ensures that each object has its own resources and can't be copied from another one without proper management.




**Parameters:**


* `Other` The [**Scene**](class_a_g_e_1_1_scene.md) object to be copied. 




        

<hr>



### function Scene [3/4]

_Constructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._
```C++
inline AGE::Scene::Scene (
    UUID ID
) 
```





**Parameters:**


* `ID` The unique identifier of the scene.

Constructs a [**Scene**](class_a_g_e_1_1_scene.md) object with the given [**UUID**](class_a_g_e_1_1_u_u_i_d.md). 

**Parameters:**


* `ID` The unique identifier for this scene. 




        

<hr>



### function Scene [4/4]

_Constructs a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object with the given name and generates an unique asset ID._
```C++
inline AGE::Scene::Scene (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The name of the scene.

Constructs a [**Scene**](class_a_g_e_1_1_scene.md) object with the given name and generates a unique asset ID. 

**Parameters:**


* `Name` The name of the scene. 




        

<hr>



### function SetEventCallback 

_This function sets the callback for handling events._ 
```C++
inline void AGE::Scene::SetEventCallback (
    const std::function< void( Event &)> & Callback
) 
```





**Parameters:**


* `Callback` The function to be called when an event occurs. It takes an [**Event**](class_a_g_e_1_1_event.md)& parameter and returns void. 



**Returns:**

Unknown


This function sets the callback for handling events. 

**Parameters:**


* `Callback` The function to be called when an event occurs. It takes an [**Event**](class_a_g_e_1_1_event.md)& as a parameter and returns void. 



**Returns:**

Unknown 





        

<hr>



### function SetSceneName 

_Sets the name of the scene._ 
```C++
inline void AGE::Scene::SetSceneName (
    const std::string & Name
) 
```



This function sets the name of the scene to a given string value. The new name is stored in member variable `m_Name`.




**Parameters:**


* `Name` - A const reference to the string that will be used as the new name for the scene.

Sets the scene name.


This function sets the scene name to a given string value. The new name is stored in member variable `m_Name`.




**Parameters:**


* `Name` - A const reference to the string that will be set as the new scene name. 




        

<hr>



### function operator= 

_Copy assignment operator for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._
```C++
inline void AGE::Scene::operator= (
    const Scene & Other
) 
```



This function is used to assign the values of one [**Scene**](class_a_g_e_1_1_scene.md) object to another. It takes a constant reference to a [**Scene**](class_a_g_e_1_1_scene.md) object as its parameter, and returns a reference to the current [**Scene**](class_a_g_e_1_1_scene.md) object.




**Parameters:**


* `Other` The [**Scene**](class_a_g_e_1_1_scene.md) object to copy from. 



**Returns:**

A reference to the current [**Scene**](class_a_g_e_1_1_scene.md) object after copying.


Copy assignment operator for the [**Scene**](class_a_g_e_1_1_scene.md) class.


This function is used to assign one scene object to another. It takes a constant reference to a [**Scene**](class_a_g_e_1_1_scene.md) object as its parameter and returns nothing. The function does not throw any exceptions.




**Parameters:**


* `Other` A const reference to a [**Scene**](class_a_g_e_1_1_scene.md) object that we want to copy into the current object. 




        

<hr>



### function ~Scene 

_Destructor for the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _class._
```C++
AGE::Scene::~Scene () 
```



This function is responsible for cleaning up any resources that were allocated during the lifetime of a [**Scene**](class_a_g_e_1_1_scene.md) object. It currently does not perform any specific cleanup actions as there are no dynamically allocated resources in the [**Scene**](class_a_g_e_1_1_scene.md) class.




**Returns:**

void


Destructor for the [**Scene**](class_a_g_e_1_1_scene.md) class.


This function is responsible for cleaning up any resources that were allocated during the lifetime of a [**Scene**](class_a_g_e_1_1_scene.md) object, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function BuildAllScenes 

```C++
static void AGE::Scene::BuildAllScenes () 
```




<hr>



### function Deserialize 

_Deserialize a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
static void AGE::Scene::Deserialize (
    DataReader * Deserializer,
    Scene & Data
) 
```



This function reads the necessary data to reconstruct a [**Scene**](class_a_g_e_1_1_scene.md) object from a [**DataReader**](class_a_g_e_1_1_data_reader.md). The [**Scene**](class_a_g_e_1_1_scene.md) object's name, viewport width and height as well as its [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) are read.




**Parameters:**


* `Deserializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` The [**Scene**](class_a_g_e_1_1_scene.md) object to be deserialized.



**Returns:**

void


Deserialize a [**Scene**](class_a_g_e_1_1_scene.md) object from a [**DataReader**](class_a_g_e_1_1_data_reader.md).


This function reads the necessary data to reconstruct a [**Scene**](class_a_g_e_1_1_scene.md) object from a [**DataReader**](class_a_g_e_1_1_data_reader.md). The [**Scene**](class_a_g_e_1_1_scene.md) object's name, viewport width and height as well as its [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) are read.




**Parameters:**


* `Deserializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` The [**Scene**](class_a_g_e_1_1_scene.md) object to be deserialized. 




        

<hr>



### function LoadScene 

_Loads a scene from the specified file path._ 
```C++
static Ref< Scene > AGE::Scene::LoadScene (
    const std::filesystem::path & Path
) 
```



This function deserializes a scene from a JSON file and returns it as a `Ref< Scene >` object. The scene is loaded into an empty `Ref< Scene >` object, which can be accessed through the returned reference.




**Parameters:**


* `Path` The filesystem path to the JSON file containing the serialized scene data. 



**Returns:**

A reference to the loaded scene.


Loads a scene from the specified file path.


This function deserializes a scene from a JSON file located at the provided path and returns it as a `Ref< Scene >` object. The returned reference can be used to access and manipulate the loaded scene.




**Parameters:**


* `Path` The filesystem path of the scene file to load. 



**Returns:**

A reference to the loaded scene. 





        

<hr>



### function Serialize 

_This function serializes a_ [_**Scene**_](class_a_g_e_1_1_scene.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static void AGE::Scene::Serialize (
    DataWriter * Serializer,
    const Scene & Data
) 
```



The function writes the size of the scene name, the scene name itself, the viewport width and height, and the scene info to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) where the serialized data will be written. 
* `Data` Const reference to the [**Scene**](class_a_g_e_1_1_scene.md) object that is being serialized.

This function serializes a [**Scene**](class_a_g_e_1_1_scene.md) object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md).


The function writes the size of the scene name, the scene name itself, the viewport width and height, and the scene info to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) where the serialized data will be written. 
* `Data` Const reference to the [**Scene**](class_a_g_e_1_1_scene.md) object that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Scene.h`

