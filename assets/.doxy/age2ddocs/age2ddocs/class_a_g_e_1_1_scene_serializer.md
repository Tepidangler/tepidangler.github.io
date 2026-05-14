

# Class AGE::SceneSerializer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneSerializer**](class_a_g_e_1_1_scene_serializer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**Deserialize**](#function-deserialize) (const std::string & FilePath) <br> |
|   | [**SceneSerializer**](#function-sceneserializer) (const Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; & S) <br>_Constructs a_ [_**SceneSerializer**_](class_a_g_e_1_1_scene_serializer.md) _object with the given scene reference._ |
|  void | [**Serialize**](#function-serialize) (const std::string & FilePath) <br>_This function serializes the current scene into a YAML file at the specified path._  |




























## Public Functions Documentation




### function Deserialize 

```C++
bool AGE::SceneSerializer::Deserialize (
    const std::string & FilePath
) 
```




<hr>



### function SceneSerializer 

_Constructs a_ [_**SceneSerializer**_](class_a_g_e_1_1_scene_serializer.md) _object with the given scene reference._
```C++
AGE::SceneSerializer::SceneSerializer (
    const Ref< Scene > & S
) 
```



This constructor initializes the m\_Scene member variable with the provided scene reference.




**Parameters:**


* `S` A const reference to a Ref&lt;Scene&gt; object representing the scene to be serialized. 




        

<hr>



### function Serialize 

_This function serializes the current scene into a YAML file at the specified path._ 
```C++
void AGE::SceneSerializer::Serialize (
    const std::string & FilePath
) 
```



The function extracts the filename from the provided filepath, sets this as the name of the scene, and then writes out the scene data to the file in YAML format. Each entity in the scene is represented by an entry in the "Entities" sequence.




**Parameters:**


* `FilePath` A string representing the path where the serialized scene should be saved.



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Public/Serializers.h`

