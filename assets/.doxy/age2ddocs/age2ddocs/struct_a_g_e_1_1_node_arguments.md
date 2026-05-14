

# Struct AGE::NodeArguments



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; rttr::variant &gt; | [**Args**](#variable-args)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**NodeArguments**](#function-nodearguments) () = default<br>_Default constructor for_ [_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Deserialize function for static [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) & Data) <br>_This function is responsible for converting a_ [_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _object into a format that can be easily stored or transmitted. It does this by iterating over each argument in the_[_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _and writing its type and value to the_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _. The type of each argument is written as a byte, followed by the actual data._ |


























## Public Attributes Documentation




### variable Args 

```C++
std::vector<rttr::variant> AGE::NodeArguments::Args;
```




<hr>
## Public Functions Documentation




### function NodeArguments 

_Default constructor for_ [_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _class._
```C++
AGE::NodeArguments::NodeArguments () = default
```



This function initializes the object with its default state. It is used to create an instance of the [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) class without any arguments.




**Returns:**

An instance of the [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) class with all members initialized to their default values.


Default constructor for [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) class. 


        

<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline Deserialize function for static NodeArguments void AGE::NodeArguments::Deserialize (
    DataReader * Serializer,
    NodeArguments & Data
) 
```




<hr>



### function Serialize 

_This function is responsible for converting a_ [_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _object into a format that can be easily stored or transmitted. It does this by iterating over each argument in the_[_**NodeArguments**_](struct_a_g_e_1_1_node_arguments.md) _and writing its type and value to the_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _. The type of each argument is written as a byte, followed by the actual data._
```C++
static inline void AGE::NodeArguments::Serialize (
    DataWriter * Serializer,
    const NodeArguments & Data
) 
```





**Parameters:**


* `Serializer` A pointer to an object that can write raw bytes or strings to a storage medium. 
* `Data` An object containing the arguments to be serialized.

This function serializes the given data into a format that can be easily stored or transmitted.


The function takes in two parameters, a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object and a [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) object. It writes to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object based on the type of each argument in the [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) object.




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for writing data. 
* `Data` The arguments to serialize, stored as a [**NodeArguments**](struct_a_g_e_1_1_node_arguments.md) object.



**Returns:**

void This function does not return any value. It directly writes the serialized data into the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md) object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

