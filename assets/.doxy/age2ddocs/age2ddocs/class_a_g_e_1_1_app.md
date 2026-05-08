

# Class AGE::App



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**App**](class_a_g_e_1_1_app.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**App**](#function-app) (const std::string & name="AGE App", [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) Args=[**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md)()) <br> |
|  void | [**Close**](#function-close) () <br> |
|  [**AppConfig**](struct_a_g_e_1_1_app_config.md) & | [**GetAppConfig**](#function-getappconfig) () <br> |
|  [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md) | [**GetCommandLineArgs**](#function-getcommandlineargs) () const<br> |
|  [**DeviceManager**](class_a_g_e_1_1_device_manager.md) & | [**GetDeviceManager**](#function-getdevicemanager) () <br> |
|  void | [**GetDirectXErrorMessages**](#function-getdirectxerrormessages) () <br> |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) & | [**GetFramebufferSize**](#function-getframebuffersize) () <br> |
|  [**ImGuiLayer**](class_a_g_e_1_1_im_gui_layer.md) \* | [**GetImGuiLayer**](#function-getimguilayer) () <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; & | [**GetProject**](#function-getproject) () <br> |
|  uint16\_t | [**GetTargetPlatform**](#function-gettargetplatform) () <br> |
|  void | [**Init**](#function-init) () <br> |
|  void | [**InitLayers**](#function-initlayers) () <br> |
|  void | [**InitRenderer**](#function-initrenderer) () <br> |
|  void | [**LoadAssets**](#function-loadassets) () <br> |
|  void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
|  void | [**PushLayer**](#function-pushlayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br> |
|  void | [**PushOverlay**](#function-pushoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br> |
|  void | [**PushScriptableComp**](#function-pushscriptablecomp) ([**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* Comp) <br> |
|  void | [**Run**](#function-run) () <br> |
|  void | [**SetProject**](#function-setproject) (Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; Proj) <br> |
|  void | [**SetTargetPlatform**](#function-settargetplatform) (uint16\_t Target) <br> |
|  void | [**Shutdown**](#function-shutdown) () <br> |
| virtual  | [**~App**](#function-app) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**App**](class_a_g_e_1_1_app.md) & | [**Get**](#function-get) () <br> |


























## Public Functions Documentation




### function App 

```C++
AGE::App::App (
    const std::string & name="AGE App",
    ApplicationCommandLineArgs Args=ApplicationCommandLineArgs ()
) 
```




<hr>



### function Close 

```C++
void AGE::App::Close () 
```




<hr>



### function GetAppConfig 

```C++
inline AppConfig & AGE::App::GetAppConfig () 
```




<hr>



### function GetCommandLineArgs 

```C++
inline ApplicationCommandLineArgs AGE::App::GetCommandLineArgs () const
```




<hr>



### function GetDeviceManager 

```C++
inline DeviceManager & AGE::App::GetDeviceManager () 
```




<hr>



### function GetDirectXErrorMessages 

```C++
void AGE::App::GetDirectXErrorMessages () 
```




<hr>



### function GetFramebufferSize 

```C++
inline const Vector2 & AGE::App::GetFramebufferSize () 
```




<hr>



### function GetImGuiLayer 

```C++
inline ImGuiLayer * AGE::App::GetImGuiLayer () 
```




<hr>



### function GetProject 

```C++
inline Ref< Project > & AGE::App::GetProject () 
```




<hr>



### function GetTargetPlatform 

```C++
inline uint16_t AGE::App::GetTargetPlatform () 
```




<hr>



### function Init 

```C++
void AGE::App::Init () 
```




<hr>



### function InitLayers 

```C++
void AGE::App::InitLayers () 
```




<hr>



### function InitRenderer 

```C++
void AGE::App::InitRenderer () 
```




<hr>



### function LoadAssets 

```C++
void AGE::App::LoadAssets () 
```




<hr>



### function OnEvent 

```C++
void AGE::App::OnEvent (
    Event & E
) 
```




<hr>



### function PushLayer 

```C++
void AGE::App::PushLayer (
    Layer * Layer
) 
```




<hr>



### function PushOverlay 

```C++
void AGE::App::PushOverlay (
    Layer * Layer
) 
```




<hr>



### function PushScriptableComp 

```C++
void AGE::App::PushScriptableComp (
    ScriptableEntity * Comp
) 
```




<hr>



### function Run 

```C++
void AGE::App::Run () 
```




<hr>



### function SetProject 

```C++
inline void AGE::App::SetProject (
    Ref< Project > Proj
) 
```




<hr>



### function SetTargetPlatform 

```C++
inline void AGE::App::SetTargetPlatform (
    uint16_t Target
) 
```




<hr>



### function Shutdown 

```C++
void AGE::App::Shutdown () 
```




<hr>



### function ~App 

```C++
virtual AGE::App::~App () 
```




<hr>
## Public Static Functions Documentation




### function Get 

```C++
static inline App & AGE::App::Get () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/App.h`

