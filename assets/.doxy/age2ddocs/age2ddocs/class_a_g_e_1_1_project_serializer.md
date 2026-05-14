

# Class AGE::ProjectSerializer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ProjectSerializer**](class_a_g_e_1_1_project_serializer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**Deserialize**](#function-deserialize) (const std::filesystem::path & FilePath) <br>_Deserializes a project from a YAML file._  |
|  bool | [**DeserializeBinary**](#function-deserializebinary) (const std::filesystem::path & FilePath) <br>_Deserializes a binary file into the project._  |
|   | [**ProjectSerializer**](#function-projectserializer) (Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; Project) <br>_Constructs a new instance of the_ [_**ProjectSerializer**_](class_a_g_e_1_1_project_serializer.md) _class with the given project reference._ |
|  bool | [**Serialize**](#function-serialize) (const std::filesystem::path & FilePath) <br>_Serializes the project configuration and information into a YAML file._  |
|  void | [**SerializeBinary**](#function-serializebinary) (const std::filesystem::path & FilePath) <br> |




























## Public Functions Documentation




### function Deserialize 

_Deserializes a project from a YAML file._ 
```C++
bool AGE::ProjectSerializer::Deserialize (
    const std::filesystem::path & FilePath
) 
```



This function reads the contents of a YAML file and populates the internal configuration and info structures with data from the file. If the file cannot be loaded, an error message is logged and false is returned.




**Parameters:**


* `FilePath` The path to the YAML file containing project information. 



**Returns:**

True if the deserialization was successful, false otherwise. 





        

<hr>



### function DeserializeBinary 

_Deserializes a binary file into the project._ 
```C++
bool AGE::ProjectSerializer::DeserializeBinary (
    const std::filesystem::path & FilePath
) 
```



This function attempts to deserialize a binary file located at the given path into the current project state. It returns true if the operation was successful, and false otherwise.




**Parameters:**


* `FilePath` The path of the binary file to be deserialized. 



**Returns:**

True if the binary file was successfully deserialized, false otherwise. 





        

<hr>



### function ProjectSerializer 

_Constructs a new instance of the_ [_**ProjectSerializer**_](class_a_g_e_1_1_project_serializer.md) _class with the given project reference._
```C++
AGE::ProjectSerializer::ProjectSerializer (
    Ref< Project > Project
) 
```





**Parameters:**


* [**Project**](class_a_g_e_1_1_project.md) The project to be serialized and stored in this object. 




        

<hr>



### function Serialize 

_Serializes the project configuration and information into a YAML file._ 
```C++
bool AGE::ProjectSerializer::Serialize (
    const std::filesystem::path & FilePath
) 
```



This function serializes the project's configuration and information into a YAML file at the specified path. The configuration includes details about the project such as its name, starting scene, asset directory, C++ namespace, copyright notice, audio engine used, renderer used, quest filepath, config filepath, and built scenes.




**Parameters:**


* `FilePath` The path to the YAML file where the serialized data will be written.



**Returns:**

Returns true if the serialization was successful, false otherwise. In this case, it always returns true as there are no exceptions that could cause a failure. 





        

<hr>



### function SerializeBinary 

```C++
void AGE::ProjectSerializer::SerializeBinary (
    const std::filesystem::path & FilePath
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Public/Serializers.h`

