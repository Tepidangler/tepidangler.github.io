

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
|   | [**AGEPin**](#function-agepin-12) () = default<br> |
|   | [**AGEPin**](#function-agepin-22) ([**UUID**](class_a_g_e_1_1_u_u_i_d.md) id, const char \* name, AGEPinType type) <br> |
|  rttr::variant | [**GetValue**](#function-getvalue) (AGEPinType Type) <br> |
| virtual  | [**~AGEPin**](#function-agepin) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGEPin**](struct_a_g_e_1_1_a_g_e_pin.md) & Data) <br> |


























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

```C++
AGE::AGEPin::AGEPin () = default
```




<hr>



### function AGEPin [2/2]

```C++
inline AGE::AGEPin::AGEPin (
    UUID id,
    const char * name,
    AGEPinType type
) 
```




<hr>



### function GetValue 

```C++
inline rttr::variant AGE::AGEPin::GetValue (
    AGEPinType Type
) 
```




<hr>



### function ~AGEPin 

```C++
virtual AGE::AGEPin::~AGEPin () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::AGEPin::Deserialize (
    DataReader * Serializer,
    AGEPin & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::AGEPin::Serialize (
    DataWriter * Serializer,
    const AGEPin & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

