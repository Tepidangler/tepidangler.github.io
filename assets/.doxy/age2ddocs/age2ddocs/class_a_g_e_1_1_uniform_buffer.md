

# Class AGE::UniformBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md)










Inherited by the following classes: [AGE::OpenGLUniformBuffer](class_a_g_e_1_1_open_g_l_uniform_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
| virtual void | [**Bind**](#function-bind) () = 0<br> |
| virtual void | [**SetData**](#function-setdata) (const void \* Data, uint32\_t Size, uint32\_t Offset=0) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () = 0<br> |
| virtual  | [**~UniformBuffer**](#function-uniformbuffer) () <br>_Virtual destructor for the_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**Create**](#function-create) (uint32\_t Size, uint32\_t Binding) <br>_Creates a new_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _instance._ |


























## Public Functions Documentation




### function As 

_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._ 
```C++
template<typename T>
T * AGE::UniformBuffer::As () 
```





**Returns:**

A null pointer of type T\*


This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown.




**Returns:**

Returns a null pointer of type T\* 





        

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

_Virtual destructor for the_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _class._
```C++
inline virtual AGE::UniformBuffer::~UniformBuffer () 
```



This function is responsible for releasing any resources that were acquired by the [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) object, such as memory or GPU resources. It does not return anything and thus has an empty return type (void). 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new_ [_**UniformBuffer**_](class_a_g_e_1_1_uniform_buffer.md) _instance._
```C++
static Ref< UniformBuffer > AGE::UniformBuffer::Create (
    uint32_t Size,
    uint32_t Binding
) 
```



This function creates and initializes a new [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) object of the specified size and binding point. The type of buffer to be created is determined by the current [**Renderer**](class_a_g_e_1_1_renderer.md) API in use. If OpenGL is currently being used, an [**OpenGLUniformBuffer**](class_a_g_e_1_1_open_g_l_uniform_buffer.md) will be created; otherwise, if no supported API is found, null is returned.




**Parameters:**


* `Size` The size (in bytes) of the [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) to create. 
* `Binding` The binding point for the [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) in the shader program.



**Returns:**

A reference to a new [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) object if successful, nullptr otherwise.


Creates a new uniform buffer.


This function creates and initializes a new [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) object of the specified size and binding point. The type of the underlying implementation is determined by the current [**Renderer**](class_a_g_e_1_1_renderer.md) API in use.




**Parameters:**


* `Size` The size of the uniform buffer, in bytes. 
* `Binding` The binding point for this uniform buffer. This determines which shader program can access it.



**Returns:**

A reference to a new [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) object. If an unsupported [**Renderer**](class_a_g_e_1_1_renderer.md) API is detected or if there are issues with creating the buffer, nullptr is returned instead. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

