

# Class AGE::OpenGLUniformBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md)








Inherits the following classes: [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override<br>_Bind the uniform buffer to a specific binding point in the GPU's memory._  |
|   | [**OpenGLUniformBuffer**](#function-opengluniformbuffer) (uint32\_t Size, uint32\_t Binding) <br>_Constructor for_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _. Creates a new uniform buffer object with the specified size and binding point._ |
| virtual void | [**SetData**](#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) override<br>_This function sets the data of an OpenGL uniform buffer._  |
| virtual void | [**Unbind**](#function-unbind) () override<br>_Unbind function for the_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _class. This function sets the buffer to an unbound state, meaning it is no longer bound to a target._ |
| virtual  | [**~OpenGLUniformBuffer**](#function-opengluniformbuffer) () <br>_Destructor for the_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _class. This function deletes a buffer object from OpenGL using glDeleteBuffers(). The buffer to be deleted is specified by its ID, which is stored in m\_RendererID member variable of this instance._ |


## Public Functions inherited from AGE::UniformBuffer

See [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_uniform_buffer.md#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
| virtual void | [**Bind**](class_a_g_e_1_1_uniform_buffer.md#function-bind) () = 0<br> |
| virtual void | [**SetData**](class_a_g_e_1_1_uniform_buffer.md#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_uniform_buffer.md#function-unbind) () = 0<br> |
| virtual  | [**~UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md#function-uniformbuffer) () <br>_Virtual destructor for the_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _class._ |




## Public Static Functions inherited from AGE::UniformBuffer

See [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_uniform_buffer.md#function-create) (uint32\_t Size, uint32\_t Binding) <br>_Creates a new_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _instance._ |


















































## Public Functions Documentation




### function Bind 

_Bind the uniform buffer to a specific binding point in the GPU's memory._ 
```C++
virtual void AGE::OpenGLUniformBuffer::Bind () override
```



This function binds the uniform buffer object (UBO) to a specific binding point in the OpenGL context. The UBO is essentially an array of uniform variables that can be accessed by shaders.




**Returns:**

void No return value.


Bind the uniform buffer to a specific binding point in the GPU's memory.


This function binds the uniform buffer object (UBO) to a specific binding point in the GPU's memory. The binding point is specified by an integer argument, 'bindingPoint'. It allows data to be sent to shaders for rendering without having to re-upload it every frame.




**Parameters:**


* `bindingPoint` An integer specifying the binding point in the GPU's memory where the UBO should be bound. 




        
Implements [*AGE::UniformBuffer::Bind*](class_a_g_e_1_1_uniform_buffer.md#function-bind)


<hr>



### function OpenGLUniformBuffer 

_Constructor for_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _. Creates a new uniform buffer object with the specified size and binding point._
```C++
AGE::OpenGLUniformBuffer::OpenGLUniformBuffer (
    uint32_t Size,
    uint32_t Binding
) 
```





**Parameters:**


* `Size` The size of the buffer in bytes. 
* `Binding` The binding point for this buffer, which determines its location in the shader program.

Constructor for [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md). Initializes an OpenGL uniform buffer object with the specified size and binding point.




**Parameters:**


* `Size` The size of the buffer in bytes. 
* `Binding` The binding point for this buffer, which determines its location in the shader program. 




        

<hr>



### function SetData 

_This function sets the data of an OpenGL uniform buffer._ 
```C++
virtual void AGE::OpenGLUniformBuffer::SetData (
    const void * Data,
    uint32_t Size,
    uint32_t Offset=0
) override
```





**Parameters:**


* `Data` A pointer to the data that will be copied into the named buffer's data store. 
* `Size` The size in bytes of the data being uploaded. 
* `Offset` The offset in bytes from the beginning of the buffer where the new data will be placed.



**Returns:**

void


This function sets the data of an OpenGL uniform buffer.




**Parameters:**


* `Data` A pointer to the data that will be copied into the named buffer's data store. 
* `Size` The size in bytes of the region of the buffer object that is being replaced. 
* `Offset` The offset, in basic machine units, within the buffer object where the replacement will begin. 




        
Implements [*AGE::UniformBuffer::SetData*](class_a_g_e_1_1_uniform_buffer.md#function-setdata)


<hr>



### function Unbind 

_Unbind function for the_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _class. This function sets the buffer to an unbound state, meaning it is no longer bound to a target._
```C++
virtual void AGE::OpenGLUniformBuffer::Unbind () override
```





**Returns:**

void


Unbind function for the [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md) class. This function is used to unbind any buffer that has been bound in the current context. It sets the uniform binding point back to its default state, which is zero.




**Returns:**

void 





        
Implements [*AGE::UniformBuffer::Unbind*](class_a_g_e_1_1_uniform_buffer.md#function-unbind)


<hr>



### function ~OpenGLUniformBuffer 

_Destructor for the_ [_**OpenGLUniformBuffer**_](class_a_g_e_1_1_open_g_l_uniform_buffer.md) _class. This function deletes a buffer object from OpenGL using glDeleteBuffers(). The buffer to be deleted is specified by its ID, which is stored in m\_RendererID member variable of this instance._
```C++
virtual AGE::OpenGLUniformBuffer::~OpenGLUniformBuffer () 
```





**Returns:**

void


Destructor for the [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md) class. This function deletes a buffer object from OpenGL using glDeleteBuffers(). The buffer to be deleted is specified by its ID, which is stored in m\_RendererID member variable of this instance. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

