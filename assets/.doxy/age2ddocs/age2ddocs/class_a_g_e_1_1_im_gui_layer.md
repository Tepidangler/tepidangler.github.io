

# Class AGE::ImGuiLayer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md)



_This class represents the ImGui layer in a system. It is responsible for rendering and handling user interface events._ [More...](#detailed-description)

* `#include <ImGuiLayer.h>`



Inherits the following classes: [AGE::Layer](class_a_g_e_1_1_layer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Begin**](#function-begin) () <br>_Begins the ImGui layer. This function prepares for rendering of UI elements by initializing necessary states and setting up frame data based on the current render API in use._  |
|  void | [**BlockEvents**](#function-blockevents) (bool block) <br>_This function is used to set the state of event blocking in a system._  |
| virtual void | [**End**](#function-end) () <br>_This function is responsible for ending the ImGui layer and rendering the GUI. It updates the display size based on the window's width and height, then renders the GUI using either OpenGL or a different API depending on the current_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API. If an invalid Render API is selected, it asserts false with a message "Invalid Render API Selected!"._ |
|   | [**ImGuiLayer**](#function-imguilayer) () <br>[_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _is a class representing the layer for handling user interface elements with ImGui library in our application._ |
| virtual void | [**OnAttach**](#function-onattach) () override<br>_This function is called when the object is attached to a scene or game world._  |
| virtual void | [**OnDetach**](#function-ondetach) () override<br>_This function is called when the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _detaches from its attached renderer. It handles cleanup based on which rendering API was selected at runtime._ |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) override<br>_This function is an event handler for the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _class. It dispatches events to their respective handlers based on the event type._ |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_This function is responsible for rendering the ImGui interface elements in the application._  |
|   | [**~ImGuiLayer**](#function-imguilayer) () <br>_Destructor for the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _class._ |


## Public Functions inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetName**](class_a_g_e_1_1_layer.md#function-getname) () const<br>_Returns the name of this object._  |
|  float | [**GetTime**](class_a_g_e_1_1_layer.md#function-gettime) () <br>_Get the current time in seconds since GLFW was initialized._  |
| virtual void | [**Init**](class_a_g_e_1_1_layer.md#function-init) () <br> |
|   | [**Layer**](class_a_g_e_1_1_layer.md#function-layer) (const std::string & name="Layer") <br>_Constructs a_ [_**Layer**_](class_a_g_e_1_1_layer.md) _object with the given debug name._ |
| virtual void | [**OnAttach**](class_a_g_e_1_1_layer.md#function-onattach) () <br>_This function is called when the object is attached to a scene or game world._  |
| virtual void | [**OnDetach**](class_a_g_e_1_1_layer.md#function-ondetach) () <br>_Detaches the component from its parent._  |
| virtual void | [**OnEvent**](class_a_g_e_1_1_layer.md#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br>_This function is called when an event occurs._  |
| virtual void | [**OnImGuiRender**](class_a_g_e_1_1_layer.md#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is called every frame to render the ImGUI interface._  |
| virtual void | [**OnUpdate**](class_a_g_e_1_1_layer.md#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is called every frame to update the game state._  |
| virtual  | [**~Layer**](class_a_g_e_1_1_layer.md#function-layer) () <br>_Destructor for the_ [_**Layer**_](class_a_g_e_1_1_layer.md) _class._ |
















## Protected Attributes inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](class_a_g_e_1_1_layer.md#variable-m_debugname)  <br> |






































## Detailed Description


The [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) class provides methods to attach, detach, render GUI elements using ImGui, block or unblock events, start and end the GUI session respectively. 


    
## Public Functions Documentation




### function Begin 

_Begins the ImGui layer. This function prepares for rendering of UI elements by initializing necessary states and setting up frame data based on the current render API in use._ 
```C++
virtual void AGE::ImGuiLayer::Begin () 
```



The function first checks the currently selected Render API using `Renderer::GetAPI()`. Depending on the result, it performs different actions:
* If the API is OpenGL (0), no action is taken as there are no UI elements to initialize for this case.
* If the API is DirectX or Vulkan (1), it calls ImGui's NewFrame function and sets up frame data for these APIs using `ImGui_ImplOpenGL3_NewFrame()`, `ImGui_ImplGlfw_NewFrame()`, and `ImGuizmo::BeginFrame()`.
* If an invalid API is selected (anything else), it asserts false with a message "Invalid Render API Selected!" to halt execution.






**Returns:**

void


Begins the ImGui layer. This function initializes the ImGui context based on the currently selected render API.


The [**Renderer::GetAPI()**](class_a_g_e_1_1_renderer.md#function-getapi) function is used to determine which render API is in use. Depending on this, different actions are taken:
* If the OpenGL API is being used (case 1), then the ImGui\_ImplOpenGL3\_NewFrame(), ImGui\_ImplGlfw\_NewFrame(), and ImGui::NewFrame() functions are called to prepare for a new frame. Additionally, if not in distribution mode (AG\_DIST), ImGuizmo::BeginFrame() is also called.
* If an invalid render API is selected (default case), then an assertion failure occurs with the message "Invalid Render API Selected!".






**Returns:**

void 





        

<hr>



### function BlockEvents 

_This function is used to set the state of event blocking in a system._ 
```C++
inline void AGE::ImGuiLayer::BlockEvents (
    bool block
) 
```





**Parameters:**


* `block` A boolean value indicating whether events should be blocked or not. 



**Returns:**

None


This function is used to set the state of event blocking in a system. 

**Parameters:**


* `block` A boolean value indicating whether events should be blocked or not. 



**Returns:**

None 





        

<hr>



### function End 

_This function is responsible for ending the ImGui layer and rendering the GUI. It updates the display size based on the window's width and height, then renders the GUI using either OpenGL or a different API depending on the current_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _API. If an invalid Render API is selected, it asserts false with a message "Invalid Render API Selected!"._
```C++
virtual void AGE::ImGuiLayer::End () 
```





**Returns:**

void


This function is responsible for ending the ImGui layer and rendering it. It also updates the display size based on the window's width and height.




**Parameters:**


* `None` 



**Returns:**

void 





        

<hr>



### function ImGuiLayer 

[_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _is a class representing the layer for handling user interface elements with ImGui library in our application._
```C++
AGE::ImGuiLayer::ImGuiLayer () 
```



[**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) is a class representing the layer for handling user interface elements with ImGui library in our application. It extends the base [**Layer**](class_a_g_e_1_1_layer.md) class and provides additional functionality specific to this library. 


        

<hr>



### function OnAttach 

_This function is called when the object is attached to a scene or game world._ 
```C++
virtual void AGE::ImGuiLayer::OnAttach () override
```





**Returns:**

void


This function is called when the component is attached to a scene.




**Returns:**

void 





        
Implements [*AGE::Layer::OnAttach*](class_a_g_e_1_1_layer.md#function-onattach)


<hr>



### function OnDetach 

_This function is called when the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _detaches from its attached renderer. It handles cleanup based on which rendering API was selected at runtime._
```C++
virtual void AGE::ImGuiLayer::OnDetach () override
```





**Returns:**

void


Detaches the ImGui layer.


This function is responsible for detaching the ImGui layer from the application. It does this by shutting down the necessary components based on the current render API in use.




**Returns:**

void 





        
Implements [*AGE::Layer::OnDetach*](class_a_g_e_1_1_layer.md#function-ondetach)


<hr>



### function OnEvent 

_This function is an event handler for the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _class. It dispatches events to their respective handlers based on the event type._
```C++
virtual void AGE::ImGuiLayer::OnEvent (
    Event & E
) override
```





**Parameters:**


* `E` Reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs to be handled.

Handles events dispatched by the application.


This function is responsible for dispatching events to their respective handlers. It uses an event dispatcher to handle different types of events, such as window resizing events. The function also checks if event blocking is enabled and updates the ImGui IO accordingly.




**Parameters:**


* `E` Reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs to be handled. 




        
Implements [*AGE::Layer::OnEvent*](class_a_g_e_1_1_layer.md#function-onevent)


<hr>



### function OnImGuiRender 

_This function is responsible for rendering the ImGui interface elements in the application._ 
```C++
virtual void AGE::ImGuiLayer::OnImGuiRender (
    TimeStep DeltaTime
) override
```





**Parameters:**


* `DeltaTime` The time step representing the elapsed time since the last frame.



**Returns:**

void No return value expected as this function does not explicitly return anything.


This function is used to render the ImGui interface elements for a specific layer.




**Parameters:**


* `DeltaTime` The time step representing the elapsed time since the last frame. 




        
Implements [*AGE::Layer::OnImGuiRender*](class_a_g_e_1_1_layer.md#function-onimguirender)


<hr>



### function ~ImGuiLayer 

_Destructor for the_ [_**ImGuiLayer**_](class_a_g_e_1_1_im_gui_layer.md) _class._
```C++
AGE::ImGuiLayer::~ImGuiLayer () 
```



Destructor for the [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) class. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/ImGui/Public/ImGuiLayer.h`

