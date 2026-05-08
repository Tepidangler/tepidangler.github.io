

# Class AGE::Scene



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Scene**](class_a_g_e_1_1_scene.md)








Inherits the following classes: std::enable_shared_from_this< Scene >


































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**BroadcastEvent**](#function-broadcastevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br> |
|  void | [**BuildScene**](#function-buildscene) (const std::filesystem::path & ProjectPath) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**Copy**](#function-copy) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Other) <br> |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**CreateEntity**](#function-createentity) (const std::string Name="") <br> |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**CreateEntityWithUUID**](#function-createentitywithuuid) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) uuid, const std::string & Name=std::string()) <br> |
|  void | [**DestoryEntity**](#function-destoryentity) ([**Entity**](class_a_g_e_1_1_entity.md) E) <br> |
|  void | [**DuplicateEntity**](#function-duplicateentity) ([**Entity**](class_a_g_e_1_1_entity.md) entity) <br> |
|  auto | [**GetAllEntitiesWith**](#function-getallentitieswith) () <br> |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br> |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**GetEntityFromUUID**](#function-getentityfromuuid) (const uint64\_t uuid) <br> |
|  std::string & | [**GetName**](#function-getname) () <br> |
|  [**Entity**](class_a_g_e_1_1_entity.md) | [**GetPrimaryCameraEntity**](#function-getprimarycameraentity) () <br> |
|  void | [**OnEditorUpdate**](#function-oneditorupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime, [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br> |
|  void | [**OnRuntimeStart**](#function-onruntimestart) () <br> |
|  void | [**OnRuntimeStop**](#function-onruntimestop) () <br> |
|  void | [**OnRuntimeUpdate**](#function-onruntimeupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**OnViewportResize**](#function-onviewportresize) (uint32\_t Width, uint32\_t Height) <br> |
|   | [**Scene**](#function-scene-14) () <br> |
|   | [**Scene**](#function-scene-24) (const [**Scene**](class_a_g_e_1_1_scene.md) & Other) = delete<br> |
|   | [**Scene**](#function-scene-34) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|   | [**Scene**](#function-scene-44) (const std::string & Name) <br> |
|  void | [**SetEventCallback**](#function-seteventcallback) (const std::function&lt; void([**Event**](class_a_g_e_1_1_event.md) &)&gt; & Callback) <br> |
|  void | [**SetSceneName**](#function-setscenename) (const std::string & Name) <br> |
|  void | [**operator=**](#function-operator) (const [**Scene**](class_a_g_e_1_1_scene.md) & Other) <br> |
|   | [**~Scene**](#function-scene) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BuildAllScenes**](#function-buildallscenes) () <br> |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Scene**](class_a_g_e_1_1_scene.md) & Data) <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**LoadScene**](#function-loadscene) (const std::filesystem::path & Path) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Scene**](class_a_g_e_1_1_scene.md) & Data) <br> |


























## Public Functions Documentation




### function BroadcastEvent 

```C++
inline void AGE::Scene::BroadcastEvent (
    Event & Event
) 
```




<hr>



### function BuildScene 

```C++
void AGE::Scene::BuildScene (
    const std::filesystem::path & ProjectPath
) 
```




<hr>



### function Copy 

```C++
Ref< Scene > AGE::Scene::Copy (
    Ref< Scene > Other
) 
```




<hr>



### function CreateEntity 

```C++
Entity AGE::Scene::CreateEntity (
    const std::string Name=""
) 
```




<hr>



### function CreateEntityWithUUID 

```C++
Entity AGE::Scene::CreateEntityWithUUID (
    UUID uuid,
    const std::string & Name=std::string()
) 
```




<hr>



### function DestoryEntity 

```C++
void AGE::Scene::DestoryEntity (
    Entity E
) 
```




<hr>



### function DuplicateEntity 

```C++
void AGE::Scene::DuplicateEntity (
    Entity entity
) 
```




<hr>



### function GetAllEntitiesWith 

```C++
template<typename... Components>
inline auto AGE::Scene::GetAllEntitiesWith () 
```




<hr>



### function GetAssetID 

```C++
inline UUID & AGE::Scene::GetAssetID () 
```




<hr>



### function GetEntityFromUUID 

```C++
Entity AGE::Scene::GetEntityFromUUID (
    const uint64_t uuid
) 
```




<hr>



### function GetName 

```C++
inline std::string & AGE::Scene::GetName () 
```




<hr>



### function GetPrimaryCameraEntity 

```C++
Entity AGE::Scene::GetPrimaryCameraEntity () 
```




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

```C++
void AGE::Scene::OnRuntimeStop () 
```




<hr>



### function OnRuntimeUpdate 

```C++
void AGE::Scene::OnRuntimeUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function OnViewportResize 

```C++
void AGE::Scene::OnViewportResize (
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function Scene [1/4]

```C++
AGE::Scene::Scene () 
```




<hr>



### function Scene [2/4]

```C++
AGE::Scene::Scene (
    const Scene & Other
) = delete
```




<hr>



### function Scene [3/4]

```C++
inline AGE::Scene::Scene (
    UUID ID
) 
```




<hr>



### function Scene [4/4]

```C++
inline AGE::Scene::Scene (
    const std::string & Name
) 
```




<hr>



### function SetEventCallback 

```C++
inline void AGE::Scene::SetEventCallback (
    const std::function< void( Event &)> & Callback
) 
```




<hr>



### function SetSceneName 

```C++
inline void AGE::Scene::SetSceneName (
    const std::string & Name
) 
```




<hr>



### function operator= 

```C++
inline void AGE::Scene::operator= (
    const Scene & Other
) 
```




<hr>



### function ~Scene 

```C++
AGE::Scene::~Scene () 
```




<hr>
## Public Static Functions Documentation




### function BuildAllScenes 

```C++
static void AGE::Scene::BuildAllScenes () 
```




<hr>



### function Deserialize 

```C++
static void AGE::Scene::Deserialize (
    DataReader * Deserializer,
    Scene & Data
) 
```




<hr>



### function LoadScene 

```C++
static Ref< Scene > AGE::Scene::LoadScene (
    const std::filesystem::path & Path
) 
```




<hr>



### function Serialize 

```C++
static void AGE::Scene::Serialize (
    DataWriter * Serializer,
    const Scene & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Scene.h`

