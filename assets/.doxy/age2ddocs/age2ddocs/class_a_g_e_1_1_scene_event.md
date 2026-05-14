

# Class AGE::SceneEvent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneEvent**](class_a_g_e_1_1_scene_event.md)








Inherits the following classes: [AGE::Event](class_a_g_e_1_1_event.md)


Inherited by the following classes: [AGE::SceneChangedEvent](class_a_g_e_1_1_scene_changed_event.md)






















## Public Attributes inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](class_a_g_e_1_1_event.md#variable-handled)   = `false`<br> |
































## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |














## Protected Attributes

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**m\_Scene**](#variable-m_scene)  <br> |
































## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**SceneEvent**](#function-sceneevent) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Scene) <br>_Constructs a new instance of the_ [_**SceneEvent**_](class_a_g_e_1_1_scene_event.md) _class with the given scene._ |








## Protected Attributes Documentation




### variable m\_Scene 

```C++
Ref<Scene> AGE::SceneEvent::m_Scene;
```




<hr>
## Protected Functions Documentation




### function SceneEvent 

_Constructs a new instance of the_ [_**SceneEvent**_](class_a_g_e_1_1_scene_event.md) _class with the given scene._
```C++
inline AGE::SceneEvent::SceneEvent (
    Ref< Scene > Scene
) 
```





**Parameters:**


* [**Scene**](class_a_g_e_1_1_scene.md) The scene to be associated with this event.

Constructs a new instance of the [**SceneEvent**](class_a_g_e_1_1_scene_event.md) class with the given scene. 

**Parameters:**


* [**Scene**](class_a_g_e_1_1_scene.md) The reference to the scene that this event is associated with. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

