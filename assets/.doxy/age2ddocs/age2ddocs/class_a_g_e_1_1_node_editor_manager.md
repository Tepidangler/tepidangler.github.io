

# Class AGE::NodeEditorManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**CreateContextAndWindow**](#function-createcontextandwindow) (const std::filesystem::path & Filepath, const std::string & WindowName, void \* Target=nullptr) <br> |
|  void | [**DeregisterFunctions**](#function-deregisterfunctions) () <br> |
|   | [**NodeEditorManager**](#function-nodeeditormanager-13) () <br> |
|   | [**NodeEditorManager**](#function-nodeeditormanager-23) (const [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) &) = delete<br> |
|   | [**NodeEditorManager**](#function-nodeeditormanager-33) ([**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) &&) = delete<br> |
|  void | [**RegisterFunctions**](#function-registerfunctions) () <br> |
|  void | [**RenderWindows**](#function-renderwindows) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual  | [**~NodeEditorManager**](#function-nodeeditormanager) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetNewNodeID**](#function-getnewnodeid) () <br> |


























## Public Functions Documentation




### function CreateContextAndWindow 

```C++
void AGE::NodeEditorManager::CreateContextAndWindow (
    const std::filesystem::path & Filepath,
    const std::string & WindowName,
    void * Target=nullptr
) 
```




<hr>



### function DeregisterFunctions 

```C++
void AGE::NodeEditorManager::DeregisterFunctions () 
```




<hr>



### function NodeEditorManager [1/3]

```C++
AGE::NodeEditorManager::NodeEditorManager () 
```




<hr>



### function NodeEditorManager [2/3]

```C++
AGE::NodeEditorManager::NodeEditorManager (
    const NodeEditorManager &
) = delete
```




<hr>



### function NodeEditorManager [3/3]

```C++
AGE::NodeEditorManager::NodeEditorManager (
    NodeEditorManager &&
) = delete
```




<hr>



### function RegisterFunctions 

```C++
void AGE::NodeEditorManager::RegisterFunctions () 
```




<hr>



### function RenderWindows 

```C++
void AGE::NodeEditorManager::RenderWindows (
    TimeStep DeltaTime
) 
```




<hr>



### function ~NodeEditorManager 

```C++
virtual AGE::NodeEditorManager::~NodeEditorManager () 
```




<hr>
## Public Static Functions Documentation




### function GetNewNodeID 

```C++
static inline uint32_t AGE::NodeEditorManager::GetNewNodeID () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/NodeEditorManager.h`

