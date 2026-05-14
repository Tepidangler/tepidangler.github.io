

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
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene) () <br>_Returns the current scene object._  |
|   | [**SceneChangedEvent**](#function-scenechangedevent) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Scene) <br>_Constructs a new instance of the_ [_**SceneChangedEvent**_](class_a_g_e_1_1_scene_changed_event.md) _class with the given scene reference._ |




## Public Functions inherited from AGE::Event

See [AGE::Event](class_a_g_e_1_1_event.md)

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](class_a_g_e_1_1_event.md#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](class_a_g_e_1_1_event.md#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](class_a_g_e_1_1_event.md#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](class_a_g_e_1_1_event.md#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](class_a_g_e_1_1_event.md#function-tostring) () const<br>_Returns a string representation of the object._  |






















## Protected Attributes inherited from AGE::SceneEvent

See [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**m\_Scene**](class_a_g_e_1_1_scene_event.md#variable-m_scene)  <br> |
















































## Protected Functions inherited from AGE::SceneEvent

See [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md)

| Type | Name |
| ---: | :--- |
|   | [**SceneEvent**](class_a_g_e_1_1_scene_event.md#function-sceneevent) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; Scene) <br>_Constructs a new instance of the_ [_**SceneEvent**_](class_a_g_e_1_1_scene_event.md) _class with the given scene._ |










## Public Functions Documentation




### function GetScene 

_Returns the current scene object._ 
```C++
inline Ref< Scene > AGE::SceneChangedEvent::GetScene () 
```



This function returns a reference to the currently active scene in the application. The returned [**Scene**](class_a_g_e_1_1_scene.md) object can be used for various operations such as rendering, updating, and managing game objects within the scene.




**Returns:**

A reference to the current scene.


Returns the current scene object.


This function retrieves and returns the currently active [**Scene**](class_a_g_e_1_1_scene.md) object, which is stored in the member variable 'm\_Scene'. The returned reference can be used to manipulate or access the properties of this [**Scene**](class_a_g_e_1_1_scene.md) object.




**Returns:**

A reference to the current [**Scene**](class_a_g_e_1_1_scene.md) object. 





        

<hr>



### function SceneChangedEvent 

_Constructs a new instance of the_ [_**SceneChangedEvent**_](class_a_g_e_1_1_scene_changed_event.md) _class with the given scene reference._
```C++
inline AGE::SceneChangedEvent::SceneChangedEvent (
    Ref< Scene > Scene
) 
```





**Parameters:**


* [**Scene**](class_a_g_e_1_1_scene.md) The scene that has changed.

Constructs a new instance of the [**SceneChangedEvent**](class_a_g_e_1_1_scene_changed_event.md) class with the given scene.




**Parameters:**


* [**Scene**](class_a_g_e_1_1_scene.md) The scene that has changed. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/GameEvent.h`

