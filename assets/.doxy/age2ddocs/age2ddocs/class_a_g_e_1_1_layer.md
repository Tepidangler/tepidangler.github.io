

# Class AGE::Layer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Layer**](class_a_g_e_1_1_layer.md)










Inherited by the following classes: [AGE::ImGuiLayer](class_a_g_e_1_1_im_gui_layer.md),  [AGE::NodeEditorWindow](class_a_g_e_1_1_node_editor_window.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetName**](#function-getname) () const<br>_Returns the name of this object._  |
|  float | [**GetTime**](#function-gettime) () <br>_Get the current time in seconds since GLFW was initialized._  |
| virtual void | [**Init**](#function-init) () <br> |
|   | [**Layer**](#function-layer) (const std::string & name="Layer") <br>_Constructs a_ [_**Layer**_](class_a_g_e_1_1_layer.md) _object with the given debug name._ |
| virtual void | [**OnAttach**](#function-onattach) () <br>_This function is called when the object is attached to a scene or game world._  |
| virtual void | [**OnDetach**](#function-ondetach) () <br>_Detaches the component from its parent._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br>_This function is called when an event occurs._  |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is called every frame to render the ImGUI interface._  |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is called every frame to update the game state._  |
| virtual  | [**~Layer**](#function-layer) () <br>_Destructor for the_ [_**Layer**_](class_a_g_e_1_1_layer.md) _class._ |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](#variable-m_debugname)  <br> |




















## Public Functions Documentation




### function GetName 

_Returns the name of this object._ 
```C++
inline const std::string & AGE::Layer::GetName () const
```



This function returns a reference to a string that represents the name of this object. The returned value is constant and does not allow modification.




**Returns:**

A const reference to the debug name of this object.


Returns the name of this object. 

**Returns:**

A constant reference to a string containing the debug name. 





        

<hr>



### function GetTime 

_Get the current time in seconds since GLFW was initialized._ 
```C++
float AGE::Layer::GetTime () 
```



This function uses glfwGetTime(), which returns the time in seconds since GLFW was initialized. The returned value is a double precision floating point number, so it can be used for more precise timing measurements.




**Returns:**

A float representing the current time in seconds.


This function returns the time in seconds since GLFW was initialized, as a floating-point number. 

**Returns:**

A float representing the current time in seconds. 





        

<hr>



### function Init 

```C++
inline virtual void AGE::Layer::Init () 
```




<hr>



### function Layer 

_Constructs a_ [_**Layer**_](class_a_g_e_1_1_layer.md) _object with the given debug name._
```C++
AGE::Layer::Layer (
    const std::string & name="Layer"
) 
```



This function is used to create a new [**Layer**](class_a_g_e_1_1_layer.md) object, which can be used for various purposes such as logging or debugging. The debug name provided will be stored and can be accessed later using getDebugName() method.




**Parameters:**


* `DebugName` A string representing the debug name of the layer.

Constructs a [**Layer**](class_a_g_e_1_1_layer.md) object with the given debug name.


This function is used to create a new [**Layer**](class_a_g_e_1_1_layer.md) object with a specific debug name. The debug name can be used for debugging purposes and provides context about the layer's purpose or functionality.




**Parameters:**


* `DebugName` A string representing the debug name of the layer. 




        

<hr>



### function OnAttach 

_This function is called when the object is attached to a scene or game world._ 
```C++
inline virtual void AGE::Layer::OnAttach () 
```





**Returns:**

void


This function is called when the component is attached to a scene.




**Returns:**

void 





        

<hr>



### function OnDetach 

_Detaches the component from its parent._ 
```C++
inline virtual void AGE::Layer::OnDetach () 
```



This function is called when a component is detached from its parent. It provides an opportunity for any necessary cleanup or notification to be done before the component is completely removed from use.




**Returns:**

void


Detaches the component from its parent.


This function is called when a component is detached from its parent. It provides an opportunity for any necessary cleanup or notification to be done.




**Returns:**

void 





        

<hr>



### function OnEvent 

_This function is called when an event occurs._ 
```C++
inline virtual void AGE::Layer::OnEvent (
    Event & Event
) 
```



The function takes a reference to an [**Event**](class_a_g_e_1_1_event.md) object as its parameter, which contains information about the event that occurred. It does not return anything (void).




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - A reference to an [**Event**](class_a_g_e_1_1_event.md) object containing details about the event.

This function is called when an event occurs.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event that has occurred. 




        

<hr>



### function OnImGuiRender 

_This function is called every frame to render the ImGUI interface._ 
```C++
inline virtual void AGE::Layer::OnImGuiRender (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The time step for the current frame, indicating how much time has passed since the last frame. 



**Returns:**

void No return value expected as this function does not return any result.


This function is called every frame to render the ImGui interface.




**Parameters:**


* `DeltaTime` The time step for the current frame, indicating how much time has passed since the last frame. 




        

<hr>



### function OnUpdate 

_This function is called every frame to update the game state._ 
```C++
inline virtual void AGE::Layer::OnUpdate (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The time elapsed since the last frame, used for smooth movement and animation. 



**Returns:**

void No return value expected as this function does not have a return statement.


This function is called every frame to update the game state based on the elapsed time since the last call.




**Parameters:**


* `DeltaTime` The time step between the current and previous frames, used to calculate how much of an effect should be applied. 




        

<hr>



### function ~Layer 

_Destructor for the_ [_**Layer**_](class_a_g_e_1_1_layer.md) _class._
```C++
virtual AGE::Layer::~Layer () 
```



This destructor does not perform any specific actions when called, but it is a necessary part of the class's interface as it releases any resources that were acquired during the lifetime of an object of this class.




**Returns:**

None.


Destructor for the [**Layer**](class_a_g_e_1_1_layer.md) class. 


        

<hr>
## Protected Attributes Documentation




### variable m\_DebugName 

```C++
std::string AGE::Layer::m_DebugName;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Layer.h`

