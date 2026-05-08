

# Class AGE::OpenGLShader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md)








Inherits the following classes: [AGE::Shader](class_a_g_e_1_1_shader.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override const<br> |
|  void | [**Compile**](#function-compile) (const std::unordered\_map&lt; GLenum, std::string &gt; & ShaderSources) <br> |
| virtual uint32\_t | [**GetRendererID**](#function-getrendererid) () override const<br> |
| virtual const std::string & | [**GetShaderName**](#function-getshadername) () override const<br> |
|   | [**OpenGLShader**](#function-openglshader-13) (const std::string & FilePath) <br> |
|   | [**OpenGLShader**](#function-openglshader-23) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br> |
|   | [**OpenGLShader**](#function-openglshader-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br> |
|  std::unordered\_map&lt; GLenum, std::string &gt; | [**PreProcess**](#function-preprocess) (const std::string & Source) <br> |
|  std::string | [**ReadFile**](#function-readfile) (const std::string FilePath) <br> |
| virtual void | [**SetFloat**](#function-setfloat) (const char \* Name, float Values, float \* ValuePtr=nullptr, int Count=2) override const<br> |
| virtual void | [**SetFloat2**](#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* ValuePtr=nullptr, int Count=2) override const<br> |
| virtual void | [**SetFloat3**](#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, const [**Vector3**](struct_a_g_e_1_1_vector3.md) \* ValuePtr=nullptr, int Count=2) override const<br> |
| virtual void | [**SetFloat4**](#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Value, const [**Vector4**](struct_a_g_e_1_1_vector4.md) \* ValuePtr=nullptr, int Count=2) override const<br> |
| virtual void | [**SetInt**](#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) override const<br> |
| virtual void | [**SetMat3**](#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) override const<br> |
| virtual void | [**SetMat4**](#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Matrix) override const<br> |
| virtual void | [**Unbind**](#function-unbind) () override const<br> |
|  void | [**UploadFloat**](#function-uploadfloat) (const char \* Name, float Values, float \* ValuePtr=nullptr, int Count=2) const<br> |
|  void | [**UploadFloat2**](#function-uploadfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* ValuePtr=nullptr, int Count=2) const<br> |
|  void | [**UploadFloat3**](#function-uploadfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, const [**Vector3**](struct_a_g_e_1_1_vector3.md) \* ValuePtr=nullptr, int Count=2) const<br> |
|  void | [**UploadFloat4**](#function-uploadfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Value, const [**Vector4**](struct_a_g_e_1_1_vector4.md) \* ValuePtr=nullptr, int Count=2) const<br> |
|  void | [**UploadInt**](#function-uploadint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const<br> |
|  void | [**UploadMat3**](#function-uploadmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const<br> |
|  void | [**UploadMat4**](#function-uploadmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Matrix) const<br> |
| virtual  | [**~OpenGLShader**](#function-openglshader) () <br> |


## Public Functions inherited from AGE::Shader

See [AGE::Shader](class_a_g_e_1_1_shader.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](class_a_g_e_1_1_shader.md#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetRendererID**](class_a_g_e_1_1_shader.md#function-getrendererid) () const = 0<br> |
| virtual const std::string & | [**GetShaderName**](class_a_g_e_1_1_shader.md#function-getshadername) () const = 0<br> |
| virtual void | [**SetFloat**](class_a_g_e_1_1_shader.md#function-setfloat) (const char \* Name, float Values, float \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat2**](class_a_g_e_1_1_shader.md#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat3**](class_a_g_e_1_1_shader.md#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, const [**Vector3**](struct_a_g_e_1_1_vector3.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetFloat4**](class_a_g_e_1_1_shader.md#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Value, const [**Vector4**](struct_a_g_e_1_1_vector4.md) \* ValuePtr=nullptr, int Count=2) const = 0<br> |
| virtual void | [**SetInt**](class_a_g_e_1_1_shader.md#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const = 0<br> |
| virtual void | [**SetMat3**](class_a_g_e_1_1_shader.md#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const = 0<br> |
| virtual void | [**SetMat4**](class_a_g_e_1_1_shader.md#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Matrix) const = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_shader.md#function-unbind) () const = 0<br> |
| virtual  | [**~Shader**](class_a_g_e_1_1_shader.md#function-shader) () <br> |




## Public Static Functions inherited from AGE::Shader

See [AGE::Shader](class_a_g_e_1_1_shader.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-13) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-23) (const std::string & FilePath) <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br> |


















































## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::OpenGLShader::Bind () override const
```



Implements [*AGE::Shader::Bind*](class_a_g_e_1_1_shader.md#function-bind)


<hr>



### function Compile 

```C++
void AGE::OpenGLShader::Compile (
    const std::unordered_map< GLenum, std::string > & ShaderSources
) 
```




<hr>



### function GetRendererID 

```C++
inline virtual uint32_t AGE::OpenGLShader::GetRendererID () override const
```



Implements [*AGE::Shader::GetRendererID*](class_a_g_e_1_1_shader.md#function-getrendererid)


<hr>



### function GetShaderName 

```C++
inline virtual const std::string & AGE::OpenGLShader::GetShaderName () override const
```



Implements [*AGE::Shader::GetShaderName*](class_a_g_e_1_1_shader.md#function-getshadername)


<hr>



### function OpenGLShader [1/3]

```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & FilePath
) 
```




<hr>



### function OpenGLShader [2/3]

```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & VertexSrcPath,
    const std::string & FragmentSrcPath
) 
```




<hr>



### function OpenGLShader [3/3]

```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & Name,
    const std::string & VertexSrc,
    const std::string & FragmentSrc
) 
```




<hr>



### function PreProcess 

```C++
std::unordered_map< GLenum, std::string > AGE::OpenGLShader::PreProcess (
    const std::string & Source
) 
```




<hr>



### function ReadFile 

```C++
std::string AGE::OpenGLShader::ReadFile (
    const std::string FilePath
) 
```




<hr>



### function SetFloat 

```C++
virtual void AGE::OpenGLShader::SetFloat (
    const char * Name,
    float Values,
    float * ValuePtr=nullptr,
    int Count=2
) override const
```



Implements [*AGE::Shader::SetFloat*](class_a_g_e_1_1_shader.md#function-setfloat)


<hr>



### function SetFloat2 

```C++
virtual void AGE::OpenGLShader::SetFloat2 (
    const char * Name,
    const Vector2 & Values,
    const Vector2 * ValuePtr=nullptr,
    int Count=2
) override const
```



Implements [*AGE::Shader::SetFloat2*](class_a_g_e_1_1_shader.md#function-setfloat2)


<hr>



### function SetFloat3 

```C++
virtual void AGE::OpenGLShader::SetFloat3 (
    const char * Name,
    const Vector3 & Values,
    const Vector3 * ValuePtr=nullptr,
    int Count=2
) override const
```



Implements [*AGE::Shader::SetFloat3*](class_a_g_e_1_1_shader.md#function-setfloat3)


<hr>



### function SetFloat4 

```C++
virtual void AGE::OpenGLShader::SetFloat4 (
    const char * Name,
    const Vector4 & Value,
    const Vector4 * ValuePtr=nullptr,
    int Count=2
) override const
```



Implements [*AGE::Shader::SetFloat4*](class_a_g_e_1_1_shader.md#function-setfloat4)


<hr>



### function SetInt 

```C++
virtual void AGE::OpenGLShader::SetInt (
    const char * Name,
    const int Texture=0,
    const int * TexturePtr=nullptr,
    const int Count=2
) override const
```



Implements [*AGE::Shader::SetInt*](class_a_g_e_1_1_shader.md#function-setint)


<hr>



### function SetMat3 

```C++
virtual void AGE::OpenGLShader::SetMat3 (
    const char * Name,
    const Matrix3D & Matrix
) override const
```



Implements [*AGE::Shader::SetMat3*](class_a_g_e_1_1_shader.md#function-setmat3)


<hr>



### function SetMat4 

```C++
virtual void AGE::OpenGLShader::SetMat4 (
    const char * Name,
    const Matrix4D & Matrix
) override const
```



Implements [*AGE::Shader::SetMat4*](class_a_g_e_1_1_shader.md#function-setmat4)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLShader::Unbind () override const
```



Implements [*AGE::Shader::Unbind*](class_a_g_e_1_1_shader.md#function-unbind)


<hr>



### function UploadFloat 

```C++
void AGE::OpenGLShader::UploadFloat (
    const char * Name,
    float Values,
    float * ValuePtr=nullptr,
    int Count=2
) const
```




<hr>



### function UploadFloat2 

```C++
void AGE::OpenGLShader::UploadFloat2 (
    const char * Name,
    const Vector2 & Values,
    const Vector2 * ValuePtr=nullptr,
    int Count=2
) const
```




<hr>



### function UploadFloat3 

```C++
void AGE::OpenGLShader::UploadFloat3 (
    const char * Name,
    const Vector3 & Values,
    const Vector3 * ValuePtr=nullptr,
    int Count=2
) const
```




<hr>



### function UploadFloat4 

```C++
void AGE::OpenGLShader::UploadFloat4 (
    const char * Name,
    const Vector4 & Value,
    const Vector4 * ValuePtr=nullptr,
    int Count=2
) const
```




<hr>



### function UploadInt 

```C++
void AGE::OpenGLShader::UploadInt (
    const char * Name,
    const int Texture=0,
    const int * TexturePtr=nullptr,
    const int Count=2
) const
```




<hr>



### function UploadMat3 

```C++
void AGE::OpenGLShader::UploadMat3 (
    const char * Name,
    const Matrix3D & Matrix
) const
```




<hr>



### function UploadMat4 

```C++
void AGE::OpenGLShader::UploadMat4 (
    const char * Name,
    const Matrix4D & Matrix
) const
```




<hr>



### function ~OpenGLShader 

```C++
virtual AGE::OpenGLShader::~OpenGLShader () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLShader.h`

