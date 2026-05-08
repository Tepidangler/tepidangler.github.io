

# Class AGE::ShaderLibrary



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Add**](#function-add-12) (const std::string & Name, const Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; & Shader) <br> |
|  void | [**Add**](#function-add-22) (Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; & Shader) <br> |
|  bool | [**Exists**](#function-exists) (const std::string & Name) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Get**](#function-get) (const std::string & Name) <br> |
|  std::unordered\_map&lt; std::string, Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; &gt; | [**GetLibrary**](#function-getlibrary) () <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-13) (const std::string & FilePath) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-23) (const std::string & FilePath1, const std::string & FilePath2) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Load**](#function-load-33) (const int Name, const std::string & Source) <br> |




























## Public Functions Documentation




### function Add [1/2]

```C++
void AGE::ShaderLibrary::Add (
    const std::string & Name,
    const Ref< Shader > & Shader
) 
```




<hr>



### function Add [2/2]

```C++
void AGE::ShaderLibrary::Add (
    Ref< Shader > & Shader
) 
```




<hr>



### function Exists 

```C++
bool AGE::ShaderLibrary::Exists (
    const std::string & Name
) 
```




<hr>



### function Get 

```C++
Ref< Shader > AGE::ShaderLibrary::Get (
    const std::string & Name
) 
```




<hr>



### function GetLibrary 

```C++
inline std::unordered_map< std::string, Ref< Shader > > AGE::ShaderLibrary::GetLibrary () 
```




<hr>



### function Load [1/3]

```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const std::string & FilePath
) 
```




<hr>



### function Load [2/3]

```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const std::string & FilePath1,
    const std::string & FilePath2
) 
```




<hr>



### function Load [3/3]

```C++
Ref< Shader > AGE::ShaderLibrary::Load (
    const int Name,
    const std::string & Source
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Shader.h`

