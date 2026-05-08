

# Class AGE::OpenGLUniformBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md)








Inherits the following classes: [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override<br> |
|   | [**OpenGLUniformBuffer**](#function-opengluniformbuffer) (uint32\_t Size, uint32\_t Binding) <br> |
| virtual void | [**SetData**](#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) override<br> |
| virtual void | [**Unbind**](#function-unbind) () override<br> |
| virtual  | [**~OpenGLUniformBuffer**](#function-opengluniformbuffer) () <br> |


## Public Functions inherited from AGE::UniformBuffer

See [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_uniform_buffer.md#function-as) () <br> |
| virtual void | [**Bind**](class_a_g_e_1_1_uniform_buffer.md#function-bind) () = 0<br> |
| virtual void | [**SetData**](class_a_g_e_1_1_uniform_buffer.md#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_uniform_buffer.md#function-unbind) () = 0<br> |
| virtual  | [**~UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md#function-uniformbuffer) () <br> |




## Public Static Functions inherited from AGE::UniformBuffer

See [AGE::UniformBuffer](class_a_g_e_1_1_uniform_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_uniform_buffer.md#function-create) (uint32\_t Size, uint32\_t Binding) <br> |


















































## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::OpenGLUniformBuffer::Bind () override
```



Implements [*AGE::UniformBuffer::Bind*](class_a_g_e_1_1_uniform_buffer.md#function-bind)


<hr>



### function OpenGLUniformBuffer 

```C++
AGE::OpenGLUniformBuffer::OpenGLUniformBuffer (
    uint32_t Size,
    uint32_t Binding
) 
```




<hr>



### function SetData 

```C++
virtual void AGE::OpenGLUniformBuffer::SetData (
    const void * Data,
    uint32_t Size,
    uint32_t Offset=0
) override
```



Implements [*AGE::UniformBuffer::SetData*](class_a_g_e_1_1_uniform_buffer.md#function-setdata)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLUniformBuffer::Unbind () override
```



Implements [*AGE::UniformBuffer::Unbind*](class_a_g_e_1_1_uniform_buffer.md#function-unbind)


<hr>



### function ~OpenGLUniformBuffer 

```C++
virtual AGE::OpenGLUniformBuffer::~OpenGLUniformBuffer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

