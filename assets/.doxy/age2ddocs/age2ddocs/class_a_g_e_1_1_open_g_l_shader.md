

# Class AGE::OpenGLShader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md)








Inherits the following classes: [AGE::Shader](class_a_g_e_1_1_shader.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override const<br>_This function binds the OpenGL shader program._  |
|  void | [**Compile**](#function-compile) (const std::unordered\_map&lt; GLenum, std::string &gt; & ShaderSources) <br> |
| virtual uint32\_t | [**GetRendererID**](#function-getrendererid) () override const<br>_Returns the unique identifier for the renderer._  |
| virtual const std::string & | [**GetShaderName**](#function-getshadername) () override const<br>_Returns the name of the shader._  |
|   | [**OpenGLShader**](#function-openglshader-13) (const std::string & FilePath) <br>_Constructs an_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _object from a file path._ |
|   | [**OpenGLShader**](#function-openglshader-23) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br>_Constructor for_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _class. Initializes an instance by reading shader sources from files specified by their paths, compiling them into a program that can be used in OpenGL rendering, and assigning a name derived from the input paths._ |
|   | [**OpenGLShader**](#function-openglshader-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br>_Constructs an_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _object with the given name, vertex source code and fragment source code._ |
|  std::unordered\_map&lt; GLenum, std::string &gt; | [**PreProcess**](#function-preprocess) (const std::string & Source) <br>_Preprocesses OpenGL shader source code to separate different types of shaders based on specific token._  |
|  std::string | [**ReadFile**](#function-readfile) (const std::string FilePath) <br>_Reads a file from the disk and returns its content as a string._  |
| virtual void | [**SetFloat**](#function-setfloat) (const char \* Name, float Values) override const<br>_This function sets a single floating-point value with the given name._  |
| virtual void | [**SetFloat2**](#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values) override const<br>_This function sets a float vector of two elements with the given name._  |
| virtual void | [**SetFloat3**](#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values) override const<br>_This function sets a float vector in the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _._ |
| virtual void | [**SetFloat4**](#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) Value) override const<br>_This function sets a float vector of size 4 by name._  |
| virtual void | [**SetInt**](#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) override const<br>_This function sets an integer uniform in the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _._ |
| virtual void | [**SetMat3**](#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) override const<br>_This function sets a 3x3 matrix with the given name._  |
| virtual void | [**SetMat4**](#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Matrix) override const<br>_Set a 4x4 matrix uniform in the shader._  |
| virtual void | [**Unbind**](#function-unbind) () override const<br>_This function unbinds the current shader program from use, setting the context to that of the default OpenGL state._  |
|  void | [**UploadFloat**](#function-uploadfloat) (const char \* Name, float Values) const<br>_Uploads a single floating-point value to the GPU._  |
|  void | [**UploadFloat2**](#function-uploadfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values) const<br>_Uploads a 2D float vector to the GPU._  |
|  void | [**UploadFloat3**](#function-uploadfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values) const<br>_Uploads a 3-component float vector to the GPU._  |
|  void | [**UploadFloat4**](#function-uploadfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Values) const<br>_Uploads a 4-component vector to the GPU._  |
|  void | [**UploadInt**](#function-uploadint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const<br>_Uploads an integer uniform to the OpenGL shader._  |
|  void | [**UploadMat3**](#function-uploadmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const<br>_Uploads a 3x3 matrix to the GPU shader program._  |
|  void | [**UploadMat4**](#function-uploadmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Matrix) const<br>_Uploads a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _to the OpenGL shader._ |
| virtual  | [**~OpenGLShader**](#function-openglshader) () <br>_Destructor for the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _class._ |


## Public Functions inherited from AGE::Shader

See [AGE::Shader](class_a_g_e_1_1_shader.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](class_a_g_e_1_1_shader.md#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetRendererID**](class_a_g_e_1_1_shader.md#function-getrendererid) () const = 0<br> |
| virtual const std::string & | [**GetShaderName**](class_a_g_e_1_1_shader.md#function-getshadername) () const = 0<br> |
| virtual void | [**SetFloat**](class_a_g_e_1_1_shader.md#function-setfloat) (const char \* Name, float Values) const = 0<br> |
| virtual void | [**SetFloat2**](class_a_g_e_1_1_shader.md#function-setfloat2) (const char \* Name, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Values) const = 0<br> |
| virtual void | [**SetFloat3**](class_a_g_e_1_1_shader.md#function-setfloat3) (const char \* Name, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values) const = 0<br> |
| virtual void | [**SetFloat4**](class_a_g_e_1_1_shader.md#function-setfloat4) (const char \* Name, const [**Vector4**](struct_a_g_e_1_1_vector4.md) Value) const = 0<br> |
| virtual void | [**SetInt**](class_a_g_e_1_1_shader.md#function-setint) (const char \* Name, const int Texture=0, const int \* TexturePtr=nullptr, const int Count=2) const = 0<br> |
| virtual void | [**SetMat3**](class_a_g_e_1_1_shader.md#function-setmat3) (const char \* Name, const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & Matrix) const = 0<br> |
| virtual void | [**SetMat4**](class_a_g_e_1_1_shader.md#function-setmat4) (const char \* Name, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Matrix) const = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_shader.md#function-unbind) () const = 0<br> |
| virtual  | [**~Shader**](class_a_g_e_1_1_shader.md#function-shader) () <br>_Virtual destructor for the_ [_**Shader**_](class_a_g_e_1_1_shader.md) _class._ |




## Public Static Functions inherited from AGE::Shader

See [AGE::Shader](class_a_g_e_1_1_shader.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-13) (const std::string & VertexSrcPath, const std::string & FragmentSrcPath) <br>_Creates a new shader object based on the current renderer's API._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-23) (const std::string & FilePath) <br>_Creates a shader object based on the current renderer API._  |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**Create**](class_a_g_e_1_1_shader.md#function-create-33) (const std::string & Name, const std::string & VertexSrc, const std::string & FragmentSrc) <br>_Creates a new shader object._  |


















































## Public Functions Documentation




### function Bind 

_This function binds the OpenGL shader program._ 
```C++
virtual void AGE::OpenGLShader::Bind () override const
```



It uses the `glUseProgram` function to bind the shader program with the given renderer ID. The function does not return any value, so it is a void function.


This function binds the OpenGL shader program.


It uses the glUseProgram function to bind this shader program, setting it as the current active program in the OpenGL context. The m\_RendererID member variable is used as an argument for this function call. 


        
Implements [*AGE::Shader::Bind*](class_a_g_e_1_1_shader.md#function-bind)


<hr>



### function Compile 

```C++
void AGE::OpenGLShader::Compile (
    const std::unordered_map< GLenum, std::string > & ShaderSources
) 
```



Compiles a collection of OpenGL shaders into a single program. The function takes in a map where each key-value pair represents the type and source code of a shader. If any compilation errors occur, they are logged and the function returns without further action. 

**Parameters:**


* `ShaderSources` A dictionary mapping GLenum (representing shader type) to string (source code). Maximum 4 shaders supported. 




        

<hr>



### function GetRendererID 

_Returns the unique identifier for the renderer._ 
```C++
inline virtual uint32_t AGE::OpenGLShader::GetRendererID () override const
```



This function returns a constant unsigned integer representing the unique ID of the renderer. It is an overridden virtual function from its base class, indicating that it provides a specific implementation for this method.




**Returns:**

A constant unsigned integer representing the renderer's ID.


This function returns the renderer ID of the object. 

**Returns:**

The renderer ID as a uint32\_t value. 





        
Implements [*AGE::Shader::GetRendererID*](class_a_g_e_1_1_shader.md#function-getrendererid)


<hr>



### function GetShaderName 

_Returns the name of the shader._ 
```C++
inline virtual const std::string & AGE::OpenGLShader::GetShaderName () override const
```





**Returns:**

A constant reference to a string containing the name of the shader.


Returns the name of the shader. 

**Returns:**

A constant reference to a string containing the name of the shader. 





        
Implements [*AGE::Shader::GetShaderName*](class_a_g_e_1_1_shader.md#function-getshadername)


<hr>



### function OpenGLShader [1/3]

_Constructs an_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _object from a file path._
```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & FilePath
) 
```



Constructor for [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) class. It takes a file path as input and reads the shader source code from it. The source code is then preprocessed and compiled into separate shaders. 

**Parameters:**


* `FilePath` A string representing the file path of the shader source code. This should be in the format "Assets/Shaders/Something.vsfs". 

This constructor reads and preprocesses the shader source code, compiles each type of shader, links them together, and extracts the name of the shader from the file path. 

**Parameters:**


* `FilePath` The path to the shader source code file. 




        

<hr>



### function OpenGLShader [2/3]

_Constructor for_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _class. Initializes an instance by reading shader sources from files specified by their paths, compiling them into a program that can be used in OpenGL rendering, and assigning a name derived from the input paths._
```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & VertexSrcPath,
    const std::string & FragmentSrcPath
) 
```





**Parameters:**


* `VertexSrcPath` The path to the vertex shader source file. 
* `FragmentSrcPath` The path to the fragment shader source file.

Constructor for [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) class.


This constructor takes in two strings representing the file paths of vertex and fragment shaders respectively. It reads these files into an unordered map with keys GL\_VERTEX\_SHADER and GL\_FRAGMENT\_SHADER, then compiles them using the Compile function. The name of the shader is extracted from the input file path and stored in m\_ShaderName.




**Parameters:**


* `VertexSrcPath` File path to vertex shader source code. 
* `FragmentSrcPath` File path to fragment shader source code. 




        

<hr>



### function OpenGLShader [3/3]

_Constructs an_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _object with the given name, vertex source code and fragment source code._
```C++
AGE::OpenGLShader::OpenGLShader (
    const std::string & Name,
    const std::string & VertexSrc,
    const std::string & FragmentSrc
) 
```



This function initializes an instance of [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) with a specified name and shader sources for both vertex and fragment stages. The sources are passed as strings to the Compile method which handles the actual compilation process.




**Parameters:**


* `Name` The name of the shader program. 
* `VertexSrc` A string containing the source code for the vertex shader stage. 
* `FragmentSrc` A string containing the source code for the fragment shader stage.

Constructs an [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) object with the given name, vertex source code and fragment source code.


This function initializes an instance of [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) by setting its shader name to the provided name, and compiling both a vertex and a fragment shader from the provided source codes. The sources are expected to be strings containing GLSL (OpenGL Shading Language) code.




**Parameters:**


* `Name` The name of the shader program. 
* `VertexSrc` A string containing the GLSL code for the vertex shader. 
* `FragmentSrc` A string containing the GLSL code for the fragment shader. 




        

<hr>



### function PreProcess 

_Preprocesses OpenGL shader source code to separate different types of shaders based on specific token._ 
```C++
std::unordered_map< GLenum, std::string > AGE::OpenGLShader::PreProcess (
    const std::string & Source
) 
```



Preprocesses an OpenGL shader source code, separating it into different sections based on type (vertex, fragment, etc.). The function takes in a string of source code and returns an unordered map where each key is a GLenum representing the shader type and each value is the corresponding shader source code. It uses a specific token (#type) to identify different sections within the source code. 




**Parameters:**


* `Source` Original source code of the shader program. 



**Returns:**

Unordered map where keys are GLenum representing shader types and values are strings containing corresponding shader sources. 





        

<hr>



### function ReadFile 

_Reads a file from the disk and returns its content as a string._ 
```C++
std::string AGE::OpenGLShader::ReadFile (
    const std::string FilePath
) 
```



This function opens a file at the given path, reads its contents into a string, and then closes the file. If the file cannot be opened for any reason (e.g., it does not exist), an error message is logged to the console.




**Parameters:**


* `FilePath` The path of the file to read. 



**Returns:**

A string containing the contents of the file, or "Unknown" if the file could not be opened.


Reads a file from the disk and returns its content as a string.


This function opens a file at the given path, reads its entire contents into a string, and then closes the file. If the file cannot be opened for any reason (e.g., it does not exist), an error message is logged to the console. 

**Parameters:**


* `FilePath` The path of the file to read from. 



**Returns:**

A string containing the content of the file. If the file could not be opened, this will be an empty string. 





        

<hr>



### function SetFloat 

_This function sets a single floating-point value with the given name._ 
```C++
virtual void AGE::OpenGLShader::SetFloat (
    const char * Name,
    float Values
) override const
```





**Parameters:**


* `Name` The name of the float variable to set. 
* `Values` The new value for the float variable.



**Returns:**

None


This function sets a single floating-point value with the given name. 

**Parameters:**


* `Name` The name of the float variable to set. 
* `Values` The new value for the float variable. 



**Returns:**

void 





        
Implements [*AGE::Shader::SetFloat*](class_a_g_e_1_1_shader.md#function-setfloat)


<hr>



### function SetFloat2 

_This function sets a float vector of two elements with the given name._ 
```C++
virtual void AGE::OpenGLShader::SetFloat2 (
    const char * Name,
    const Vector2 & Values
) override const
```





**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Values` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object containing the values to be set for the uniform variable.



**Returns:**

void


This function sets a float vector of two elements with the given name.




**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Values` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object containing the values to be set for the uniform variable.



**Returns:**

void 





        
Implements [*AGE::Shader::SetFloat2*](class_a_g_e_1_1_shader.md#function-setfloat2)


<hr>



### function SetFloat3 

_This function sets a float vector in the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _._
```C++
virtual void AGE::OpenGLShader::SetFloat3 (
    const char * Name,
    const Vector3 & Values
) override const
```





**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Values` The [**Vector3**](struct_a_g_e_1_1_vector3.md) value to be uploaded.



**Returns:**

void


This function sets a float vector of length 3.




**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Values` The [**Vector3**](struct_a_g_e_1_1_vector3.md) object containing the new values for the uniform variable.



**Returns:**

void 





        
Implements [*AGE::Shader::SetFloat3*](class_a_g_e_1_1_shader.md#function-setfloat3)


<hr>



### function SetFloat4 

_This function sets a float vector of size 4 by name._ 
```C++
virtual void AGE::OpenGLShader::SetFloat4 (
    const char * Name,
    const Vector4 Value
) override const
```





**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Value` The [**Vector4**](struct_a_g_e_1_1_vector4.md) value to be set.



**Returns:**

void


This function sets a float vector of size 4 in the [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) object.




**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Value` The [**Vector4**](struct_a_g_e_1_1_vector4.md) value to be set for the uniform variable.



**Returns:**

void 





        
Implements [*AGE::Shader::SetFloat4*](class_a_g_e_1_1_shader.md#function-setfloat4)


<hr>



### function SetInt 

_This function sets an integer uniform in the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _._
```C++
virtual void AGE::OpenGLShader::SetInt (
    const char * Name,
    const int Texture=0,
    const int * TexturePtr=nullptr,
    const int Count=2
) override const
```





**Parameters:**


* `Name` The name of the uniform to set. 
* [**Texture**](class_a_g_e_1_1_texture.md) The texture unit number to bind to the uniform. 
* `TexturePtr` Pointer to array of texture units to bind to the uniform. 
* `Count` Number of elements in the TexturePtr array.



**Returns:**

void


This function sets an integer uniform in the OpenGL shader.




**Parameters:**


* `Name` The name of the uniform variable to set. 
* [**Texture**](class_a_g_e_1_1_texture.md) The texture unit number to bind. 
* `TexturePtr` Pointer to the array of texture units to bind. 
* `Count` Number of elements in the TexturePtr array. 




        
Implements [*AGE::Shader::SetInt*](class_a_g_e_1_1_shader.md#function-setint)


<hr>



### function SetMat3 

_This function sets a 3x3 matrix with the given name._ 
```C++
virtual void AGE::OpenGLShader::SetMat3 (
    const char * Name,
    const Matrix3D & Matrix
) override const
```





**Parameters:**


* `Name` The name of the uniform variable to set in the shader program. 
* `Matrix` The 3x3 matrix to be uploaded.



**Returns:**

void


This function sets a 3x3 matrix with the given name and value.




**Parameters:**


* `Name` The name of the uniform variable to set in the shader program. 
* `Matrix` The 3x3 matrix to be uploaded.



**Returns:**

void 





        
Implements [*AGE::Shader::SetMat3*](class_a_g_e_1_1_shader.md#function-setmat3)


<hr>



### function SetMat4 

_Set a 4x4 matrix uniform in the shader._ 
```C++
virtual void AGE::OpenGLShader::SetMat4 (
    const char * Name,
    const Matrix4D Matrix
) override const
```



This function sets a 4x4 matrix uniform with the given name and value in the [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) object. The matrix is uploaded to the GPU for use by the shaders.




**Parameters:**


* `Name` The name of the uniform variable to set. 
* `Matrix` The 4x4 matrix to upload.



**Returns:**

void


This function sets a matrix of type [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) with the given name. 

**Parameters:**


* `Name` The name of the uniform variable to set in the shader program. 
* `Matrix` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object that will be uploaded to the GPU. 



**Returns:**

void 





        
Implements [*AGE::Shader::SetMat4*](class_a_g_e_1_1_shader.md#function-setmat4)


<hr>



### function Unbind 

_This function unbinds the current shader program from use, setting the context to that of the default OpenGL state._ 
```C++
virtual void AGE::OpenGLShader::Unbind () override const
```





**Returns:**

void


This function unbinds the current shader program from use by binding to 0 (the null program). 

**Returns:**

void 





        
Implements [*AGE::Shader::Unbind*](class_a_g_e_1_1_shader.md#function-unbind)


<hr>



### function UploadFloat 

_Uploads a single floating-point value to the GPU._ 
```C++
void AGE::OpenGLShader::UploadFloat (
    const char * Name,
    float Values
) const
```



This function uploads a single float value to the GPU using OpenGL's glUniform1f function. It does this by first obtaining the location of the uniform variable in the shader program with glGetUniformLocation, and then passing that location along with the float value to be uploaded to the GPU.




**Parameters:**


* `Name` The name of the uniform variable in the shader program. 
* `Values` The single floating-point value to upload to the GPU.



**Returns:**

void


Uploads a single floating-point value to the GPU.


This function uploads a single float value to the GPU using OpenGL's glUniform1f function. The location of the uniform variable is determined by calling glGetUniformLocation with the shader program and the name of the uniform variable as arguments.




**Parameters:**


* `Name` A string representing the name of the uniform variable in the shader program. 
* `Values` The float value to be uploaded to the GPU. 




        

<hr>



### function UploadFloat2 

_Uploads a 2D float vector to the GPU._ 
```C++
void AGE::OpenGLShader::UploadFloat2 (
    const char * Name,
    const Vector2 & Values
) const
```



This function uploads a 2D float vector to the GPU using OpenGL's glUniform2f and glGetUniformLocation functions. The uniform location is determined by the provided name, which should correspond to an existing uniform in the shader program.




**Parameters:**


* `Name` A string representing the name of the uniform variable in the shader program. 
* `Values` A [**Vector2**](struct_a_g_e_1_1_vector2.md) object containing the 2D float values to be uploaded.

Uploads a 2-component float vector to the GPU.


This function uploads a two component floating point vector to the GPU at the location specified by Name. The values of the vector are passed as separate arguments, Values[0] and Values[1].




**Parameters:**


* `Name` The name of the uniform variable in the shader program. 
* `Values` A 2-component float vector containing the new value for the uniform variable. 




        

<hr>



### function UploadFloat3 

_Uploads a 3-component float vector to the GPU._ 
```C++
void AGE::OpenGLShader::UploadFloat3 (
    const char * Name,
    const Vector3 & Values
) const
```



This function uploads a three component floating point vector to the GPU, which can be used for various shader operations such as light positioning or material properties. The uniform location is obtained using the provided name and uploaded to the GPU using `glUniform3f`.




**Parameters:**


* `Name` A string representing the name of the uniform variable in the shader program. 
* `Values` A 3-component floating point vector containing the values to be uploaded.

Uploads a 3-component floating point vector to the GPU.


This function uploads a three component floating point vector to the GPU, which can be used for various shader operations such as light positioning or material properties.




**Parameters:**


* `Name` The name of the uniform variable in the shader program. 
* `Values` A 3-component floating point vector containing the values to upload. 




        

<hr>



### function UploadFloat4 

_Uploads a 4-component vector to the GPU._ 
```C++
void AGE::OpenGLShader::UploadFloat4 (
    const char * Name,
    const Vector4 & Values
) const
```



This function uploads a 4-component vector (represented by a [**Vector4**](struct_a_g_e_1_1_vector4.md) object) to the GPU, using OpenGL's glUniform4f function. The location of the uniform variable on the GPU is determined by the provided name string.




**Parameters:**


* `Name` A pointer to a null-terminated string representing the name of the uniform variable in the shader program. 
* `Values` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object containing the 4 components of the vector to be uploaded.

Uploads a 4-component vector to the GPU as a uniform variable.


This function uploads a 4-component vector (x, y, z, w) to the GPU as a uniform variable with the specified name. The location of this uniform is obtained using `glGetUniformLocation`.




**Parameters:**


* `Name` A string representing the name of the uniform variable on the GPU. 
* `Values` A 4-component vector containing the values to be uploaded. 




        

<hr>



### function UploadInt 

_Uploads an integer uniform to the OpenGL shader._ 
```C++
void AGE::OpenGLShader::UploadInt (
    const char * Name,
    const int Texture=0,
    const int * TexturePtr=nullptr,
    const int Count=2
) const
```



This function uploads a single integer or an array of integers as a uniform variable in the OpenGL shader program. It first checks if the `TexturePtr` parameter is not null, and if so, it uses `glUniform1iv()` to set the uniform value using the pointer to the data. If `TexturePtr` is null, it simply sets the single integer uniform with `glUniform1i()`.




**Parameters:**


* `Name` The name of the uniform variable in the shader program. 
* [**Texture**](class_a_g_e_1_1_texture.md) A single integer value to be uploaded as a uniform. 
* `TexturePtr` Pointer to an array of integers to be uploaded as uniforms. If this is null, `Texture` will be used instead. 
* `Count` The number of elements in the `TexturePtr` array if it's not null. This parameter is ignored if `TexturePtr` is null.

Uploads an integer uniform to the OpenGL shader.


This function uploads a single integer or an array of integers to the specified uniform variable in the OpenGL shader. The location of the uniform is determined by its name, which must be valid and existent within the shader program. If TexturePtr is not null, it will use glUniform1iv to upload Count number of integer values from TexturePtr array. Otherwise, it will simply upload a single integer value using glUniform1i. 

**Parameters:**


* `Name` The name of the uniform variable in the shader program. 
* [**Texture**](class_a_g_e_1_1_texture.md) A single integer value to be uploaded. 
* `TexturePtr` Pointer to an array of integers to be uploaded. If this is null, only a single integer will be uploaded. 
* `Count` Number of elements in the TexturePtr array if it's not null. This parameter has no effect if TexturePtr is null. 




        

<hr>



### function UploadMat3 

_Uploads a 3x3 matrix to the GPU shader program._ 
```C++
void AGE::OpenGLShader::UploadMat3 (
    const char * Name,
    const Matrix3D & Matrix
) const
```



This function uploads a 3x3 matrix to the GPU shader program using OpenGL's glUniformMatrix3fv function. The location of the uniform variable in the shader is determined by calling glGetUniformLocation with the name of the uniform and the ID of the shader program.




**Parameters:**


* `Name` A string representing the name of the uniform variable in the shader program. 
* `Matrix` A 3x3 matrix to be uploaded to the GPU.

Uploads a 3x3 matrix to the GPU shader program.


This function uploads a 3x3 matrix to the GPU shader program using OpenGL's glUniformMatrix3fv function. The location of the uniform variable in the shader program is obtained by calling glGetUniformLocation with the name of the uniform and the ID of the shader program.




**Parameters:**


* `Name` A string representing the name of the uniform variable in the shader program. 
* `Matrix` A 3x3 matrix to be uploaded to the GPU. 




        

<hr>



### function UploadMat4 

_Uploads a_ [_**Matrix4D**_](struct_a_g_e_1_1_matrix4_d.md) _to the OpenGL shader._
```C++
void AGE::OpenGLShader::UploadMat4 (
    const char * Name,
    const Matrix4D & Matrix
) const
```



This function uploads a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to an OpenGL shader by first getting the location of the uniform variable in the shader using glGetUniformLocation, then passing the matrix data to this location with glUniformMatrix4fv.




**Parameters:**


* `Name` The name of the uniform variable in the shader. 
* `Matrix` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be uploaded.

Uploads a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to the OpenGL shader.


This function uploads a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to an OpenGL shader by first getting the uniform location of the variable in the shader, and then using glUniformMatrix4fv to set the value of that variable. The matrix is uploaded as a raw float array.




**Parameters:**


* `Name` The name of the [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) variable in the shader. 
* `Matrix` The [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) to be uploaded. 




        

<hr>



### function ~OpenGLShader 

_Destructor for the_ [_**OpenGLShader**_](class_a_g_e_1_1_open_g_l_shader.md) _class._
```C++
virtual AGE::OpenGLShader::~OpenGLShader () 
```



This function deletes a shader program from the GPU using glDeleteProgram(). The ID of the shader program to delete is stored in m\_RendererID.


Destructor for the [**OpenGLShader**](class_a_g_e_1_1_open_g_l_shader.md) class.


This function deletes a shader program from the GPU using glDeleteProgram(). The ID of the shader program to delete is stored in m\_RendererID. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLShader.h`

