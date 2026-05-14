

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
|   | [**AGENodeLink**](#function-agenodelink-12) () = default<br>_Default constructor for_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _class._ |
|   | [**AGENodeLink**](#function-agenodelink-22) (ax::NodeEditor::LinkId LID, ax::NodeEditor::PinId SPID, ax::NodeEditor::PinId EPID) <br>_Constructs an instance of_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _with the given LinkId, StartPinId and EndPinId. The color is set to white (255, 255, 255)._ |
| virtual  | [**~AGENodeLink**](#function-agenodelink) () = default<br>_Virtual destructor for the_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) & Data) <br>_Deserializes data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _into an_[_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) & Data) <br>_This function serializes an_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























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

_Default constructor for_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _class._
```C++
AGE::AGENodeLink::AGENodeLink () = default
```



This function initializes an instance of the [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) class with its members set to their default values. The default value is determined by the C++ standard, which may vary depending on the specific type of each member variable. For example, if a member variable is of type int, it will be initialized to 0; for pointers, they will be initialized to nullptr. If you need more control over initialization, consider using an initializer list in the constructor definition.




**Returns:**

An instance of [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) with all members set to their default values.


Default constructor for [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) class. 


        

<hr>



### function AGENodeLink [2/2]

_Constructs an instance of_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _with the given LinkId, StartPinId and EndPinId. The color is set to white (255, 255, 255)._
```C++
inline AGE::AGENodeLink::AGENodeLink (
    ax::NodeEditor::LinkId LID,
    ax::NodeEditor::PinId SPID,
    ax::NodeEditor::PinId EPID
) 
```





**Parameters:**


* `LID` The unique identifier for this link. 
* `SPID` The id of the start pin of this link. 
* `EPID` The id of the end pin of this link.

Constructs an instance of [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) with the given LinkId, StartPinId and EndPinId. The color is set to white (255, 255, 255). 

**Parameters:**


* `LID` Unique identifier for the link. 
* `SPID` Identifier for the start pin of the link. 
* `EPID` Identifier for the end pin of the link. 




        

<hr>



### function ~AGENodeLink 

_Virtual destructor for the_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _class._
```C++
virtual AGE::AGENodeLink::~AGENodeLink () = default
```



This function is responsible for freeing any resources that were allocated by the object during its lifetime. It does not take any parameters and returns void.


Virtual destructor for the [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not take any parameters and returns void. 


        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserializes data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _into an_[_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _object._
```C++
static inline void AGE::AGENodeLink::Deserialize (
    DataReader * Serializer,
    AGENodeLink & Data
) 
```



This function reads raw data from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and populates an [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object with it. The data read includes IDs for the node link, start pin ID, end pin ID, and color of the link.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` An [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object where the deserialized data will be stored.



**Returns:**

void


Deserialize function for [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) data structure. This function reads raw data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and populates an [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object with the deserialized data.




**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides the serialized data. 
* `Data` Reference to the [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_This function serializes an_ [_**AGENodeLink**_](struct_a_g_e_1_1_a_g_e_node_link.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::AGENodeLink::Serialize (
    DataWriter * Serializer,
    const AGENodeLink & Data
) 
```



The function writes the ID, StartPinID, EndPinID and Color of the given [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md). It uses WriteRaw method from [**DataWriter**](class_a_g_e_1_1_data_writer.md) to write each value as raw binary data.




**Parameters:**


* `Serializer` Pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be used for serialization. 
* `Data` Reference to an [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object that needs to be serialized.

This function serializes an [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md).


The function writes the ID, StartPinID, EndPinID and Color of the given [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md). It uses WriteRaw method for each data type (uint64\_t, uint32\_t) to write the respective values into the serializer.




**Parameters:**


* `Serializer` Pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the serialized data will be written. 
* `Data` Reference to an [**AGENodeLink**](struct_a_g_e_1_1_a_g_e_node_link.md) object that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

