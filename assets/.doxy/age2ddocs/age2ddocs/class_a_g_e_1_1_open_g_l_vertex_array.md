

# Class AGE::OpenGLVertexArray



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLVertexArray**](class_a_g_e_1_1_open_g_l_vertex_array.md)








Inherits the following classes: [AGE::VertexArray](class_a_g_e_1_1_vertex_array.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddVertexBuffer**](#function-addvertexbuffer) (Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; & VertexBuffer) override<br> |
| virtual void | [**Bind**](#function-bind) () override const<br> |
| virtual void | [**EnableVertexAttribArray**](#function-enablevertexattribarray) (uint32\_t ArrayID) override const<br> |
| virtual const Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & | [**GetIndexBuffer**](#function-getindexbuffer) () override const<br> |
| virtual const std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt; & | [**GetVertexBuffers**](#function-getvertexbuffers) () override const<br> |
| virtual void | [**MakeVertexAttribPtr**](#function-makevertexattribptr) (uint32\_t index, int size, uint32\_t type, uint8\_t normalized, int stride, const void \* pointer) override const<br> |
|   | [**OpenGLVertexArray**](#function-openglvertexarray) () <br> |
| virtual void | [**SetIndexBuffer**](#function-setindexbuffer) (Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & IndexBuffer) override<br> |
| virtual void | [**Unbind**](#function-unbind) () override const<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**begin**](#function-begin-12) () override<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**begin**](#function-begin-22) () override const<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**end**](#function-end-12) () override<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**end**](#function-end-22) () override const<br> |
|   | [**~OpenGLVertexArray**](#function-openglvertexarray) () override<br> |


## Public Functions inherited from AGE::VertexArray

See [AGE::VertexArray](class_a_g_e_1_1_vertex_array.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**AddVertexBuffer**](class_a_g_e_1_1_vertex_array.md#function-addvertexbuffer) (Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; & VertexBuffer) = 0<br> |
| virtual void | [**Bind**](class_a_g_e_1_1_vertex_array.md#function-bind) () const = 0<br> |
| virtual void | [**EnableVertexAttribArray**](class_a_g_e_1_1_vertex_array.md#function-enablevertexattribarray) (uint32\_t ArrayID) const = 0<br> |
| virtual const Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & | [**GetIndexBuffer**](class_a_g_e_1_1_vertex_array.md#function-getindexbuffer) () const = 0<br> |
| virtual const std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt; & | [**GetVertexBuffers**](class_a_g_e_1_1_vertex_array.md#function-getvertexbuffers) () const = 0<br> |
| virtual void | [**MakeVertexAttribPtr**](class_a_g_e_1_1_vertex_array.md#function-makevertexattribptr) (uint32\_t index, int size, uint32\_t type, uint8\_t normalized, int stride, const void \* pointer) const = 0<br> |
| virtual void | [**SetIndexBuffer**](class_a_g_e_1_1_vertex_array.md#function-setindexbuffer) (Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & IndexBuffer) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_vertex_array.md#function-unbind) () const = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**begin**](class_a_g_e_1_1_vertex_array.md#function-begin-12) () = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**begin**](class_a_g_e_1_1_vertex_array.md#function-begin-22) () const = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**end**](class_a_g_e_1_1_vertex_array.md#function-end-12) () = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**end**](class_a_g_e_1_1_vertex_array.md#function-end-22) () const = 0<br> |
| virtual  | [**~VertexArray**](class_a_g_e_1_1_vertex_array.md#function-vertexarray) () <br> |




## Public Static Functions inherited from AGE::VertexArray

See [AGE::VertexArray](class_a_g_e_1_1_vertex_array.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_array.md#function-create) () <br> |


















































## Public Functions Documentation




### function AddVertexBuffer 

```C++
virtual void AGE::OpenGLVertexArray::AddVertexBuffer (
    Ref< VertexBuffer > & VertexBuffer
) override
```



Implements [*AGE::VertexArray::AddVertexBuffer*](class_a_g_e_1_1_vertex_array.md#function-addvertexbuffer)


<hr>



### function Bind 

```C++
virtual void AGE::OpenGLVertexArray::Bind () override const
```



Implements [*AGE::VertexArray::Bind*](class_a_g_e_1_1_vertex_array.md#function-bind)


<hr>



### function EnableVertexAttribArray 

```C++
virtual void AGE::OpenGLVertexArray::EnableVertexAttribArray (
    uint32_t ArrayID
) override const
```



Implements [*AGE::VertexArray::EnableVertexAttribArray*](class_a_g_e_1_1_vertex_array.md#function-enablevertexattribarray)


<hr>



### function GetIndexBuffer 

```C++
inline virtual const Ref< IndexBuffer > & AGE::OpenGLVertexArray::GetIndexBuffer () override const
```



Implements [*AGE::VertexArray::GetIndexBuffer*](class_a_g_e_1_1_vertex_array.md#function-getindexbuffer)


<hr>



### function GetVertexBuffers 

```C++
inline virtual const std::vector< Ref< VertexBuffer > > & AGE::OpenGLVertexArray::GetVertexBuffers () override const
```



Implements [*AGE::VertexArray::GetVertexBuffers*](class_a_g_e_1_1_vertex_array.md#function-getvertexbuffers)


<hr>



### function MakeVertexAttribPtr 

```C++
virtual void AGE::OpenGLVertexArray::MakeVertexAttribPtr (
    uint32_t index,
    int size,
    uint32_t type,
    uint8_t normalized,
    int stride,
    const void * pointer
) override const
```



Implements [*AGE::VertexArray::MakeVertexAttribPtr*](class_a_g_e_1_1_vertex_array.md#function-makevertexattribptr)


<hr>



### function OpenGLVertexArray 

```C++
AGE::OpenGLVertexArray::OpenGLVertexArray () 
```




<hr>



### function SetIndexBuffer 

```C++
virtual void AGE::OpenGLVertexArray::SetIndexBuffer (
    Ref< IndexBuffer > & IndexBuffer
) override
```



Implements [*AGE::VertexArray::SetIndexBuffer*](class_a_g_e_1_1_vertex_array.md#function-setindexbuffer)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLVertexArray::Unbind () override const
```



Implements [*AGE::VertexArray::Unbind*](class_a_g_e_1_1_vertex_array.md#function-unbind)


<hr>



### function begin [1/2]

```C++
inline virtual std::vector< Ref< VertexBuffer > >::iterator AGE::OpenGLVertexArray::begin () override
```



Implements [*AGE::VertexArray::begin*](class_a_g_e_1_1_vertex_array.md#function-begin-12)


<hr>



### function begin [2/2]

```C++
inline virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::OpenGLVertexArray::begin () override const
```



Implements [*AGE::VertexArray::begin*](class_a_g_e_1_1_vertex_array.md#function-begin-22)


<hr>



### function end [1/2]

```C++
inline virtual std::vector< Ref< VertexBuffer > >::iterator AGE::OpenGLVertexArray::end () override
```



Implements [*AGE::VertexArray::end*](class_a_g_e_1_1_vertex_array.md#function-end-12)


<hr>



### function end [2/2]

```C++
inline virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::OpenGLVertexArray::end () override const
```



Implements [*AGE::VertexArray::end*](class_a_g_e_1_1_vertex_array.md#function-end-22)


<hr>



### function ~OpenGLVertexArray 

```C++
AGE::OpenGLVertexArray::~OpenGLVertexArray () override
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLVertexArray.h`

