

# Class AGE::OpenGLIndexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLIndexBuffer**](class_a_g_e_1_1_open_g_l_index_buffer.md)








Inherits the following classes: [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override const<br> |
| virtual uint32\_t | [**GetCount**](#function-getcount) () override<br> |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () override const<br> |
|   | [**OpenGLIndexBuffer**](#function-openglindexbuffer) (uint32\_t \* Indices, uint32\_t Size) <br> |
| virtual void | [**Unbind**](#function-unbind) () override const<br> |
| virtual  | [**~OpenGLIndexBuffer**](#function-openglindexbuffer) () <br> |


## Public Functions inherited from AGE::IndexBuffer

See [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_index_buffer.md#function-as) () <br> |
| virtual void | [**Bind**](class_a_g_e_1_1_index_buffer.md#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetCount**](class_a_g_e_1_1_index_buffer.md#function-getcount) () = 0<br> |
| virtual void | [**InvalidateBuffer**](class_a_g_e_1_1_index_buffer.md#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_index_buffer.md#function-unbind) () const = 0<br> |
| virtual  | [**~IndexBuffer**](class_a_g_e_1_1_index_buffer.md#function-indexbuffer) () <br> |




## Public Static Functions inherited from AGE::IndexBuffer

See [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_index_buffer.md#function-create) (uint32\_t \* Indices, uint32\_t Count) <br> |


















































## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::OpenGLIndexBuffer::Bind () override const
```



Implements [*AGE::IndexBuffer::Bind*](class_a_g_e_1_1_index_buffer.md#function-bind)


<hr>



### function GetCount 

```C++
inline virtual uint32_t AGE::OpenGLIndexBuffer::GetCount () override
```



Implements [*AGE::IndexBuffer::GetCount*](class_a_g_e_1_1_index_buffer.md#function-getcount)


<hr>



### function InvalidateBuffer 

```C++
virtual void AGE::OpenGLIndexBuffer::InvalidateBuffer () override const
```



Implements [*AGE::IndexBuffer::InvalidateBuffer*](class_a_g_e_1_1_index_buffer.md#function-invalidatebuffer)


<hr>



### function OpenGLIndexBuffer 

```C++
AGE::OpenGLIndexBuffer::OpenGLIndexBuffer (
    uint32_t * Indices,
    uint32_t Size
) 
```




<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLIndexBuffer::Unbind () override const
```



Implements [*AGE::IndexBuffer::Unbind*](class_a_g_e_1_1_index_buffer.md#function-unbind)


<hr>



### function ~OpenGLIndexBuffer 

```C++
virtual AGE::OpenGLIndexBuffer::~OpenGLIndexBuffer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

