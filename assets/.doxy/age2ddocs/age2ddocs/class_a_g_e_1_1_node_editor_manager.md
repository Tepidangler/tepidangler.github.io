

# Class AGE::NodeEditorManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**CreateContextAndWindow**](#function-createcontextandwindow) (const std::filesystem::path & Filepath, const std::string & WindowName, void \* Target=nullptr) <br> |
|  void | [**DeregisterFunctions**](#function-deregisterfunctions) () <br>_Deregisters functions from all active windows._  |
|   | [**NodeEditorManager**](#function-nodeeditormanager-13) () <br> |
|   | [**NodeEditorManager**](#function-nodeeditormanager-23) (const [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) &) = delete<br>_Deleted copy constructor for the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _class to prevent copying._ |
|   | [**NodeEditorManager**](#function-nodeeditormanager-33) ([**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) &&) = delete<br>[_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _move constructor is deleted to prevent copying of the manager object._ |
|  void | [**RegisterFunctions**](#function-registerfunctions) () <br>_This function is used to register functions for all active windows in the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _. It iterates over each window (pair of a pointer to a Window and its name) in m\_ActiveWindows, and calls_[_**RegisterFunctions()**_](class_a_g_e_1_1_node_editor_manager.md#function-registerfunctions) _on the Window object pointed to by the first element of the pair._ |
|  void | [**RenderWindows**](#function-renderwindows) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_Render all active windows in the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _._ |
| virtual  | [**~NodeEditorManager**](#function-nodeeditormanager) () <br>_Destructor for_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _class. It iterates over all active windows and destroys each editor instance using ax::NodeEditor::DestroyEditor function._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetNewNodeID**](#function-getnewnodeid) () <br>_Generates a new unique node ID._  |


























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

_Deregisters functions from all active windows._ 
```C++
void AGE::NodeEditorManager::DeregisterFunctions () 
```



This function iterates over the list of active windows (m\_ActiveWindows) and calls the [**DeregisterFunctions()**](class_a_g_e_1_1_node_editor_manager.md#function-deregisterfunctions) method on each window's node editor. It is used to remove any registered functions that are no longer needed or relevant.




**Returns:**

void


Deregisters all functions from the active windows.


This function iterates over each active window and calls the `DeregisterFunctions` method on that window's node editor instance. It does not return anything, so it has a void return type. 


        

<hr>



### function NodeEditorManager [1/3]

```C++
AGE::NodeEditorManager::NodeEditorManager () 
```




<hr>



### function NodeEditorManager [2/3]

_Deleted copy constructor for the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _class to prevent copying._
```C++
AGE::NodeEditorManager::NodeEditorManager (
    const NodeEditorManager &
) = delete
```



This function is marked as deleted because we do not want any copies of this object. It's a good practice in C++ to avoid unnecessary copying and wasting memory resources, especially when dealing with complex objects like this one.




**Parameters:**


* `other` The [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) instance to be copied. This parameter is ignored as the copy constructor is marked as deleted.



**Returns:**

Nothing. As a result of being marked as deleted, attempting to use it will lead to a compile-time error.


Deleted copy constructor for the [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) class to prevent copying.


This function is marked as deleted because we do not want any copies of this object. It's a good practice to avoid unnecessary copying and duplication in our code, which can lead to performance issues or memory leaks.




**Parameters:**


* `other` The [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) instance to be copied. This parameter is not used as the copy constructor is marked as deleted.



**Returns:**

Nothing as this function does not return any value. 





        

<hr>



### function NodeEditorManager [3/3]

[_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _move constructor is deleted to prevent copying of the manager object._
```C++
AGE::NodeEditorManager::NodeEditorManager (
    NodeEditorManager &&
) = delete
```



This function is marked as deleted because we do not want to allow copying of the [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) object. We only allow moving semantics, which means transferring ownership of resources from one object to another.




**Returns:**

The move constructor does not return anything since it's a deleted function.


[**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) move constructor is deleted to prevent copying of the manager object.


This function is marked as deleted because we do not want to allow copying of this class's objects. We only allow moving semantics, which means transferring ownership of resources from one object to another.




**Returns:**

The move constructor does not return anything. It simply takes the resources from an existing object and moves them into a new one. 





        

<hr>



### function RegisterFunctions 

_This function is used to register functions for all active windows in the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _. It iterates over each window (pair of a pointer to a Window and its name) in m\_ActiveWindows, and calls_[_**RegisterFunctions()**_](class_a_g_e_1_1_node_editor_manager.md#function-registerfunctions) _on the Window object pointed to by the first element of the pair._
```C++
void AGE::NodeEditorManager::RegisterFunctions () 
```





**Returns:**

void


This function registers functions for all active windows in the [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md).


The function iterates over each window (pair of a pointer to a Window and its name) stored in m\_ActiveWindows, and calls the [**RegisterFunctions()**](class_a_g_e_1_1_node_editor_manager.md#function-registerfunctions) method on that window's node editor. It does not return anything.




**Returns:**

void 





        

<hr>



### function RenderWindows 

_Render all active windows in the_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _._
```C++
void AGE::NodeEditorManager::RenderWindows (
    TimeStep DeltaTime
) 
```



This function iterates over all active windows and calls their OnImGuiRender method, passing in the provided [**TimeStep**](class_a_g_e_1_1_time_step.md) value. It is used to update and render each window during the main application loop.




**Parameters:**


* `DeltaTime` The time step for rendering and updating the windows.

Renders all active windows in the [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md).


This function iterates over each window stored in m\_ActiveWindows and calls OnImGuiRender on it, passing DeltaTime as an argument. It is used to update and render all GUI elements associated with the windows.




**Parameters:**


* `DeltaTime` The time step for rendering. 




        

<hr>



### function ~NodeEditorManager 

_Destructor for_ [_**NodeEditorManager**_](class_a_g_e_1_1_node_editor_manager.md) _class. It iterates over all active windows and destroys each editor instance using ax::NodeEditor::DestroyEditor function._
```C++
virtual AGE::NodeEditorManager::~NodeEditorManager () 
```





**Returns:**

None


Destructor for [**NodeEditorManager**](class_a_g_e_1_1_node_editor_manager.md) class. It iterates over all active windows and destroys each editor instance using ax::NodeEditor::DestroyEditor function.




**Returns:**

None 





        

<hr>
## Public Static Functions Documentation




### function GetNewNodeID 

_Generates a new unique node ID._ 
```C++
static inline uint32_t AGE::NodeEditorManager::GetNewNodeID () 
```



This function increments the global NodeID variable and returns it, effectively generating a new unique identifier for each call.




**Returns:**

The newly generated node ID as a uint32\_t.


Generates a new unique node ID for use in the system.


This function increments the static variable NodeID and returns its value, effectively generating a new unique ID each time it is called.




**Returns:**

The newly generated node ID as a uint32\_t. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/NodeEditorManager.h`

