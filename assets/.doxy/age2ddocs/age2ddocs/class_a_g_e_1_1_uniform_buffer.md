

# Class AGE::UniformBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md)










Inherited by the following classes: [AGE::OpenGLUniformBuffer](class_a_g_e_1_1_open_g_l_uniform_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br> |
| virtual void | [**Bind**](#function-bind) () = 0<br> |
| virtual void | [**SetData**](#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () = 0<br> |
| virtual  | [**~UniformBuffer**](#function-uniformbuffer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**Create**](#function-create) (uint32\_t Size, uint32\_t Binding) <br> |


























## Public Functions Documentation




### function As 

```C++
template<typename T>
T * AGE::UniformBuffer::As () 
```




<hr>



### function Bind 

```C++
virtual void AGE::UniformBuffer::Bind () = 0
```




<hr>



### function SetData 

```C++
virtual void AGE::UniformBuffer::SetData (
    const void * Data,
    uint32_t Size,
    uint32_t Offset=0
) = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::UniformBuffer::Unbind () = 0
```




<hr>



### function ~UniformBuffer 

```C++
inline virtual AGE::UniformBuffer::~UniformBuffer () 
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< UniformBuffer > AGE::UniformBuffer::Create (
    uint32_t Size,
    uint32_t Binding
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

