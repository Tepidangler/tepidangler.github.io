

# Struct AGE::SceneInfo



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneInfo**](struct_a_g_e_1_1_scene_info.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  const char \* | [**AssetMap**](#variable-assetmap)  <br> |
|  std::string | [**Flags**](#variable-flags)   = `""`<br> |
|  size\_t | [**Size**](#variable-size)   = `0`<br> |


















## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) & Data) <br>_Deserialize function for_ [_**SceneInfo**_](struct_a_g_e_1_1_scene_info.md) _class._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) & Data) <br>_Serializes the_ [_**SceneInfo**_](struct_a_g_e_1_1_scene_info.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


























## Public Attributes Documentation




### variable AssetMap 

```C++
const char* AGE::SceneInfo::AssetMap;
```




<hr>



### variable Flags 

```C++
std::string AGE::SceneInfo::Flags;
```




<hr>



### variable Size 

```C++
size_t AGE::SceneInfo::Size;
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize function for_ [_**SceneInfo**_](struct_a_g_e_1_1_scene_info.md) _class._
```C++
static void AGE::SceneInfo::Deserialize (
    DataReader * Deserializer,
    SceneInfo & Data
) 
```



This function reads raw data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and populates the provided [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object with it.




**Parameters:**


* `Deserializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides the serialized data. 
* `Data` Reference to the [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object where the deserialized data will be stored.

Deserialize function for [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) class.


This function reads raw data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and populates the provided [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object with it.




**Parameters:**


* `Deserializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides the serialized data. 
* `Data` Reference to the [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_Serializes the_ [_**SceneInfo**_](struct_a_g_e_1_1_scene_info.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static void AGE::SceneInfo::Serialize (
    DataWriter * Serializer,
    const SceneInfo & Data
) 
```



This function serializes various parts of the [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) data structure, including the size of AssetMap and the Flags string. It also writes the raw pointer to AssetMap.




**Parameters:**


* `Serializer` The [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the serialized data will be written into. 
* `Data` The [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) instance that contains the data to be serialized.

This function serializes the [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for serialization. 
* `Data` The [**SceneInfo**](struct_a_g_e_1_1_scene_info.md) object that is being serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Scene.h`

