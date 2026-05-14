

# Class AGE::ShaderLibrary



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Add**](#function-add-12) (const std::string & Name, const Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; & Shader) <br>_Adds a shader to the library with a given name and reference._  |
|  void | [**Add**](#function-add-22) (Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; & Shader) <br>_Adds a shader to the library._  |
|  bool | [**Exists**](#function-exists) (const std::string & Name) <br>_Checks if a shader with the given name exists in the library._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Get**](#function-get) (const std::string & Name) <br>_Retrieves a shader from the library by name._  |
|  std::unordered\_map&lt; std::string, Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; &gt; | [**GetLibrary**](#function-getlibrary) () <br>_Returns a reference to the shader library._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-13) (const std::string & FilePath) <br>_Loads a shader from the given file path and adds it to the library._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-23) (const std::string & FilePath1, const std::string & FilePath2) <br>_Loads a shader from two file paths and adds it to the library._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-33) (const int Name, const std::string & Source) <br>_Loads a shader into the library. The type of shader is determined by the Name parameter, where 1 represents "Vertex" and any other value represents "Pixel"._  |




























## Public Functions Documentation




### function Add [1/2]

_Adds a shader to the library with a given name and reference._ 
```C++
void AGE::ShaderLibrary::Add (
    const std::string & Name,
    const Ref< Shader > & Shader
) 
```



This function adds a new shader to the library if it does not already exist. If a shader with the same name exists, a warning is logged and the function returns without adding anything.




**Parameters:**


* `Name` The name of the shader to add. 
* [**Shader**](class_a_g_e_1_1_shader.md) A reference to the shader object to be added.

Adds a shader to the library with a given name and reference.


This function adds a new shader to the library if it does not already exist. If a shader with the same name exists, a warning is logged and the function returns without adding anything.




**Parameters:**


* `Name` The name of the shader to add. 
* [**Shader**](class_a_g_e_1_1_shader.md) A reference to the shader object to be added. 




        

<hr>



### function Add [2/2]

_Adds a shader to the library._ 
```C++
void AGE::ShaderLibrary::Add (
    Ref< Shader > & Shader
) 
```



This function takes a reference to a shader object and adds it to the library. The name of the shader is obtained by calling the GetShaderName() method on the [**Shader**](class_a_g_e_1_1_shader.md) object.




**Parameters:**


* [**Shader**](class_a_g_e_1_1_shader.md) A reference to the shader object that needs to be added.

Adds a shader to the library.


This function adds a reference to a shader object to the library. The name of the shader is obtained from the GetShaderName() method of the [**Shader**](class_a_g_e_1_1_shader.md) object. If the shader with the same name already exists, it will be replaced by the new one.




**Parameters:**


* [**Shader**](class_a_g_e_1_1_shader.md) A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object that needs to be added to the library. 




        

<hr>



### function Exists 

_Checks if a shader with the given name exists in the library._ 
```C++
bool AGE::ShaderLibrary::Exists (
    const std::string & Name
) 
```



This function checks whether there is an entry for a shader with the specified name in the [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md)'s internal map of shaders. It returns true if such an entry exists, and false otherwise.




**Parameters:**


* `Name` The name of the shader to check for. 



**Returns:**

True if a shader with the given name exists, false otherwise.


Checks if a shader with the given name exists in the library.


This function checks whether there is an entry for a shader with the provided name in the [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md)'s internal map of shaders. It returns true if such an entry exists and false otherwise.




**Parameters:**


* `Name` The name of the shader to check for. 



**Returns:**

True if a shader with the given name exists, false otherwise. 





        

<hr>



### function Get 

_Retrieves a shader from the library by name._ 
```C++
Ref< Shader > AGE::ShaderLibrary::Get (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The name of the shader to retrieve. 



**Returns:**

A reference to the requested shader, or an empty Ref if no such shader exists in the library.


Retrieves a shader from the library by name. 

**Parameters:**


* `Name` The name of the shader to retrieve. 



**Returns:**

A reference to the requested shader. If the shader does not exist, an assertion will be triggered and the program will terminate. 





        

<hr>



### function GetLibrary 

_Returns a reference to the shader library._ 
```C++
inline std::unordered_map< std::string, Ref< Shader > > AGE::ShaderLibrary::GetLibrary () 
```



This function returns an unordered map where keys are strings and values are references to [**Shader**](class_a_g_e_1_1_shader.md) objects. The purpose of this function is to provide access to all currently loaded shaders in the system.




**Returns:**

An unordered\_map containing string-Shader pairs representing the names and corresponding shaders of all loaded shaders.


Returns a reference to the shader library.


This function returns an unordered map that contains all the shaders in the library. The keys are the names of the shaders and the values are references to the actual [**Shader**](class_a_g_e_1_1_shader.md) objects.




**Returns:**

An unordered\_map containing string-Shader pairs representing the shader library. 





        

<hr>



### function Load [1/3]

_Loads a shader from the given file path and adds it to the library._ 
```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const std::string & FilePath
) 
```





**Parameters:**


* `FilePath` The path of the shader file. 



**Returns:**

A reference to the loaded shader.


Loads a shader from the given file path and adds it to the library. 

**Parameters:**


* `FilePath` The path of the shader file. 



**Returns:**

A reference to the loaded shader. 





        

<hr>



### function Load [2/3]

_Loads a shader from two file paths and adds it to the library._ 
```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```



The function creates a new shader object using `Shader::Create` with the provided file paths, then adds this shader to the library using `Add` method. Finally, it returns the created shader.




**Parameters:**


* `FilePath1` The path of the first shader file. 
* `FilePath2` The path of the second shader file.



**Returns:**

A reference to the loaded shader object.


Loads a shader from the given file paths and adds it to the library.


The function creates a new shader object using `Shader::Create` with the provided file paths, then adds this shader to the library using `Add` method. Finally, it returns the created shader.




**Parameters:**


* `FilePath1` The path of the first shader file. 
* `FilePath2` The path of the second shader file (optional). 



**Returns:**

A reference to the loaded shader object. 





        

<hr>



### function Load [3/3]

_Loads a shader into the library. The type of shader is determined by the Name parameter, where 1 represents "Vertex" and any other value represents "Pixel"._ 
```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const int Name,
    const std::string & Source
) 
```





**Parameters:**


* `Name` An integer representing the type of shader to be loaded. 
* `Source` A string containing the source code for the shader. 



**Returns:**

Returns a reference to the newly loaded [**Shader**](class_a_g_e_1_1_shader.md) object.


Loads a shader into the library. The type of shader is determined by the Name parameter, where 1 represents "Vertex" and any other value represents "Pixel". 

**Parameters:**


* `Name` An integer representing the type of shader to be loaded (1 for [**Vertex**](struct_a_g_e_1_1_vertex.md), anything else for Pixel). 
* `Source` A string containing the source code of the shader. 



**Returns:**

Returns a reference to the newly created [**Shader**](class_a_g_e_1_1_shader.md) object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Shader.h`

