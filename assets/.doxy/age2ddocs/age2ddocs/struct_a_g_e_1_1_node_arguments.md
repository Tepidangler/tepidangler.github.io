

# Struct AGE::NodeArguments



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; rttr::variant &gt; | [**Args**](#variable-args)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**NodeArguments**](#function-nodearguments) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) & Data) <br> |


























## Public Attributes Documentation




### variable Args 

```C++
std::vector<rttr::variant> AGE::NodeArguments::Args;
```




<hr>
## Public Functions Documentation




### function NodeArguments 

```C++
AGE::NodeArguments::NodeArguments () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::NodeArguments::Deserialize (
    DataReader * Serializer,
    NodeArguments & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::NodeArguments::Serialize (
    DataWriter * Serializer,
    const NodeArguments & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

