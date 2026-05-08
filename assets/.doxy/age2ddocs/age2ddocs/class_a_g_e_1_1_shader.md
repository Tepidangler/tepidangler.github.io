

# Class AGE::Shader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Shader**](class_a_g_e_1_1_shader.md)










Inherited by the following classes: [AGE::OpenGLShader](class_a_g_e_1_1_open_g_l_shader.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetRendererID**](#function-getrendererid) () const = 0<br> |
| virtual const std::string & | [**GetShaderName**](#function-getshadername) () const = 0<br> |
| virtual void | [**SetFloat**](#function-setfloat) (const char \* Name, float Values, float \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat2**](#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat3**](#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, const [**Vector3**](struct_a_g_e_1_1_vector3.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat4**](#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Value, const [**Vector4**](struct_a_g_e_1_1_vector4.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetInt**](#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const = 0<br> |
| virtual void | [**SetMat3**](#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const = 0<br> |
| virtual void | [**SetMat4**](#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Matrix) const = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual  | [**~Shader**](#function-shader) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-13) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-23) (const std::string & FilePath) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](#function-create-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br> |


























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
    float Values,
    float * ValuePtr=nullptr,
    int Count=2
) const = 0
```




<hr>



### function SetFloat2 

```C++
virtual void AGE::Shader::SetFloat2 (
    const char * Name,
    const Vector2 & Values,
    const Vector2 * ValuePtr=nullptr,
    int Count=2
) const = 0
```




<hr>



### function SetFloat3 

```C++
virtual void AGE::Shader::SetFloat3 (
    const char * Name,
    const Vector3 & Values,
    const Vector3 * ValuePtr=nullptr,
    int Count=2
) const = 0
```




<hr>



### function SetFloat4 

```C++
virtual void AGE::Shader::SetFloat4 (
    const char * Name,
    const Vector4 & Value,
    const Vector4 * ValuePtr=nullptr,
    int Count=2
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
    const Matrix4D & Matrix
) const = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::Shader::Unbind () const = 0
```




<hr>



### function ~Shader 

```C++
inline virtual AGE::Shader::~Shader () 
```




<hr>
## Public Static Functions Documentation




### function Create [1/3]

```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & VertexSrcPath,
    const std::string & FragmentSrcPath
) 
```




<hr>



### function Create [2/3]

```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & FilePath
) 
```




<hr>



### function Create [3/3]

```C++
static Ref< Shader > AGE::Shader::Create (
    const std::string & Name,
    const std::string & VertexSrc,
    const std::string & FragmentSrc
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Shader.h`

