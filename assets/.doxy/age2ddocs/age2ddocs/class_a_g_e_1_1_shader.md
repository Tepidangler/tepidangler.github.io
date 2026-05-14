

# Class AGE::Shader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Shader**](class_a_g_e_1_1_shader.md)










Inherited by the following classes: [AGE::OpenGLShader](class_a_g_e_1_1_open_g_l_shader.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetRendererID**](#function-getrendererid) () const = 0<br> |
| virtual const std::string & | [**GetShaderName**](#function-getshadername) () const = 0<br> |
| virtual void | [**SetFloat**](#function-setfloat) (const char \* Name, float Values) const = 0<br> |
| virtual void | [**SetFloat2**](#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values) const = 0<br> |
| virtual void | [**SetFloat3**](#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values) const = 0<br> |
| virtual void | [**SetFloat4**](#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) Value) const = 0<br> |
| virtual void | [**SetInt**](#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const = 0<br> |
| virtual void | [**SetMat3**](#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const = 0<br> |
| virtual void | [**SetMat4**](#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Matrix) const = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual  | [**~Shader**](#function-shader) () <br>_Virtual destructor for the_ [_**Shader**_](class_a_g_e_1_1_shader.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-13) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br>_Creates a new shader object based on the current renderer's API._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-23) (const std::string & FilePath) <br>_Creates a shader object based on the current renderer API._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br>_Creates a new shader object._  |


























## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::Shader::Bind () const = 0
```




<hr>



### function GetRendererID 

```C++
inline virtual uint32_t AGE::Shader::GetRendererID () const = 0
```




<hr>



### function GetShaderName 

```C++
virtual const std::string & AGE::Shader::GetShaderName () const = 0
```




<hr>



### function SetFloat 

```C++
virtual void AGE::Shader::SetFloat (
    const char * Name,
    float Values
) const = 0
```




<hr>



### function SetFloat2 

```C++
virtual void AGE::Shader::SetFloat2 (
    const char * Name,
    const Vector2 & Values
) const = 0
```




<hr>



### function SetFloat3 

```C++
virtual void AGE::Shader::SetFloat3 (
    const char * Name,
    const Vector3 & Values
) const = 0
```




<hr>



### function SetFloat4 

```C++
virtual void AGE::Shader::SetFloat4 (
    const char * Name,
    const Vector4 Value
) const = 0
```




<hr>



### function SetInt 

```C++
virtual void AGE::Shader::SetInt (
    const char * Name,
    const int Texture=0,
    const int * TexturePtr=nullptr,
    const int Count=2
) const = 0
```




<hr>



### function SetMat3 

```C++
virtual void AGE::Shader::SetMat3 (
    const char * Name,
    const Matrix3D & Matrix
) const = 0
```




<hr>



### function SetMat4 

```C++
virtual void AGE::Shader::SetMat4 (
    const char * Name,
    const Matrix4D Matrix
) const = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::Shader::Unbind () const = 0
```




<hr>



### function ~Shader 

_Virtual destructor for the_ [_**Shader**_](class_a_g_e_1_1_shader.md) _class._
```C++
inline virtual AGE::Shader::~Shader () 
```



This function is responsible for freeing any resources that were allocated during the lifetime of the object, such as GPU memory or shaders. It does not return anything and thus has an empty return type (void).


Virtual destructor for the [**Shader**](class_a_g_e_1_1_shader.md) class.


This function is responsible for releasing any resources that were acquired by the [**Shader**](class_a_g_e_1_1_shader.md) object during its lifetime. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Create [1/3]

_Creates a new shader object based on the current renderer's API._ 
```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & VertexSrcPath,
    const std::string & FragmentSrcPath
) 
```



The function checks the current renderer's API and creates an appropriate shader object accordingly. If no supported API is detected, it asserts false and returns nullptr.




**Parameters:**


* `VertexSrcPath` A string representing the path to the vertex shader source code file. 
* `FragmentSrcPath` A string representing the path to the fragment shader source code file.



**Returns:**

A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object, which can be either an [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) or another type of shader depending on the current renderer's API. If no supported API is detected, it returns nullptr.


Creates a new shader object based on the current renderer's API.


The function checks the current renderer's API and creates an appropriate shader object accordingly. If no supported API is found, it asserts false and returns nullptr.




**Parameters:**


* `VertexSrcPath` A string representing the path to the vertex shader source code file. 
* `FragmentSrcPath` A string representing the path to the fragment shader source code file.



**Returns:**

A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object, or nullptr if no supported API is found. 





        

<hr>



### function Create [2/3]

_Creates a shader object based on the current renderer API._ 
```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & FilePath
) 
```





**Parameters:**


* `FilePath` The path to the shader file.



**Returns:**

A smart pointer (Ref&lt;Shader&gt;) pointing to the newly created [**Shader**](class_a_g_e_1_1_shader.md) object, or nullptr if an unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) enum value was passed.


Creates a shader object based on the current renderer API.


This function creates and returns a shader object of the appropriate type for the current renderer API. If the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is OpenGL, it will create an [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) object. Otherwise, if the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is unknown or not supported, it will assert false and return nullptr.




**Parameters:**


* `FilePath` The path to the shader file. This parameter is currently unused in this function as all shaders are hardcoded into the executable. 



**Returns:**

A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object if successful, otherwise nullptr. 





        

<hr>



### function Create [3/3]

_Creates a new shader object._ 
```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & Name,
    const std::string & VertexSrc,
    const std::string & FragmentSrc
) 
```



This function creates and returns a reference to a [**Shader**](class_a_g_e_1_1_shader.md) object based on the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use. It supports OpenGL as of now, but more APIs can be added easily by extending this switch-case structure.




**Parameters:**


* `Name` The name of the shader program. 
* `VertexSrc` A string containing the source code for the vertex shader. 
* `FragmentSrc` A string containing the source code for the fragment shader.



**Returns:**

A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object, or nullptr if an unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is in use.


Creates a new shader object.


This function creates and returns a new [**Shader**](class_a_g_e_1_1_shader.md) object based on the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use. It supports OpenGL for now, but more APIs may be added in future. If an unsupported or unknown API is detected, it will assert and return nullptr.




**Parameters:**


* `Name` The name of the shader. This is used to identify the shader during debugging. 
* `VertexSrc` The source code for the vertex shader. 
* `FragmentSrc` The source code for the fragment shader.



**Returns:**

A reference to a [**Shader**](class_a_g_e_1_1_shader.md) object if successful, nullptr otherwise. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Shader.h`

