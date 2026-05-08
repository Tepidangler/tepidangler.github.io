

# Class AGE::SceneChangedEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneChangedEvent**](class_a_g_e_1_1_scene_changed_event.md)








Inherits the following classes: [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md)






























## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |












































## Public Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene) () <br> |
|   | [**SceneChangedEvent**](#function-scenechangedevent) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Scene) <br> |




## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br> |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br> |






















## Protected Attributes inherited from AGE::SceneEvent

See [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**m\_Scene**](class_a_g_e_1_1_scene_event.md#variable-m_scene)  <br> |
















































## Protected Functions inherited from AGE::SceneEvent

See [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md)

| Type | Name |
| ---: | :--- |
|   | [**SceneEvent**](class_a_g_e_1_1_scene_event.md#function-sceneevent) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Scene) <br> |










## Public Functions Documentation




### function GetScene 

```C++
inline Ref< Scene > AGE::SceneChangedEvent::GetScene () 
```




<hr>



### function SceneChangedEvent 

```C++
inline AGE::SceneChangedEvent::SceneChangedEvent (
    Ref< Scene > Scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

