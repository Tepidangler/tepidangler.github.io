

# Struct AGE::AGEPin



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**Boolean**](#variable-boolean)   = `false`<br> |
|  ax::NodeEditor::PinId | [**ID**](#variable-id)  <br> |
|  int | [**Integer**](#variable-integer)   = `0`<br> |
|  int16\_t | [**Integer16**](#variable-integer16)   = `0`<br> |
|  int64\_t | [**Integer64**](#variable-integer64)   = `0`<br> |
|  ax::NodeEditor::PinKind | [**Kind**](#variable-kind)  <br> |
|  std::string | [**Name**](#variable-name)  <br> |
|  ax::NodeEditor::NodeId | [**NextNodeID**](#variable-nextnodeid)  <br> |
|  Ref&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md) &gt; | [**Node**](#variable-node)  <br> |
|  Ref&lt; [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; | [**ObjPtr**](#variable-objptr)   = `nullptr`<br> |
|  std::string | [**String**](#variable-string)   = `""`<br> |
|  AGEPinType | [**Type**](#variable-type)  <br> |
|  uint16\_t | [**UInteger16**](#variable-uinteger16)   = `0`<br> |
|  uint32\_t | [**UInteger32**](#variable-uinteger32)   = `0`<br> |
|  uint64\_t | [**UInteger64**](#variable-uinteger64)   = `0`<br> |
|  float | [**Value**](#variable-value)   = `0.f`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Vector2D**](#variable-vector2d)   = `{ 0.f,0.f }`<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Vector3D**](#variable-vector3d)   = `{ 0.f,0.f,0.f }`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**Vector4D**](#variable-vector4d)   = `{ 0.f,0.f,0.f,0.f }`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEPin**](#function-agepin-12) () = default<br>_Default constructor for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _class._ |
|   | [**AGEPin**](#function-agepin-22) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) id, const char \* name, AGEPinType type) <br>_Constructs an instance of_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _with the given parameters._ |
|  rttr::variant | [**GetValue**](#function-getvalue) (AGEPinType Type) <br>_GetValue is a function that returns an rttr::variant based on the input AGEPinType._  |
| virtual  | [**~AGEPin**](#function-agepin) () = default<br>_Virtual destructor for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) & Data) <br>_Deserialize function for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _structure. This function reads data from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object and populates an_[_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _object with it. The function assumes that the_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _is correctly initialized and ready to read data._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) & Data) <br>_This function serializes an_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























## Public Attributes Documentation




### variable Boolean 

```C++
bool AGE::AGEPin::Boolean;
```




<hr>



### variable ID 

```C++
ax::NodeEditor::PinId AGE::AGEPin::ID;
```




<hr>



### variable Integer 

```C++
int AGE::AGEPin::Integer;
```




<hr>



### variable Integer16 

```C++
int16_t AGE::AGEPin::Integer16;
```




<hr>



### variable Integer64 

```C++
int64_t AGE::AGEPin::Integer64;
```




<hr>



### variable Kind 

```C++
ax::NodeEditor::PinKind AGE::AGEPin::Kind;
```




<hr>



### variable Name 

```C++
std::string AGE::AGEPin::Name;
```




<hr>



### variable NextNodeID 

```C++
ax::NodeEditor::NodeId AGE::AGEPin::NextNodeID;
```




<hr>



### variable Node 

```C++
Ref<AGENode> AGE::AGEPin::Node;
```




<hr>



### variable ObjPtr 

```C++
Ref<ScriptableEntity> AGE::AGEPin::ObjPtr;
```




<hr>



### variable String 

```C++
std::string AGE::AGEPin::String;
```




<hr>



### variable Type 

```C++
AGEPinType AGE::AGEPin::Type;
```




<hr>



### variable UInteger16 

```C++
uint16_t AGE::AGEPin::UInteger16;
```




<hr>



### variable UInteger32 

```C++
uint32_t AGE::AGEPin::UInteger32;
```




<hr>



### variable UInteger64 

```C++
uint64_t AGE::AGEPin::UInteger64;
```




<hr>



### variable Value 

```C++
float AGE::AGEPin::Value;
```




<hr>



### variable Vector2D 

```C++
Vector2 AGE::AGEPin::Vector2D;
```




<hr>



### variable Vector3D 

```C++
Vector3 AGE::AGEPin::Vector3D;
```




<hr>



### variable Vector4D 

```C++
Vector4 AGE::AGEPin::Vector4D;
```




<hr>
## Public Functions Documentation




### function AGEPin [1/2]

_Default constructor for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _class._
```C++
AGE::AGEPin::AGEPin () = default
```



This function initializes an instance of the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) class with its default values. It does not take any parameters and returns nothing.


Default constructor for the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) class. 


        

<hr>



### function AGEPin [2/2]

_Constructs an instance of_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _with the given parameters._
```C++
inline AGE::AGEPin::AGEPin (
    UUID id,
    const char * name,
    AGEPinType type
) 
```



This constructor initializes a new instance of [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) with the provided [**UUID**](class_a_g_e_1_1_u_u_i_d.md), name, and type. The Node pointer is initialized to nullptr, Kind is set to [**Input**](class_a_g_e_1_1_input.md), and other members are assigned their respective values. 

**Parameters:**


* `id` Unique identifier for this pin. 
* `name` Name or label associated with this pin. 
* `type` Specifies the kind of data that this pin can handle.



**Returns:**

[**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md)


Constructs an instance of [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) with the given parameters.


This constructor initializes a new instance of [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) with the provided [**UUID**](class_a_g_e_1_1_u_u_i_d.md), name, and type. The Node pointer is set to nullptr, Kind is initialized as [**Input**](class_a_g_e_1_1_input.md).




**Parameters:**


* `id` Unique identifier for this pin. 
* `name` Name or label associated with this pin. 
* `type` Specifies the type of the pin ([**Input**](class_a_g_e_1_1_input.md), Output, etc.). 




        

<hr>



### function GetValue 

_GetValue is a function that returns an rttr::variant based on the input AGEPinType._ 
```C++
inline rttr::variant AGE::AGEPin::GetValue (
    AGEPinType Type
) 
```



The function takes one parameter, Type of type AGEPinType and returns an rttr::variant. It uses a switch statement to determine which variant to return based on the integer value of Type.




**Parameters:**


* `Type` An enumeration that specifies the type of variant to be returned. 



**Returns:**

The function returns an rttr::variant corresponding to the input AGEPinType. If no matching case is found, it returns nullptr.


GetValue is a function that returns an rttr::variant based on the input AGEPinType.




**Parameters:**


* `Type` The type of pin to get the value for. This can be one of several types defined in AGEPinType, including Boolean, Integer, Integer16, etc. 



**Returns:**

rttr::variant The variant corresponding to the input type. If the type is not recognized, nullptr is returned. 





        

<hr>



### function ~AGEPin 

_Virtual destructor for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _class._
```C++
virtual AGE::AGEPin::~AGEPin () = default
```



This function is responsible for freeing any resources that were allocated by the object, such as memory or file handles. It's a virtual function because it can be overridden in derived classes to provide specific cleanup behavior.




**Returns:**

void


Virtual destructor for the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not perform any specific actions related to the AGEPIN object itself.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize function for the_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _structure. This function reads data from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object and populates an_[_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _object with it. The function assumes that the_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _is correctly initialized and ready to read data._
```C++
static inline void AGE::AGEPin::Deserialize (
    DataReader * Serializer,
    AGEPin & Data
) 
```





**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object which provides the serialized data. 
* `Data` Reference to the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object where the deserialized data will be stored.

Deserialize function for [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) data.


This function reads various types of data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and assigns them to an [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object. It handles different types such as uint64\_t, [**UUID**](class_a_g_e_1_1_u_u_i_d.md), bool, int, int16\_t, int64\_t, uint16\_t, uint32\_t, uint64\_t, float, [**Vector2**](struct_a_g_e_1_1_vector2.md), [**Vector3**](struct_a_g_e_1_1_vector3.md), and [**Vector4**](struct_a_g_e_1_1_vector4.md).




**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides serialized data. 
* `Data` Reference to the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_This function serializes an_ [_**AGEPin**_](struct_a_g_e_1_1_a_g_e_pin.md) _object into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::AGEPin::Serialize (
    DataWriter * Serializer,
    const AGEPin & Data
) 
```



The function writes various properties of the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md), including its ID, NextNodeID, Name, Type, Kind, String, Boolean, Integer, Integer16, Integer64, UInteger16, UInteger32, UInteger64, Value, Vector2D, Vector3D, and Vector4D. It also handles the case where an object pointer is present in the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md). If it exists, a boolean value of true is written to indicate that an object is being serialized, followed by its [**UUID**](class_a_g_e_1_1_u_u_i_d.md). Otherwise, a boolean value of false is written.




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance which will be used for serialization. 
* `Data` Const reference to the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object that needs to be serialized.

This function serializes an [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md).


The function writes various properties of the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md), including its ID, NextNodeID, Name, Type, Kind, String, Boolean, Integer, Integer16, Integer64, UInteger16, UInteger32, UInteger64, Value, Vector2D, Vector3D, and Vector4D.


It also checks if the [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) has an associated [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) object (ObjPtr). If it does, it writes a true flag followed by the [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the associated entity; otherwise, it writes a false flag.




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) where the serialized data will be written. 
* `Data` The [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) object that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

