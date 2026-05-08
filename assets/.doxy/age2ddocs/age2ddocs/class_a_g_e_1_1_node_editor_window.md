

# Class AGE::NodeEditorWindow



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md)








Inherits the following classes: [AGE::Layer](class_a_g_e_1_1_layer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetWindowName**](#function-getwindowname) () const<br> |
|   | [**NodeEditorWindow**](#function-nodeeditorwindow) (const std::string & WindowName, ax::NodeEditor::EditorContext \* Context, void \* Target=nullptr, bool LoadingExisting=false) <br> |
| virtual void | [**OnAttach**](#function-onattach) () <br> |
| virtual void | [**OnImGuiRender**](#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual  | [**~NodeEditorWindow**](#function-nodeeditorwindow) () <br> |


## Public Functions inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  const std::string & | [**GetName**](class_a_g_e_1_1_layer.md#function-getname) () const<br> |
|  float | [**GetTime**](class_a_g_e_1_1_layer.md#function-gettime) () <br> |
| virtual void | [**Init**](class_a_g_e_1_1_layer.md#function-init) () <br> |
|   | [**Layer**](class_a_g_e_1_1_layer.md#function-layer) (const std::string & name="Layer") <br> |
| virtual void | [**OnAttach**](class_a_g_e_1_1_layer.md#function-onattach) () <br> |
| virtual void | [**OnDetach**](class_a_g_e_1_1_layer.md#function-ondetach) () <br> |
| virtual void | [**OnEvent**](class_a_g_e_1_1_layer.md#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) <br> |
| virtual void | [**OnImGuiRender**](class_a_g_e_1_1_layer.md#function-onimguirender) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**OnUpdate**](class_a_g_e_1_1_layer.md#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual  | [**~Layer**](class_a_g_e_1_1_layer.md#function-layer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NodeEditorWindow**](class_a_g_e_1_1_node_editor_window.md) & Data) <br> |














## Protected Attributes inherited from AGE::Layer

See [AGE::Layer](class_a_g_e_1_1_layer.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_DebugName**](class_a_g_e_1_1_layer.md#variable-m_debugname)  <br> |






























## Protected Functions

| Type | Name |
| ---: | :--- |
|  void | [**BuildNode**](#function-buildnode) (Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; Node) <br> |
|  void | [**BuildNodes**](#function-buildnodes) () <br> |
|  bool | [**CanCreateLink**](#function-cancreatelink) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; A, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; B) <br> |
|  void | [**CompileGraph**](#function-compilegraph) () <br> |
|  void | [**DeleteNode**](#function-deletenode) () <br> |
|  void | [**DeregisterFunctions**](#function-deregisterfunctions) () <br> |
|  void | [**DrawAndCreateNewLink**](#function-drawandcreatenewlink) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, std::function&lt; void(const char \*, ImColor)&gt; ShowLabelFunction) <br> |
|  void | [**DrawAndCreateNewNode**](#function-drawandcreatenewnode) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newNodeLinkPin, bool createNewNode, std::function&lt; void(const char \*, ImColor)&gt; ShowLabelFunction) <br> |
|  void | [**DrawHeader**](#function-drawheader) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, bool IsSimple, bool HasOutputCallbacks) <br> |
|  void | [**DrawInputPins**](#function-drawinputpins) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin) <br> |
|  void | [**DrawNodes**](#function-drawnodes) (Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin) <br> |
|  void | [**DrawOutputPins**](#function-drawoutputpins) (ax::NodeEditor::Utilities::BlueprintNodeBuilder & Builder, Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node, Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & newLinkPin, bool IsSimple) <br> |
|  void | [**DrawPinIcon**](#function-drawpinicon) (const Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; & Pin, bool Connected, int Alpha) <br> |
|  Ref&lt; [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) &gt; | [**FindLink**](#function-findlink-12) (ax::NodeEditor::LinkId ID) <br> |
|  Ref&lt; [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) &gt; | [**FindLink**](#function-findlink-22) (ax::NodeEditor::PinId ID) <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**FindNode**](#function-findnode) (ax::NodeEditor::NodeId ID) <br> |
|  Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; | [**FindPin**](#function-findpin) (ax::NodeEditor::PinId ID) <br> |
|  ImColor | [**GetIconColor**](#function-geticoncolor) (AGEPinType Type) <br> |
|  uint32\_t | [**GetNextID**](#function-getnextid) () <br> |
|  ax::NodeEditor::LinkId | [**GetNextLinkID**](#function-getnextlinkid) () <br> |
|  float | [**GetTouchProgress**](#function-gettouchprogress) (ax::NodeEditor::NodeId ID) <br> |
|  ImRect | [**ImGui\_GetItemRect**](#function-imgui_getitemrect) () <br> |
|  ImRect | [**ImRect\_Expanded**](#function-imrect_expanded) (const ImRect & Rect, float x, float y) <br> |
|  bool | [**IsPinLinked**](#function-ispinlinked) (ax::NodeEditor::PinId ID) <br> |
|  void | [**RebuildWindow**](#function-rebuildwindow) () <br> |
|  void | [**RegisterFunctions**](#function-registerfunctions) () <br> |
|  void | [**RenderWindow**](#function-renderwindow) (bool \* Opened, [**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**SaveGraph**](#function-savegraph) () <br> |
|  void | [**ShowDetailPanel**](#function-showdetailpanel) (bool \* ShowPanel=nullptr) <br> |
|  void | [**ShowLeftPane**](#function-showleftpane) (float PanelWidth) <br> |
|  void | [**ShowNodeOptions**](#function-shownodeoptions) (Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; & Node) <br> |
|  void | [**ShowStyleEditor**](#function-showstyleeditor) (bool \* Show=nullptr) <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnAppendString**](#function-spawnappendstring) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnBeginPlayNode**](#function-spawnbeginplaynode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCosine**](#function-spawncosine) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCrossProduct**](#function-spawncrossproduct) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnCubeRoot**](#function-spawncuberoot) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnDivide**](#function-spawndivide) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnDotProduct**](#function-spawndotproduct) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnEqualToNode**](#function-spawnequaltonode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGTETNode**](#function-spawngtetnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetActor**](#function-spawngetactor) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetLocation2D**](#function-spawngetlocation2d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGetLocation3D**](#function-spawngetlocation3d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnGreaterThanNode**](#function-spawngreaterthannode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnLTETNode**](#function-spawnltetnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnLessThanNode**](#function-spawnlessthannode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnMakeLiteralString**](#function-spawnmakeliteralstring) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnModulo**](#function-spawnmodulo) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnMultiply**](#function-spawnmultiply) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnOnUpdateNode**](#function-spawnonupdatenode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnOutputActionNode**](#function-spawnoutputactionnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnPow**](#function-spawnpow) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnPrintStringNode**](#function-spawnprintstringnode) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSetLocation2D**](#function-spawnsetlocation2d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSetLocation3D**](#function-spawnsetlocation3d) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSine**](#function-spawnsine) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSquareRoot**](#function-spawnsquareroot) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSubtract**](#function-spawnsubtract) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnSum**](#function-spawnsum) () <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**SpawnToString**](#function-spawntostring) () <br> |
|  void | [**SyncLinks**](#function-synclinks) () <br> |
|  void | [**TouchNode**](#function-touchnode) (ax::NodeEditor::NodeId ID) <br> |
|  void | [**UpdateTouch**](#function-updatetouch) (float DeltaTime) <br> |




## Protected Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**Splitter**](#function-splitter) (bool SplitVertically, float Thickness, float \* Size1, float \* Size2, float Min\_Size1, float Min\_Size2, float SplitterLongAxisSize=-1.f) <br> |




## Public Functions Documentation




### function GetWindowName 

```C++
inline const std::string & AGE::NodeEditorWindow::GetWindowName () const
```




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

```C++
virtual void AGE::NodeEditorWindow::OnAttach () 
```



Implements [*AGE::Layer::OnAttach*](class_a_g_e_1_1_layer.md#function-onattach)


<hr>



### function OnImGuiRender 

```C++
virtual void AGE::NodeEditorWindow::OnImGuiRender (
    TimeStep DeltaTime
) 
```



Implements [*AGE::Layer::OnImGuiRender*](class_a_g_e_1_1_layer.md#function-onimguirender)


<hr>



### function ~NodeEditorWindow 

```C++
virtual AGE::NodeEditorWindow::~NodeEditorWindow () 
```




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

```C++
static inline void AGE::NodeEditorWindow::Serialize (
    DataWriter * Serializer,
    const NodeEditorWindow & Data
) 
```




<hr>
## Protected Functions Documentation




### function BuildNode 

```C++
void AGE::NodeEditorWindow::BuildNode (
    Ref< AGENode > Node
) 
```




<hr>



### function BuildNodes 

```C++
void AGE::NodeEditorWindow::BuildNodes () 
```




<hr>



### function CanCreateLink 

```C++
bool AGE::NodeEditorWindow::CanCreateLink (
    Ref< AGEPin > A,
    Ref< AGEPin > B
) 
```




<hr>



### function CompileGraph 

```C++
void AGE::NodeEditorWindow::CompileGraph () 
```




<hr>



### function DeleteNode 

```C++
void AGE::NodeEditorWindow::DeleteNode () 
```




<hr>



### function DeregisterFunctions 

```C++
void AGE::NodeEditorWindow::DeregisterFunctions () 
```




<hr>



### function DrawAndCreateNewLink 

```C++
void AGE::NodeEditorWindow::DrawAndCreateNewLink (
    Ref< AGEPin > & newLinkPin,
    std::function< void(const char *, ImColor)> ShowLabelFunction
) 
```




<hr>



### function DrawAndCreateNewNode 

```C++
void AGE::NodeEditorWindow::DrawAndCreateNewNode (
    Ref< AGEPin > & newLinkPin,
    Ref< AGEPin > & newNodeLinkPin,
    bool createNewNode,
    std::function< void(const char *, ImColor)> ShowLabelFunction
) 
```




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

```C++
Ref< AGENodeLink > AGE::NodeEditorWindow::FindLink (
    ax::NodeEditor::LinkId ID
) 
```




<hr>



### function FindLink [2/2]

```C++
Ref< AGENodeLink > AGE::NodeEditorWindow::FindLink (
    ax::NodeEditor::PinId ID
) 
```




<hr>



### function FindNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::FindNode (
    ax::NodeEditor::NodeId ID
) 
```




<hr>



### function FindPin 

```C++
Ref< AGEPin > AGE::NodeEditorWindow::FindPin (
    ax::NodeEditor::PinId ID
) 
```




<hr>



### function GetIconColor 

```C++
ImColor AGE::NodeEditorWindow::GetIconColor (
    AGEPinType Type
) 
```




<hr>



### function GetNextID 

```C++
uint32_t AGE::NodeEditorWindow::GetNextID () 
```




<hr>



### function GetNextLinkID 

```C++
ax::NodeEditor::LinkId AGE::NodeEditorWindow::GetNextLinkID () 
```




<hr>



### function GetTouchProgress 

```C++
float AGE::NodeEditorWindow::GetTouchProgress (
    ax::NodeEditor::NodeId ID
) 
```




<hr>



### function ImGui\_GetItemRect 

```C++
ImRect AGE::NodeEditorWindow::ImGui_GetItemRect () 
```




<hr>



### function ImRect\_Expanded 

```C++
ImRect AGE::NodeEditorWindow::ImRect_Expanded (
    const ImRect & Rect,
    float x,
    float y
) 
```




<hr>



### function IsPinLinked 

```C++
bool AGE::NodeEditorWindow::IsPinLinked (
    ax::NodeEditor::PinId ID
) 
```




<hr>



### function RebuildWindow 

```C++
void AGE::NodeEditorWindow::RebuildWindow () 
```




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

```C++
void AGE::NodeEditorWindow::SaveGraph () 
```




<hr>



### function ShowDetailPanel 

```C++
void AGE::NodeEditorWindow::ShowDetailPanel (
    bool * ShowPanel=nullptr
) 
```




<hr>



### function ShowLeftPane 

```C++
void AGE::NodeEditorWindow::ShowLeftPane (
    float PanelWidth
) 
```




<hr>



### function ShowNodeOptions 

```C++
void AGE::NodeEditorWindow::ShowNodeOptions (
    Ref< AGENode > & Node
) 
```




<hr>



### function ShowStyleEditor 

```C++
void AGE::NodeEditorWindow::ShowStyleEditor (
    bool * Show=nullptr
) 
```




<hr>



### function SpawnAppendString 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnAppendString () 
```




<hr>



### function SpawnBeginPlayNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnBeginPlayNode () 
```




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

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnDivide () 
```




<hr>



### function SpawnDotProduct 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnDotProduct () 
```




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

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGetLocation3D () 
```




<hr>



### function SpawnGreaterThanNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnGreaterThanNode () 
```




<hr>



### function SpawnLTETNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnLTETNode () 
```




<hr>



### function SpawnLessThanNode 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnLessThanNode () 
```




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

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnOutputActionNode () 
```




<hr>



### function SpawnPow 

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnPow () 
```




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

```C++
Ref< AGENode > AGE::NodeEditorWindow::SpawnToString () 
```




<hr>



### function SyncLinks 

```C++
void AGE::NodeEditorWindow::SyncLinks () 
```




<hr>



### function TouchNode 

```C++
void AGE::NodeEditorWindow::TouchNode (
    ax::NodeEditor::NodeId ID
) 
```




<hr>



### function UpdateTouch 

```C++
void AGE::NodeEditorWindow::UpdateTouch (
    float DeltaTime
) 
```




<hr>
## Protected Static Functions Documentation




### function Splitter 

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




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/NodeEditorWindow.h`

