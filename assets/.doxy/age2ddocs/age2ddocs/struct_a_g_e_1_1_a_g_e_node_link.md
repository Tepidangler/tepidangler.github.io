

# Struct AGE::AGENodeLink



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  ImColor | [**Color**](#variable-color)  <br> |
|  ax::NodeEditor::PinId | [**EndPinID**](#variable-endpinid)  <br> |
|  ax::NodeEditor::LinkId | [**ID**](#variable-id)  <br> |
|  ax::NodeEditor::PinId | [**StartPinID**](#variable-startpinid)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGENodeLink**](#function-agenodelink-12) () = default<br> |
|   | [**AGENodeLink**](#function-agenodelink-22) (ax::NodeEditor::LinkId LID, ax::NodeEditor::PinId SPID, ax::NodeEditor::PinId EPID) <br> |
| virtual  | [**~AGENodeLink**](#function-agenodelink) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) & Data) <br> |


























## Public Attributes Documentation




### variable Color 

```C++
ImColor AGE::AGENodeLink::Color;
```




<hr>



### variable EndPinID 

```C++
ax::NodeEditor::PinId AGE::AGENodeLink::EndPinID;
```




<hr>



### variable ID 

```C++
ax::NodeEditor::LinkId AGE::AGENodeLink::ID;
```




<hr>



### variable StartPinID 

```C++
ax::NodeEditor::PinId AGE::AGENodeLink::StartPinID;
```




<hr>
## Public Functions Documentation




### function AGENodeLink [1/2]

```C++
AGE::AGENodeLink::AGENodeLink () = default
```




<hr>



### function AGENodeLink [2/2]

```C++
inline AGE::AGENodeLink::AGENodeLink (
    ax::NodeEditor::LinkId LID,
    ax::NodeEditor::PinId SPID,
    ax::NodeEditor::PinId EPID
) 
```




<hr>



### function ~AGENodeLink 

```C++
virtual AGE::AGENodeLink::~AGENodeLink () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::AGENodeLink::Deserialize (
    DataReader * Serializer,
    AGENodeLink & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::AGENodeLink::Serialize (
    DataWriter * Serializer,
    const AGENodeLink & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

