

# Class AGE::NodeEditorWindow



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md)








Inherits the following classes: [AGE::Layer](class_a_g_e_1_1_layer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetWindowName**](#function-getwindowname) () const<br>_Returns the name of the window._  |
|   | [**NodeEditorWindow**](#function-nodeeditorwindow) (const std::string & WindowName, ax::NodeEditor::EditorContext \* Context, void \* Target=nullptr, bool LoadingExisting=false) <br> |
| virtual void | [**OnAttach**](#function-onattach) () <br>_This function is called when the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _is attached to the application. It sets up various aspects of the editor, such as setting the current editor context and positioning nodes._ |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is responsible for rendering the ImGui interface in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._ |
| virtual  | [**~NodeEditorWindow**](#function-nodeeditorwindow) () <br>_Destructor for the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _class._ |


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


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) & Data) <br>_This function serializes the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |














## Protected Attributes inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](class_a_g_e_1_1_layer.md#variable-m_debugname)  <br> |






























## Protected Functions

| Type | Name |
| ---: | :--- |
|  void | [**BuildNode**](#function-buildnode) (Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; Node) <br>_This function builds a node by setting its inputs and outputs._  |
|  void | [**BuildNodes**](#function-buildnodes) () <br>_This function builds all the nodes in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _. It iterates over each node (_`m_Nodes` _) and calls_`BuildNode()` _on it. The purpose of this function is to update or rebuild all nodes in the window, ensuring they are up-to-date with any changes made elsewhere in the program._ |
|  bool | [**CanCreateLink**](#function-cancreatelink) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; A, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; B) <br>_Checks if a link can be created between two pins._  |
|  void | [**CompileGraph**](#function-compilegraph) () <br>_Compiles the graph and saves it if successful._  |
|  void | [**DeleteNode**](#function-deletenode) () <br> |
|  void | [**DeregisterFunctions**](#function-deregisterfunctions) () <br>_Deregisters all functions from the target node._  |
|  void | [**DrawAndCreateNewLink**](#function-drawandcreatenewlink) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, std::function&lt; void(const char \*, ImColor)&gt; ShowLabelFunction) <br>_Draws and creates a new link between two pins._  |
|  void | [**DrawAndCreateNewNode**](#function-drawandcreatenewnode) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newNodeLinkPin, bool createNewNode, std::function&lt; void(const char \*, ImColor)&gt; ShowLabelFunction) <br>_Draws and creates a new node in the Node Editor Window._  |
|  void | [**DrawHeader**](#function-drawheader) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, bool IsSimple, bool HasOutputCallbacks) <br> |
|  void | [**DrawInputPins**](#function-drawinputpins) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin) <br> |
|  void | [**DrawNodes**](#function-drawnodes) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin) <br> |
|  void | [**DrawOutputPins**](#function-drawoutputpins) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, bool IsSimple) <br> |
|  void | [**DrawPinIcon**](#function-drawpinicon) (const Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & Pin, bool Connected, int Alpha) <br> |
|  Ref&lt; [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) &gt; | [**FindLink**](#function-findlink-12) (ax::NodeEditor::LinkId ID) <br>_Finds a link with the given ID in the node editor window._  |
|  Ref&lt; [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) &gt; | [**FindLink**](#function-findlink-22) (ax::NodeEditor::PinId ID) <br>_Finds a link with the given start pin id._  |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**FindNode**](#function-findnode) (ax::NodeEditor::NodeId ID) <br>_Finds a node with the given ID in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._ |
|  Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; | [**FindPin**](#function-findpin) (ax::NodeEditor::PinId ID) <br>_Finds a pin with the given ID in the node editor._  |
|  ImColor | [**GetIconColor**](#function-geticoncolor) (AGEPinType Type) <br> |
|  uint32\_t | [**GetNextID**](#function-getnextid) () <br>_This function returns the next available ID for a new node._  |
|  ax::NodeEditor::LinkId | [**GetNextLinkID**](#function-getnextlinkid) () <br>_Generates the next available Link ID._  |
|  float | [**GetTouchProgress**](#function-gettouchprogress) (ax::NodeEditor::NodeId ID) <br>_Get the touch progress of a node with given ID._  |
|  ImRect | [**ImGui\_GetItemRect**](#function-imgui_getitemrect) () <br>_This function returns an_ `ImRect` _object that represents the rectangle of the current item._ |
|  ImRect | [**ImRect\_Expanded**](#function-imrect_expanded) (const ImRect & Rect, float x, float y) <br>_Expands an ImRect by a given amount in both dimensions._  |
|  bool | [**IsPinLinked**](#function-ispinlinked) (ax::NodeEditor::PinId ID) <br>_Checks if a pin is linked._  |
|  void | [**RebuildWindow**](#function-rebuildwindow) () <br>_This function is used to rebuild the window. It sets m\_IsOpen to true, indicating that the window should be rebuilt._  |
|  void | [**RegisterFunctions**](#function-registerfunctions) () <br> |
|  void | [**RenderWindow**](#function-renderwindow) (bool \* Opened, [**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**SaveGraph**](#function-savegraph) () <br>_Saves the graph to a file in the game content directory._  |
|  void | [**ShowDetailPanel**](#function-showdetailpanel) (bool \* ShowPanel=nullptr) <br>_This function is used to display the detail panel for a given target. The detail panel shows stats and properties of the entity._  |
|  void | [**ShowLeftPane**](#function-showleftpane) (float PanelWidth) <br> |
|  void | [**ShowNodeOptions**](#function-shownodeoptions) (Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node) <br>_Displays a menu with various options for creating and assigning nodes._  |
|  void | [**ShowStyleEditor**](#function-showstyleeditor) (bool \* Show=nullptr) <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnAppendString**](#function-spawnappendstring) () <br>_Spawns a new node with the type "Append String" and adds it to the nodes list. The function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _, sets its properties, and then calls_[_**BuildNode()**_](class_a_g_e_1_1_node_editor_window.md#function-buildnode) _on this newly created object. It also emplaces two input pins (one for each string) and one output pin into the node's Inputs and Outputs vectors respectively._ |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnBeginPlayNode**](#function-spawnbeginplaynode) () <br>_Spawns a new Begin Play node and adds it to the nodes list._  |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCosine**](#function-spawncosine) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCrossProduct**](#function-spawncrossproduct) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCubeRoot**](#function-spawncuberoot) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnDivide**](#function-spawndivide) () <br>_SpawnDivide creates a new divide node in the graph and adds it to the nodes list._  _\* The function creates an_[_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with two float inputs and one output, sets its type as Simple,_ _\* builds the node, assigns a reference to itself for use in the execution context,_ _\* and finally returns the newly created node._ _\*._ |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnDotProduct**](#function-spawndotproduct) () <br>_Spawns a new node representing the dot product operation in the graph. The function creates an_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties and adds it to the nodes list of the_[_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _instance. It also sets up the inputs, outputs, and utilities for this particular node._ |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnEqualToNode**](#function-spawnequaltonode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGTETNode**](#function-spawngtetnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetActor**](#function-spawngetactor) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetLocation2D**](#function-spawngetlocation2d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetLocation3D**](#function-spawngetlocation3d) () <br>_Spawns a new Get Location 3D node in the Node Editor Window. This function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties and configurations, such as name, color, type, inputs, outputs, etc. It also sets up the function details for this node including reference to itself, ID of its object, value of the function, entity pointer and its ID._ |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGreaterThanNode**](#function-spawngreaterthannode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnLTETNode**](#function-spawnltetnode) () <br>_Spawns a Less Than or Equal To (&lt;=) node with two float inputs and one boolean output._  |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnLessThanNode**](#function-spawnlessthannode) () <br>_Spawns a less than node in the graph._  |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnMakeLiteralString**](#function-spawnmakeliteralstring) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnModulo**](#function-spawnmodulo) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnMultiply**](#function-spawnmultiply) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnOnUpdateNode**](#function-spawnonupdatenode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnOutputActionNode**](#function-spawnoutputactionnode) () <br>_Spawns an output action node with two outputs - "Condition" and "Event". The first output is of type Float, the second is of type Boolean._  |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnPow**](#function-spawnpow) () <br>_Spawns a new_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with type 'Pow'._ |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnPrintStringNode**](#function-spawnprintstringnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSetLocation2D**](#function-spawnsetlocation2d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSetLocation3D**](#function-spawnsetlocation3d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSine**](#function-spawnsine) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSquareRoot**](#function-spawnsquareroot) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSubtract**](#function-spawnsubtract) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSum**](#function-spawnsum) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnToString**](#function-spawntostring) () <br>_Spawns a new node of type "To String" and adds it to the nodes list. The function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties, such as name, color, input pin type, output pin type etc., then builds the node using_[_**BuildNode()**_](class_a_g_e_1_1_node_editor_window.md#function-buildnode) _method. It also sets some additional properties for the created node like reference, ID, value, entity, and whether it is a utility function or not._ |
|  void | [**SyncLinks**](#function-synclinks) () <br>_Synchronizes the links between nodes._  |
|  void | [**TouchNode**](#function-touchnode) (ax::NodeEditor::NodeId ID) <br>_This function is used to update the touch time for a specific node._  |
|  void | [**UpdateTouch**](#function-updatetouch) (float DeltaTime) <br>_This function updates the touch time for each node in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._ |




## Protected Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**Splitter**](#function-splitter) (bool SplitVertically, float Thickness, float \* Size1, float \* Size2, float Min\_Size1, float Min\_Size2, float SplitterLongAxisSize=-1.f) <br>_Handles the behavior of a splitter in an ImGui context._  |




## Public Functions Documentation




### function GetWindowName 

_Returns the name of the window._ 
```C++
inline const std::string & AGE::NodeEditorWindow::GetWindowName () const
```





**Returns:**

A constant reference to a string containing the name of the window.


Returns the name of the window. 

**Returns:**

A constant reference to a string containing the window's name. 





        

<hr>



### function NodeEditorWindow 

```C++
AGE::NodeEditorWindow::NodeEditorWindow (
    const std::string & WindowName,
    ax::NodeEditor::EditorContext * Context,
    void * Target=nullptr,
    bool LoadingExisting=false
) 
```




<hr>



### function OnAttach 

_This function is called when the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _is attached to the application. It sets up various aspects of the editor, such as setting the current editor context and positioning nodes._
```C++
virtual void AGE::NodeEditorWindow::OnAttach () 
```





**Parameters:**


* `None` 



**Returns:**

void 





        
Implements [*AGE::Layer::OnAttach*](class_a_g_e_1_1_layer.md#function-onattach)


<hr>



### function OnImGuiRender 

_This function is responsible for rendering the ImGui interface in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._
```C++
virtual void AGE::NodeEditorWindow::OnImGuiRender (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The time step representing the elapsed time since the last frame.



**Returns:**

void 





        
Implements [*AGE::Layer::OnImGuiRender*](class_a_g_e_1_1_layer.md#function-onimguirender)


<hr>



### function ~NodeEditorWindow 

_Destructor for the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _class._
```C++
virtual AGE::NodeEditorWindow::~NodeEditorWindow () 
```



This function is responsible for cleaning up any resources that were allocated during the lifetime of this object, such as memory or file handles. It's important to ensure that all resources are properly released when an object is destroyed to prevent memory leaks and other issues. 


        

<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::NodeEditorWindow::Deserialize (
    DataReader * Serializer,
    NodeEditorWindow & Data
) 
```




<hr>



### function Serialize 

_This function serializes the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::NodeEditorWindow::Serialize (
    DataWriter * Serializer,
    const NodeEditorWindow & Data
) 
```



The function takes in a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) and a constant reference to a [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md). It writes out various properties of the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md), including its name, ID, nodes, links, and whether it shows ordinals or not.




**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be used for serialization. 
* `Data` The constant reference to the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) whose data is being serialized.



**Returns:**

void


This function serializes the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) data into a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object.




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the serialized data will be written. 
* `Data` Const reference to the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) whose data is being serialized.



**Returns:**

None 





        

<hr>
## Protected Functions Documentation




### function BuildNode 

_This function builds a node by setting its inputs and outputs._ 
```C++
void AGE::NodeEditorWindow::BuildNode (
    Ref< AGENode > Node
) 
```





**Parameters:**


* `Node` The node to be built. It is expected that this node has been initialized with at least some input and output pins. 




        

<hr>



### function BuildNodes 

_This function builds all the nodes in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _. It iterates over each node (_`m_Nodes` _) and calls_`BuildNode()` _on it. The purpose of this function is to update or rebuild all nodes in the window, ensuring they are up-to-date with any changes made elsewhere in the program._
```C++
void AGE::NodeEditorWindow::BuildNodes () 
```





**Returns:**

void 





        

<hr>



### function CanCreateLink 

_Checks if a link can be created between two pins._ 
```C++
bool AGE::NodeEditorWindow::CanCreateLink (
    Ref< AGEPin > A,
    Ref< AGEPin > B
) 
```



This function checks whether it is possible to create a link between two pins, A and B. It considers several factors such as the existence of the pins, their equality, the kind of each pin, and the type of each pin. Additionally, it also takes into account certain special cases where one pin's type can be any of 'Flow' or 'Callback'.




**Parameters:**


* `A` The first pin to consider for creating a link. 
* `B` The second pin to consider for creating a link. 



**Returns:**

True if a link can be created, false otherwise. 





        

<hr>



### function CompileGraph 

_Compiles the graph and saves it if successful._ 
```C++
void AGE::NodeEditorWindow::CompileGraph () 
```



This function compiles all nodes in the graph, sets their arguments, checks for any errors during compilation, syncs links, and finally saves the graph to a file if everything was successful. It also logs an info message with the name of the saved graph and its path if the compilation is successful or an error message otherwise. 


        

<hr>



### function DeleteNode 

```C++
void AGE::NodeEditorWindow::DeleteNode () 
```




<hr>



### function DeregisterFunctions 

_Deregisters all functions from the target node._ 
```C++
void AGE::NodeEditorWindow::DeregisterFunctions () 
```



This function is used to remove all registered functions from the target node. It calls the ClearFunctions() method on the m\_Target object, which presumably clears any previously registered functions.




**Returns:**

void 





        

<hr>



### function DrawAndCreateNewLink 

_Draws and creates a new link between two pins._ 
```C++
void AGE::NodeEditorWindow::DrawAndCreateNewLink (
    Ref< AGEPin > & newLinkPin,
    std::function< void(const char *, ImColor)> ShowLabelFunction
) 
```





**Parameters:**


* `newLinkPin` The newly created link pin. 
* `ShowLabelFunction` A function to show labels with different colors. 




        

<hr>



### function DrawAndCreateNewNode 

_Draws and creates a new node in the Node Editor Window._ 
```C++
void AGE::NodeEditorWindow::DrawAndCreateNewNode (
    Ref< AGEPin > & newLinkPin,
    Ref< AGEPin > & newNodeLinkPin,
    bool createNewNode,
    std::function< void(const char *, ImColor)> ShowLabelFunction
) 
```



This function handles user interactions related to creating or drawing nodes within the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md). It takes references to [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) objects, a boolean indicating whether a new node should be created, and a ShowLabelFunction that displays labels on the UI. 


        

<hr>



### function DrawHeader 

```C++
void AGE::NodeEditorWindow::DrawHeader (
    ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder,
    Ref< AGENode > & Node,
    Ref< AGEPin > & newLinkPin,
    bool IsSimple,
    bool HasOutputCallbacks
) 
```




<hr>



### function DrawInputPins 

```C++
void AGE::NodeEditorWindow::DrawInputPins (
    ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder,
    Ref< AGENode > & Node,
    Ref< AGEPin > & newLinkPin
) 
```




<hr>



### function DrawNodes 

```C++
void AGE::NodeEditorWindow::DrawNodes (
    Ref< AGEPin > & newLinkPin
) 
```




<hr>



### function DrawOutputPins 

```C++
void AGE::NodeEditorWindow::DrawOutputPins (
    ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder,
    Ref< AGENode > & Node,
    Ref< AGEPin > & newLinkPin,
    bool IsSimple
) 
```




<hr>



### function DrawPinIcon 

```C++
void AGE::NodeEditorWindow::DrawPinIcon (
    const Ref< AGEPin > & Pin,
    bool Connected,
    int Alpha
) 
```




<hr>



### function FindLink [1/2]

_Finds a link with the given ID in the node editor window._ 
```C++
Ref< AGENodeLink > AGE::NodeEditorWindow::FindLink (
    ax::NodeEditor::LinkId ID
) 
```



This function iterates over all links in the m\_Links vector and returns the first one that has an ID matching the input parameter 'ID'. If no such link is found, it returns an empty Ref object.




**Parameters:**


* `ID` The ID of the link to be found. 



**Returns:**

A reference to the found link or an empty Ref object if no such link exists. 





        

<hr>



### function FindLink [2/2]

_Finds a link with the given start pin id._ 
```C++
Ref< AGENodeLink > AGE::NodeEditorWindow::FindLink (
    ax::NodeEditor::PinId ID
) 
```



This function iterates over all links in the node editor window and returns the first one that has the same start pin id as the input parameter ID. If no such link is found, an empty reference to [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) is returned.




**Parameters:**


* `ID` The id of the start pin to search for. 



**Returns:**

A reference to the found link or an empty reference if no matching link was found. 





        

<hr>



### function FindNode 

_Finds a node with the given ID in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._
```C++
Ref< AGENode > AGE::NodeEditorWindow::FindNode (
    ax::NodeEditor::NodeId ID
) 
```



This function iterates over all nodes in the m\_Nodes vector and checks if their ID matches the input ID. If it does, that node is returned. If no matching node is found, an empty Ref&lt;AGENode&gt; object is returned.




**Parameters:**


* `ID` The ID of the node to be searched for. 



**Returns:**

A reference to the node with the given ID if one exists, otherwise returns an empty Ref&lt;AGENode&gt; object. 





        

<hr>



### function FindPin 

_Finds a pin with the given ID in the node editor._ 
```C++
Ref< AGEPin > AGE::NodeEditorWindow::FindPin (
    ax::NodeEditor::PinId ID
) 
```



This function iterates over all nodes and their inputs/outputs to find a pin that matches the provided ID. If no such pin is found, an empty reference (Ref&lt;AGEPin&gt;()) is returned. 

**Parameters:**


* `ID` The ID of the pin to be found. 



**Returns:**

A reference to the found pin or an empty reference if no matching pin was found. 





        

<hr>



### function GetIconColor 

```C++
ImColor AGE::NodeEditorWindow::GetIconColor (
    AGEPinType Type
) 
```




<hr>



### function GetNextID 

_This function returns the next available ID for a new node._ 
```C++
uint32_t AGE::NodeEditorWindow::GetNextID () 
```





**Returns:**

The unique identifier for the next node. 





        

<hr>



### function GetNextLinkID 

_Generates the next available Link ID._ 
```C++
ax::NodeEditor::LinkId AGE::NodeEditorWindow::GetNextLinkID () 
```



This function generates a unique Link ID for use in the Node Editor system. It uses the [**GetNextID()**](class_a_g_e_1_1_node_editor_window.md#function-getnextid) function to generate an integer, which is then converted into a LinkId object. The generated Link Id can be used to identify and manipulate links within the Node Editor system.




**Returns:**

ax::NodeEditor::LinkId - A unique identifier for a link in the Node Editor system. 





        

<hr>



### function GetTouchProgress 

_Get the touch progress of a node with given ID._ 
```C++
float AGE::NodeEditorWindow::GetTouchProgress (
    ax::NodeEditor::NodeId ID
) 
```



This function returns the touch progress for a specific node identified by its ID. The touch progress is calculated as the time elapsed since the last touch divided by the total touch time. If no touch data exists or if the touch time is zero, it will return 0.0f.




**Parameters:**


* `ID` The unique identifier of the node 



**Returns:**

float The touch progress in range [0.0, 1.0] 





        

<hr>



### function ImGui\_GetItemRect 

_This function returns an_ `ImRect` _object that represents the rectangle of the current item._
```C++
ImRect AGE::NodeEditorWindow::ImGui_GetItemRect () 
```



The returned `ImRect` is created using the minimum and maximum coordinates of the current item as obtained by calling `ImGui::GetItemRectMin()` and `ImGui::GetItemRectMax()` respectively.




**Returns:**

ImRect An object representing the rectangle of the current item. 





        

<hr>



### function ImRect\_Expanded 

_Expands an ImRect by a given amount in both dimensions._ 
```C++
ImRect AGE::NodeEditorWindow::ImRect_Expanded (
    const ImRect & Rect,
    float x,
    float y
) 
```



This function takes an existing ImRect and expands it by the specified amounts in both x and y directions. The resulting rectangle will have its minimum corner moved to the left and up, and its maximum corner moved to the right and down.




**Parameters:**


* `Rect` The original ImRect to be expanded. 
* `x` The amount to expand in the x direction (left/right). 
* `y` The amount to expand in the y direction (up/down).



**Returns:**

An ImRect that is expanded by the given amounts in both dimensions. 





        

<hr>



### function IsPinLinked 

_Checks if a pin is linked._ 
```C++
bool AGE::NodeEditorWindow::IsPinLinked (
    ax::NodeEditor::PinId ID
) 
```



This function checks whether the given PinId (ID) is linked to any other pins in the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md). It does this by iterating over all links in m\_Links and checking if either the StartPinID or EndPinID of each link equals the provided ID. If a match is found, it returns true indicating that the pin is linked. Otherwise, it returns false.




**Parameters:**


* `ID` The PinId to check for linking status.



**Returns:**

True if the pin is linked (i.e., connected to another pin), False otherwise. 





        

<hr>



### function RebuildWindow 

_This function is used to rebuild the window. It sets m\_IsOpen to true, indicating that the window should be rebuilt._ 
```C++
void AGE::NodeEditorWindow::RebuildWindow () 
```





**Returns:**

void 





        

<hr>



### function RegisterFunctions 

```C++
void AGE::NodeEditorWindow::RegisterFunctions () 
```




<hr>



### function RenderWindow 

```C++
void AGE::NodeEditorWindow::RenderWindow (
    bool * Opened,
    TimeStep DeltaTime
) 
```




<hr>



### function SaveGraph 

_Saves the graph to a file in the game content directory._ 
```C++
void AGE::NodeEditorWindow::SaveGraph () 
```



This function retrieves the application configuration and uses it to generate the path for saving the graph. The graph itself is written using a [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md), which writes an object of type [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) to the specified file path.




**Returns:**

void 





        

<hr>



### function ShowDetailPanel 

_This function is used to display the detail panel for a given target. The detail panel shows stats and properties of the entity._ 
```C++
void AGE::NodeEditorWindow::ShowDetailPanel (
    bool * ShowPanel=nullptr
) 
```





**Parameters:**


* `ShowPanel` A boolean pointer that indicates whether the detail panel should be shown or not. 




        

<hr>



### function ShowLeftPane 

```C++
void AGE::NodeEditorWindow::ShowLeftPane (
    float PanelWidth
) 
```




<hr>



### function ShowNodeOptions 

_Displays a menu with various options for creating and assigning nodes._ 
```C++
void AGE::NodeEditorWindow::ShowNodeOptions (
    Ref< AGENode > & Node
) 
```



Depending on the user's selection, different types of nodes are created using Spawn\*Node() functions (where '\*' can be any node type) and assigned to the input parameter 'Node'.




**Parameters:**


* `Node` A reference to an [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) object that will be modified by this function. The type of node created depends on which ImGui::MenuItem is selected. 




        

<hr>



### function ShowStyleEditor 

```C++
void AGE::NodeEditorWindow::ShowStyleEditor (
    bool * Show=nullptr
) 
```




<hr>



### function SpawnAppendString 

_Spawns a new node with the type "Append String" and adds it to the nodes list. The function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _, sets its properties, and then calls_[_**BuildNode()**_](class_a_g_e_1_1_node_editor_window.md#function-buildnode) _on this newly created object. It also emplaces two input pins (one for each string) and one output pin into the node's Inputs and Outputs vectors respectively._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnAppendString () 
```





**Returns:**

A reference to the new append string node. 





        

<hr>



### function SpawnBeginPlayNode 

_Spawns a new Begin Play node and adds it to the nodes list._ 
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnBeginPlayNode () 
```



This function creates a new instance of [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with specific attributes, such as name ("Begin Play"), color (ImColor(255,128,128)), and pin type (AGEPinType::Flow). It then adds this node to the m\_Nodes list. The function returns a reference to the newly created node.




**Returns:**

Ref&lt;AGENode&gt; A reference to the newly spawned Begin Play node. 





        

<hr>



### function SpawnCosine 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnCosine () 
```




<hr>



### function SpawnCrossProduct 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnCrossProduct () 
```




<hr>



### function SpawnCubeRoot 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnCubeRoot () 
```




<hr>



### function SpawnDivide 

_SpawnDivide creates a new divide node in the graph and adds it to the nodes list._  _\* The function creates an_[_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with two float inputs and one output, sets its type as Simple,_ _\* builds the node, assigns a reference to itself for use in the execution context,_ _\* and finally returns the newly created node._ _\*._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnDivide () 
```




 \* 

**Returns:**

Ref&lt;AGENode&gt; A reference to the newly spawned divide node.
 





        

<hr>



### function SpawnDotProduct 

_Spawns a new node representing the dot product operation in the graph. The function creates an_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties and adds it to the nodes list of the_[_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _instance. It also sets up the inputs, outputs, and utilities for this particular node._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnDotProduct () 
```





**Returns:**

A reference to the newly created [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md). 





        

<hr>



### function SpawnEqualToNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnEqualToNode () 
```




<hr>



### function SpawnGTETNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGTETNode () 
```




<hr>



### function SpawnGetActor 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGetActor () 
```




<hr>



### function SpawnGetLocation2D 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGetLocation2D () 
```




<hr>



### function SpawnGetLocation3D 

_Spawns a new Get Location 3D node in the Node Editor Window. This function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties and configurations, such as name, color, type, inputs, outputs, etc. It also sets up the function details for this node including reference to itself, ID of its object, value of the function, entity pointer and its ID._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGetLocation3D () 
```





**Returns:**

A Ref&lt;AGENode&gt; instance representing the newly created Get Location 3D node. 





        

<hr>



### function SpawnGreaterThanNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGreaterThanNode () 
```




<hr>



### function SpawnLTETNode 

_Spawns a Less Than or Equal To (&lt;=) node with two float inputs and one boolean output._ 
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnLTETNode () 
```



This function creates an [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) of type Simple, with two input pins of type Float and one output pin of type Boolean. The node's ID is set to the next available ID, its label is set to "&lt;=", and its color is set to a light blue (128, 195, 248). It also sets up the function details for this node: it references itself, stores the reference ID as the node's ID, sets the value string to "Less Than or Equal To", and sets the entity handle to null. The bIsUtilFunction flag is set to true. Finally, it calls BuildNode with the newly created node as an argument.




**Returns:**

Ref&lt;AGENode&gt; A reference to the newly spawned Less Than or Equal To (&lt;=) node. 





        

<hr>



### function SpawnLessThanNode 

_Spawns a less than node in the graph._ 
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnLessThanNode () 
```



This function creates a new [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with two input pins of type float and one output pin of type boolean, representing a simple comparison operation (less than). The node is then added to the m\_Nodes vector.




**Returns:**

Ref&lt;AGENode&gt; A reference to the newly created less than node. 





        

<hr>



### function SpawnMakeLiteralString 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnMakeLiteralString () 
```




<hr>



### function SpawnModulo 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnModulo () 
```




<hr>



### function SpawnMultiply 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnMultiply () 
```




<hr>



### function SpawnOnUpdateNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnOnUpdateNode () 
```




<hr>



### function SpawnOutputActionNode 

_Spawns an output action node with two outputs - "Condition" and "Event". The first output is of type Float, the second is of type Boolean._ 
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnOutputActionNode () 
```





**Returns:**

A reference to the newly created [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) object. 





        

<hr>



### function SpawnPow 

_Spawns a new_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with type 'Pow'._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnPow () 
```



This function creates a new [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) of type 'Pow' with two input pins and one output pin, all of which are of Float type. It also sets up the necessary properties for this node to be used as an util function.




**Returns:**

Ref&lt;AGENode&gt; A reference to the newly created Pow [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md). 





        

<hr>



### function SpawnPrintStringNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnPrintStringNode () 
```




<hr>



### function SpawnSetLocation2D 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSetLocation2D () 
```




<hr>



### function SpawnSetLocation3D 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSetLocation3D () 
```




<hr>



### function SpawnSine 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSine () 
```




<hr>



### function SpawnSquareRoot 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSquareRoot () 
```




<hr>



### function SpawnSubtract 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSubtract () 
```




<hr>



### function SpawnSum 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnSum () 
```




<hr>



### function SpawnToString 

_Spawns a new node of type "To String" and adds it to the nodes list. The function creates an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with specific properties, such as name, color, input pin type, output pin type etc., then builds the node using_[_**BuildNode()**_](class_a_g_e_1_1_node_editor_window.md#function-buildnode) _method. It also sets some additional properties for the created node like reference, ID, value, entity, and whether it is a utility function or not._
```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnToString () 
```





**Returns:**

Ref&lt;AGENode&gt; A reference to the newly spawned [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) instance. 





        

<hr>



### function SyncLinks 

_Synchronizes the links between nodes._ 
```C++
void AGE::NodeEditorWindow::SyncLinks () 
```



This function iterates over all the links in the [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) and updates the corresponding pins based on the type of pin. It handles different types of pins such as Boolean, Int, Float, String etc., by copying the value from the start pin to the end pin. The function does not return any values. 


        

<hr>



### function TouchNode 

_This function is used to update the touch time for a specific node._ 
```C++
void AGE::NodeEditorWindow::TouchNode (
    ax::NodeEditor::NodeId ID
) 
```





**Parameters:**


* `ID` The unique identifier of the node. 



**Returns:**

void 





        

<hr>



### function UpdateTouch 

_This function updates the touch time for each node in the_ [_**NodeEditorWindow**_](class_a_g_e_1_1_node_editor_window.md) _._
```C++
void AGE::NodeEditorWindow::UpdateTouch (
    float DeltaTime
) 
```



The function iterates over all elements (pairs of nodes and their corresponding touch times) in m\_NodeTouchTime, subtracts the provided DeltaTime from each element's second value if it is greater than zero. This effectively reduces the remaining time for which a node has been touched by the specified amount. If the touch time reaches 0, the function will not further reduce it.




**Parameters:**


* `DeltaTime` The amount of time to subtract from each element's second value in m\_NodeTouchTime. 




        

<hr>
## Protected Static Functions Documentation




### function Splitter 

_Handles the behavior of a splitter in an ImGui context._ 
```C++
static bool AGE::NodeEditorWindow::Splitter (
    bool SplitVertically,
    float Thickness,
    float * Size1,
    float * Size2,
    float Min_Size1,
    float Min_Size2,
    float SplitterLongAxisSize=-1.f
) 
```



This function determines whether the user is interacting with the splitter and updates the size variables accordingly. It takes into account various parameters such as the direction, thickness, minimum sizes, etc. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/NodeEditorWindow.h`

