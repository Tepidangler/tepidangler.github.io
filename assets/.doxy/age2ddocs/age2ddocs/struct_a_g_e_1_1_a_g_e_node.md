

# Struct AGE::AGENode



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md)








Inherits the following classes: std::enable_shared_from_this< AGENode >


















## Public Attributes

| Type | Name |
| ---: | :--- |
|  ImColor | [**Color**](#variable-color)  <br> |
|  [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md), [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; | [**Func**](#variable-func)  <br> |
|  [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) | [**FunctionArgs**](#variable-functionargs)  <br> |
|  ax::NodeEditor::NodeId | [**ID**](#variable-id)  <br> |
|  std::vector&lt; Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; &gt; | [**Inputs**](#variable-inputs)  <br> |
|  std::string | [**Name**](#variable-name)  <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**NextNode**](#variable-nextnode)  <br> |
|  uint32\_t | [**NextNodeID**](#variable-nextnodeid)   = `0`<br> |
|  std::vector&lt; Ref&lt; [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) &gt; &gt; | [**Outputs**](#variable-outputs)  <br> |
|  std::string | [**SavedState**](#variable-savedstate)  <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Size**](#variable-size)  <br> |
|  std::string | [**State**](#variable-state)  <br> |
|  AGENodeType | [**Type**](#variable-type)  <br> |
|  bool | [**bIsBeginPlay**](#variable-bisbeginplay)   = `false`<br> |
|  bool | [**bIsOnUpdate**](#variable-bisonupdate)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGENode**](#function-agenode-12) () = default<br> |
|   | [**AGENode**](#function-agenode-22) (ax::NodeEditor::NodeId id, const char \* name, ImColor color=ImColor(255, 255, 255)) <br> |
|  bool | [**CompileOutputPins**](#function-compileoutputpins) () <br> |
|  void | [**SetNodeFuncArguments**](#function-setnodefuncarguments) () <br> |
|  bool | [**operator&lt;**](#function-operator) (const [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Other) const<br> |
| virtual  | [**~AGENode**](#function-agenode) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Data) <br> |


























## Public Attributes Documentation




### variable Color 

```C++
ImColor AGE::AGENode::Color;
```




<hr>



### variable Func 

```C++
AGEFunction<AGENode, ScriptableEntity> AGE::AGENode::Func;
```




<hr>



### variable FunctionArgs 

```C++
NodeArguments AGE::AGENode::FunctionArgs;
```




<hr>



### variable ID 

```C++
ax::NodeEditor::NodeId AGE::AGENode::ID;
```




<hr>



### variable Inputs 

```C++
std::vector<Ref<AGEPin> > AGE::AGENode::Inputs;
```




<hr>



### variable Name 

```C++
std::string AGE::AGENode::Name;
```




<hr>



### variable NextNode 

```C++
Ref<AGENode> AGE::AGENode::NextNode;
```




<hr>



### variable NextNodeID 

```C++
uint32_t AGE::AGENode::NextNodeID;
```




<hr>



### variable Outputs 

```C++
std::vector<Ref<AGEPin> > AGE::AGENode::Outputs;
```




<hr>



### variable SavedState 

```C++
std::string AGE::AGENode::SavedState;
```




<hr>



### variable Size 

```C++
Vector2 AGE::AGENode::Size;
```




<hr>



### variable State 

```C++
std::string AGE::AGENode::State;
```




<hr>



### variable Type 

```C++
AGENodeType AGE::AGENode::Type;
```




<hr>



### variable bIsBeginPlay 

```C++
bool AGE::AGENode::bIsBeginPlay;
```




<hr>



### variable bIsOnUpdate 

```C++
bool AGE::AGENode::bIsOnUpdate;
```




<hr>
## Public Functions Documentation




### function AGENode [1/2]

```C++
AGE::AGENode::AGENode () = default
```




<hr>



### function AGENode [2/2]

```C++
inline AGE::AGENode::AGENode (
    ax::NodeEditor::NodeId id,
    const char * name,
    ImColor color=ImColor(255, 255, 255)
) 
```




<hr>



### function CompileOutputPins 

```C++
inline bool AGE::AGENode::CompileOutputPins () 
```




<hr>



### function SetNodeFuncArguments 

```C++
inline void AGE::AGENode::SetNodeFuncArguments () 
```




<hr>



### function operator&lt; 

```C++
inline bool AGE::AGENode::operator< (
    const AGENode & Other
) const
```




<hr>



### function ~AGENode 

```C++
virtual AGE::AGENode::~AGENode () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::AGENode::Deserialize (
    DataReader * Serializer,
    AGENode & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::AGENode::Serialize (
    DataWriter * Serializer,
    const AGENode & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

