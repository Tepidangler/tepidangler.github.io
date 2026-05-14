

# Class AGE::App



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**App**](class_a_g_e_1_1_app.md)



_The main application class._ [More...](#detailed-description)

* `#include <App.h>`





































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**App**](#function-app) (const std::string & name="AGE App", [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) Args=[**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md)()) <br> |
|  void | [**Close**](#function-close) () <br>_Closes the application by setting m\_Running to false._  |
|  [**AppConfig**](struct_a_g_e_1_1_app_config.md) & | [**GetAppConfig**](#function-getappconfig) () <br>_Returns the application configuration object._  |
|  [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) | [**GetCommandLineArgs**](#function-getcommandlineargs) () const<br>_Retrieves the command line arguments of the application._  |
|  [**DeviceManager**](class_a_g_e_1_1_device_manager.md) & | [**GetDeviceManager**](#function-getdevicemanager) () <br>_Returns a reference to the device manager instance._  |
|  void | [**GetDirectXErrorMessages**](#function-getdirectxerrormessages) () <br>_This function retrieves DirectX error messages._  |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**GetFramebufferSize**](#function-getframebuffersize) () <br>_Returns the framebuffer size of the application._  |
|  [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) \* | [**GetImGuiLayer**](#function-getimguilayer) () <br>_This function returns the ImGui layer of the application._  |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; & | [**GetProject**](#function-getproject) () <br>_Returns a reference to the_ [_**Project**_](class_a_g_e_1_1_project.md) _object._ |
|  uint16\_t | [**GetTargetPlatform**](#function-gettargetplatform) () <br>_This function returns the target platform._  |
|  void | [**Init**](#function-init) () <br>_Initializes the application. This function sets up various components of the app such as device manager, asset manager and ImGui layer._  |
|  void | [**InitLayers**](#function-initlayers) () <br>_Initializes and attaches all layers in the layer stack._  |
|  void | [**InitRenderer**](#function-initrenderer) () <br>_Initializes the renderer._  |
|  void | [**LoadAssets**](#function-loadassets) () <br>_Loads assets asynchronously in separate threads._  |
|  void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br>_Handles an event dispatched by the application._  |
|  void | [**PushLayer**](#function-pushlayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br>_Pushes a layer onto the stack and attaches it._  |
|  void | [**PushOverlay**](#function-pushoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br>_Pushes an overlay layer onto the stack and calls its OnAttach() function._  |
|  void | [**PushScriptableComp**](#function-pushscriptablecomp) ([**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* Comp) <br>_Pushes a_ [_**ScriptableEntity**_](class_a_g_e_1_1_scriptable_entity.md) _component onto the stack._ |
|  void | [**Run**](#function-run) () <br> |
|  void | [**SetProject**](#function-setproject) (Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; Proj) <br>_Sets the project object._  |
|  void | [**SetTargetPlatform**](#function-settargetplatform) (uint16\_t Target) <br>_Sets the target platform to a specified value._  |
|  void | [**Shutdown**](#function-shutdown) () <br>_This function is used to shutdown the application. It sets a flag indicating that the program is no longer running, and then shuts down the renderer._  |
| virtual  | [**~App**](#function-app) () <br>_Destructor for the_ [_**App**_](class_a_g_e_1_1_app.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**App**](class_a_g_e_1_1_app.md) & | [**Get**](#function-get) () <br>_This function returns a reference to the singleton instance of the_ [_**App**_](class_a_g_e_1_1_app.md) _class._ |


























## Detailed Description


This class represents the core of the AGE (Another Game Engine) framework, managing various aspects such as device management, layers, scripts, and assets. It also handles window events and manages the ImGui layer for user interface elements. 


    
## Public Functions Documentation




### function App 

```C++
AGE::App::App (
    const std::string & name="AGE App",
    ApplicationCommandLineArgs Args=ApplicationCommandLineArgs ()
) 
```



Constructor for the [**App**](class_a_g_e_1_1_app.md) class. Initializes an instance of the application with a name and command line arguments.




**Parameters:**


* `name` The name of the application. 
* `Args` Command line arguments provided when starting the application.



**Returns:**

None Constructor for the [**App**](class_a_g_e_1_1_app.md) class. Initializes an instance of the application with a name and command line arguments.




**Parameters:**


* `name` The name of the application. 
* `Args` Command line arguments provided when starting the application.



**Returns:**

None 





        

<hr>



### function Close 

_Closes the application by setting m\_Running to false._ 
```C++
void AGE::App::Close () 
```



This function sets the member variable m\_Running to false, effectively closing the application. It does not return anything and has no parameters.




**Returns:**

void


Closes the application by setting m\_Running to false.


This function sets the member variable m\_Running of an instance of the [**App**](class_a_g_e_1_1_app.md) class to false, effectively closing the application. It does not return any value and has no parameters.




**Returns:**

void 





        

<hr>



### function GetAppConfig 

_Returns the application configuration object._ 
```C++
inline AppConfig & AGE::App::GetAppConfig () 
```



This function returns a reference to the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object that holds all the configurations for the application. The returned object can be used to modify the application's settings.




**Returns:**

A reference to the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object.


Returns the application configuration object.


This function returns a reference to the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object that holds all of the configuration settings for the application. It is used by other parts of the application to access and modify these settings as needed.




**Returns:**

A reference to the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object. 





        

<hr>



### function GetCommandLineArgs 

_Retrieves the command line arguments of the application._ 
```C++
inline ApplicationCommandLineArgs AGE::App::GetCommandLineArgs () const
```





**Returns:**

An instance of [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) containing all the command line arguments.


Retrieves the command line arguments of the application. 

**Returns:**

An instance of [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) containing all the command line arguments. 





        

<hr>



### function GetDeviceManager 

_Returns a reference to the device manager instance._ 
```C++
inline DeviceManager & AGE::App::GetDeviceManager () 
```



This function returns a reference to the device manager instance that is currently in use by the application. The returned object can be used to interact with the hardware devices managed by the system.




**Returns:**

A reference to the [**DeviceManager**](class_a_g_e_1_1_device_manager.md) instance.


Returns a reference to the device manager instance.


This function returns a reference to the device manager instance that is currently in use by the application. The returned object can be used for various operations related to managing devices, such as initializing or shutting down devices.




**Returns:**

A reference to the [**DeviceManager**](class_a_g_e_1_1_device_manager.md) instance. 





        

<hr>



### function GetDirectXErrorMessages 

_This function retrieves DirectX error messages._ 
```C++
void AGE::App::GetDirectXErrorMessages () 
```



The function does not take any parameters and returns void. It is designed to handle the retrieval of error messages from the DirectX API, which can be useful for debugging purposes. However, it doesn't provide any specific information about the errors that might occur during its execution. For more detailed error handling, consider using other functions or classes provided by the DirectX SDK.




**Returns:**

void


This function retrieves DirectX error messages.


The function does not take any parameters and returns void. It is designed to handle the retrieval of error messages from the DirectX library, which can be useful for debugging purposes. However, it doesn't provide specific information about the errors that have occurred. For this, additional functions or methods might be needed.




**Returns:**

Void 





        

<hr>



### function GetFramebufferSize 

_Returns the framebuffer size of the application._ 
```C++
inline const Vector2 & AGE::App::GetFramebufferSize () 
```





**Returns:**

A constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the current framebuffer size.


Returns the framebuffer size of the application. 

**Returns:**

A constant reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the current framebuffer size. 





        

<hr>



### function GetImGuiLayer 

_This function returns the ImGui layer of the application._ 
```C++
inline ImGuiLayer * AGE::App::GetImGuiLayer () 
```





**Returns:**

Pointer to the [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) object if it exists, nullptr otherwise.


Returns the ImGui layer instance.


This function returns a pointer to the ImGui layer instance stored in this class. It is used for handling user interface events and rendering.




**Returns:**

Pointer to the [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) instance. 





        

<hr>



### function GetProject 

_Returns a reference to the_ [_**Project**_](class_a_g_e_1_1_project.md) _object._
```C++
inline Ref< Project > & AGE::App::GetProject () 
```



This function returns a reference to the [**Project**](class_a_g_e_1_1_project.md) object stored in the member variable 'm\_Project'. It allows for direct manipulation of this data if required.




**Returns:**

A reference to the [**Project**](class_a_g_e_1_1_project.md) object.


Returns a reference to the [**Project**](class_a_g_e_1_1_project.md) object.


This function returns a reference to the [**Project**](class_a_g_e_1_1_project.md) object stored in the class instance. It allows for direct manipulation of this data if necessary.




**Returns:**

A reference to the [**Project**](class_a_g_e_1_1_project.md) object. 





        

<hr>



### function GetTargetPlatform 

_This function returns the target platform._ 
```C++
inline uint16_t AGE::App::GetTargetPlatform () 
```





**Returns:**

uint16\_t The target platform as a uint16\_t value.


This function returns the target platform. 

**Returns:**

uint16\_t The target platform as a uint16\_t value. 





        

<hr>



### function Init 

_Initializes the application. This function sets up various components of the app such as device manager, asset manager and ImGui layer._ 
```C++
void AGE::App::Init () 
```



It creates a [**DeviceManager**](class_a_g_e_1_1_device_manager.md) instance with an AudioEngineType of AGESoundEngine. The event callback for this is set to [**App::OnEvent**](class_a_g_e_1_1_app.md#function-onevent).


In non-distribution builds, no further setup is performed. However, in distribution builds, it initializes the [**AssetManager**](class_a_g_e_1_1_asset_manager.md) and loads a .AGEpak file.


It then pushes an [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) onto the layer stack and attaches it to the NewProjectLayer if bShowNewProjectMenu is true. Finally, it sets m\_Running to true. 


        

<hr>



### function InitLayers 

_Initializes and attaches all layers in the layer stack._ 
```C++
void AGE::App::InitLayers () 
```



This function iterates over each layer in the m\_LayerStack, checks if its name is either "NewProjectLayer" or "ImGuiLayer", and skips these two special layers. For other layers, it calls their [**Init()**](class_a_g_e_1_1_app.md#function-init) method to initialize them and then OnAttach() to attach them. The variable bBlockThisFrame is also set to false at the end of this function.




**Returns:**

void


Initializes and attaches all layers in the layer stack.


This function iterates over each layer in the m\_LayerStack vector, checks if its name is either "NewProjectLayer" or "ImGuiLayer", and skips these two special layers. For other layers, it calls [**Init()**](class_a_g_e_1_1_app.md#function-init) to initialize them and OnAttach() to attach them to the application. It also sets bBlockThisFrame to false at the end of this function.




**Returns:**

void 





        

<hr>



### function InitRenderer 

_Initializes the renderer._ 
```C++
void AGE::App::InitRenderer () 
```



This function is used to initialize the [**Renderer**](class_a_g_e_1_1_renderer.md) by calling its Init method. It sets up any necessary resources for rendering, such as shaders and textures.




**Returns:**

void


Initializes the [**Renderer**](class_a_g_e_1_1_renderer.md) module.


This function is used to initialize the [**Renderer**](class_a_g_e_1_1_renderer.md) module by calling the [**Init()**](class_a_g_e_1_1_app.md#function-init) function from the [**Renderer**](class_a_g_e_1_1_renderer.md) class. It sets up any necessary resources for rendering, such as setting up OpenGL context or initializing shaders and textures.




**Returns:**

void 





        

<hr>



### function LoadAssets 

_Loads assets asynchronously in separate threads._ 
```C++
void AGE::App::LoadAssets () 
```



This function starts three additional threads to load scenes, sound banks and [**Aseprite**](class_a_g_e_1_1_aseprite.md) files respectively. After starting the threads, it detaches them so that they run independently of the main thread. Finally, it calls `LoadTextures` and `LoadShaders` functions to load textures and shaders.




**Returns:**

void


Loads assets in separate threads for concurrent loading.


This function starts three additional threads to load scenes, sound banks and [**Aseprite**](class_a_g_e_1_1_aseprite.md) files concurrently. It then detaches these threads so they run independently of the main thread. After that, it calls `LoadTextures` and `LoadShaders` functions to finish the asset loading process.




**Returns:**

void 





        

<hr>



### function OnEvent 

_Handles an event dispatched by the application._ 
```C++
void AGE::App::OnEvent (
    Event & E
) 
```



This function is responsible for dispatching events to all layers and components in the application. It uses an [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md) object to handle different types of events, such as [**WindowCloseEvent**](class_a_g_e_1_1_window_close_event.md), [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md), [**FramebufferResizeEvent**](class_a_g_e_1_1_framebuffer_resize_event.md), [**RendererChangeEvent**](class_a_g_e_1_1_renderer_change_event.md), [**ProjectCreatedEvent**](class_a_g_e_1_1_project_created_event.md), and [**ProjectLoadedEvent**](class_a_g_e_1_1_project_loaded_event.md).




**Parameters:**


* `E` Reference to the event that needs to be handled.

Handles an event dispatched by the application.


This function is responsible for dispatching events to all layers and components in the application's layer stack. It uses an [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md) object to handle different types of events such as [**WindowCloseEvent**](class_a_g_e_1_1_window_close_event.md), [**WindowResizeEvent**](class_a_g_e_1_1_window_resize_event.md), [**FramebufferResizeEvent**](class_a_g_e_1_1_framebuffer_resize_event.md), [**RendererChangeEvent**](class_a_g_e_1_1_renderer_change_event.md), [**ProjectCreatedEvent**](class_a_g_e_1_1_project_created_event.md), and [**ProjectLoadedEvent**](class_a_g_e_1_1_project_loaded_event.md). The function also checks for specific conditions like if the NewProjectLayer is shown or if event handling should be blocked in the current frame. It iterates over the layer stack from back to front and calls OnEvent on each layer until an event has been handled. Similarly, it does this for components as well. If an event gets handled during any of these iterations, the loop breaks early.




**Parameters:**


* `E` The event to be dispatched. 




        

<hr>



### function PushLayer 

_Pushes a layer onto the stack and attaches it._ 
```C++
void AGE::App::PushLayer (
    Layer * Layer
) 
```



This function pushes a given [**Layer**](class_a_g_e_1_1_layer.md) object onto the m\_LayerStack, which is essentially a stack of layers used in an application. The OnAttach() method for this layer will be called to initialize it. 

**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the [**Layer**](class_a_g_e_1_1_layer.md) that needs to be pushed and attached.

Pushes a layer onto the application's layer stack.


This function pushes a given [**Layer**](class_a_g_e_1_1_layer.md) object into the m\_LayerStack of the [**App**](class_a_g_e_1_1_app.md) class. The layer is added at the top of the stack, and will be processed last during rendering.




**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the [**Layer**](class_a_g_e_1_1_layer.md) object that needs to be pushed onto the stack. 




        

<hr>



### function PushOverlay 

_Pushes an overlay layer onto the stack and calls its OnAttach() function._ 
```C++
void AGE::App::PushOverlay (
    Layer * Layer
) 
```



This function pushes a given [**Layer**](class_a_g_e_1_1_layer.md) object into the m\_LayerStack, which is assumed to be of type [**LayerStack**](class_a_g_e_1_1_layer_stack.md). The [**Layer**](class_a_g_e_1_1_layer.md)'s OnAttach() function is then called.




**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the [**Layer**](class_a_g_e_1_1_layer.md) object that will be pushed onto the stack and its OnAttach() function will be called.

Pushes an overlay layer onto the stack and calls its OnAttach function.


This function pushes a given [**Layer**](class_a_g_e_1_1_layer.md) object into the m\_LayerStack, which is assumed to be of type [**LayerStack**](class_a_g_e_1_1_layer_stack.md). It then calls the OnAttach() function on this [**Layer**](class_a_g_e_1_1_layer.md) object. The AGE\_PROFILE\_FUNCTION macro is used for profiling purposes and should not affect the functionality of the application.




**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to a [**Layer**](class_a_g_e_1_1_layer.md) object that will be pushed onto the stack. 




        

<hr>



### function PushScriptableComp 

_Pushes a_ [_**ScriptableEntity**_](class_a_g_e_1_1_scriptable_entity.md) _component onto the stack._
```C++
void AGE::App::PushScriptableComp (
    ScriptableEntity * Comp
) 
```



This function pushes a given [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) component onto the m\_CompStack, which is likely to be a stack of components for some kind of scripting system or similar use case. The parameter Comp should be an instance of a class that inherits from the [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) base class.




**Parameters:**


* `Comp` Pointer to the [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) component to push onto the stack. 



**Returns:**

void No return value.


Pushes a [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) component onto the stack.


This function takes in a pointer to a [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) object and pushes it into the m\_CompStack, which is likely a stack of components for some kind of application.




**Parameters:**


* `Comp` A pointer to the [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) component that will be pushed onto the stack. 




        

<hr>



### function Run 

```C++
void AGE::App::Run () 
```




<hr>



### function SetProject 

_Sets the project object._ 
```C++
inline void AGE::App::SetProject (
    Ref< Project > Proj
) 
```



This function sets the value of the member variable 'm\_Project' to the input parameter 'Proj'. It takes a reference to a [**Project**](class_a_g_e_1_1_project.md) object and assigns it to 'm\_Project'.




**Parameters:**


* `Proj` A Ref&lt;Project&gt; object representing the new project.

Sets the project object.


This function sets the value of the member variable `m_Project` to the provided `Proj` parameter. The purpose of this function is to provide a way to update the current project object that's being used by other parts of the system.




**Parameters:**


* `Proj` A reference to the new [**Project**](class_a_g_e_1_1_project.md) object to be set. 




        

<hr>



### function SetTargetPlatform 

_Sets the target platform to a specified value._ 
```C++
inline void AGE::App::SetTargetPlatform (
    uint16_t Target
) 
```



This function sets the member variable `m_Target` of the class to a new value, which represents the target platform. The parameter `Target` is an unsigned 16-bit integer that specifies the new target platform.




**Parameters:**


* `Target` The new target platform as an unsigned 16-bit integer.

Sets the target platform to a given value.


This function sets the member variable `m_Target` to the provided uint16\_t parameter `Target`, which is cast to type `TargetPlatform` before assignment. The purpose of this function is to update the current target platform being targeted by the system.




**Parameters:**


* `Target` The new value for the target platform. This should be a valid enumerator of the `TargetPlatform` enum. 




        

<hr>



### function Shutdown 

_This function is used to shutdown the application. It sets a flag indicating that the program is no longer running, and then shuts down the renderer._ 
```C++
void AGE::App::Shutdown () 
```





**Parameters:**


* `None` 



**Returns:**

void


This function is used to shutdown the application. It sets a flag indicating that the program is no longer running, and then shuts down the renderer. 

**Returns:**

void 





        

<hr>



### function ~App 

_Destructor for the_ [_**App**_](class_a_g_e_1_1_app.md) _class._
```C++
virtual AGE::App::~App () 
```



This function is responsible for cleaning up any resources that were acquired during the lifetime of an instance of this class, such as memory or file handles. It calls the [**Shutdown()**](class_a_g_e_1_1_app.md#function-shutdown) method to perform these cleanups.


Destructor for the [**App**](class_a_g_e_1_1_app.md) class.


This function is responsible for cleaning up any resources that were acquired during the lifetime of an instance of this class. In this case, it calls the [**Shutdown()**](class_a_g_e_1_1_app.md#function-shutdown) method to ensure all system resources are properly released and cleaned up.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Get 

_This function returns a reference to the singleton instance of the_ [_**App**_](class_a_g_e_1_1_app.md) _class._
```C++
static inline App & AGE::App::Get () 
```





**Returns:**

A reference to the singleton instance of the [**App**](class_a_g_e_1_1_app.md) class.


This function returns a reference to the singleton instance of the [**App**](class_a_g_e_1_1_app.md) class. 

**Returns:**

A reference to the singleton instance of the [**App**](class_a_g_e_1_1_app.md) class. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/App.h`

