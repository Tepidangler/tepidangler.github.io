

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
|   | [**AGENode**](#function-agenode-12) () = default<br>_Default constructor for_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _class._ |
|   | [**AGENode**](#function-agenode-22) (ax::NodeEditor::NodeId id, const char \* name, ImColor color=ImColor(255, 255, 255)) <br>_Constructs an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with the given parameters._ |
|  bool | [**CompileOutputPins**](#function-compileoutputpins) () <br> |
|  void | [**SetNodeFuncArguments**](#function-setnodefuncarguments) () <br>_This function sets the arguments for a node function based on the input parameters._  |
|  bool | [**operator&lt;**](#function-operator) (const [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Other) const<br>_Compares the ID of this node with another node's ID._  |
| virtual  | [**~AGENode**](#function-agenode) () = default<br>_Virtual destructor for the_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Data) <br>_Deserializes an object of type_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _instance._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) & Data) <br>_Serializes an_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























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

_Default constructor for_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _class._
```C++
AGE::AGENode::AGENode () = default
```



This function initializes an instance of the [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) class with its default values. It does not take any parameters and returns nothing.


Default constructor for [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) class. 


        

<hr>



### function AGENode [2/2]

_Constructs an instance of_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _with the given parameters._
```C++
inline AGE::AGENode::AGENode (
    ax::NodeEditor::NodeId id,
    const char * name,
    ImColor color=ImColor(255, 255, 255)
) 
```



This constructor initializes a new instance of [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with the provided id, name and color. The default color is white (255, 255, 255). The Type is set to Blueprint by default. Size is initialized as 0.f. 

**Parameters:**


* `id` Unique identifier for this node. 
* `name` Name of the node. 
* `color` Color of the node in RGB format (default: white).

Constructs an instance of [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with the given id, name and color.


The function initializes a new instance of [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with the provided id, name, and color. It also sets the default type to Blueprint and size to 0.




**Parameters:**


* `id` Unique identifier for the node. 
* `name` Name or label associated with the node. 
* `color` Color used to represent the node in visualizations. Defaults to white (255, 255, 255).



**Returns:**

An instance of [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) with the provided id, name and color. 





        

<hr>



### function CompileOutputPins 

```C++
inline bool AGE::AGENode::CompileOutputPins () 
```




<hr>



### function SetNodeFuncArguments 

_This function sets the arguments for a node function based on the input parameters._ 
```C++
inline void AGE::AGENode::SetNodeFuncArguments () 
```



The function iterates over each argument in `FunctionArgs` and checks its type. If it's a pointer to string or float, it gets the value of that pointer and adds it to `Func.Args`. For an AGEPinType, if it equals Any, it adds the last input's type and value to `Func.Args`.




**Parameters:**


* `bCanSkip` This flag is used to skip certain iterations in the loop based on its value. 



**Returns:**

void No return value. The function modifies `Func.Args` directly. 





        

<hr>



### function operator&lt; 

_Compares the ID of this node with another node's ID._ 
```C++
inline bool AGE::AGENode::operator< (
    const AGENode & Other
) const
```



This function compares the ID of the current node (`this->ID.Get()`) with the ID of the other node passed as an argument (`Other.ID.Get()`). It returns `true` if the ID of this node is less than that of the other, and `false` otherwise.




**Parameters:**


* `Other` The [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) instance to compare with. 



**Returns:**

True if the ID of this node is less than that of the other, false otherwise.


Compares the ID of this node with another node's ID.


This function compares the ID of the current node (`this->ID.Get()`) with the ID of another node (`Other.ID.Get()`). It returns `true` if the ID of this node is less than that of the other, and `false` otherwise.




**Parameters:**


* `Other` The [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) instance to compare against. 



**Returns:**

True if the ID of this node is less than the other's, false otherwise. 





        

<hr>



### function ~AGENode 

_Virtual destructor for the_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _class._
```C++
virtual AGE::AGENode::~AGENode () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not take any parameters and returns no value.


Virtual destructor for the [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserializes an object of type_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _instance._
```C++
static inline void AGE::AGENode::Deserialize (
    DataReader * Serializer,
    AGENode & Data
) 
```



This function reads data from the provided serializer and populates an [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) object with it. The data read includes the node's ID, name, color, inputs, outputs, type, size, next node ID (if any), state, saved state, function arguments, whether the node is in begin play mode, and if it runs on update.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides serialized data. 
* `Data` An lvalue reference to an [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) object where the deserialized data will be stored.

Deserializes an object of type [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) from a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance.


This function reads various data types and populates the provided [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) instance with deserialized data. It uses the [**DataReader**](class_a_g_e_1_1_data_reader.md) to read raw data, strings, arrays, and objects. The function also handles some basic data types like uint64\_t, uint32\_t, bool, [**Vector2**](struct_a_g_e_1_1_vector2.md), etc.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides serialized data. 
* `Data` An lvalue reference to an [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_Serializes an_ [_**AGENode**_](struct_a_g_e_1_1_a_g_e_node.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::AGENode::Serialize (
    DataWriter * Serializer,
    const AGENode & Data
) 
```



This function takes in a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) and an instance of the [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) class, then writes various properties of the node to the [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for serialization. 
* `Data` An instance of the [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) class whose properties are being serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

