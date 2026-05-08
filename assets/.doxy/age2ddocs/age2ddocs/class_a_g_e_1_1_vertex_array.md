

# Class AGE::VertexArray



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**VertexArray**](class_a_g_e_1_1_vertex_array.md)










Inherited by the following classes: [AGE::OpenGLVertexArray](class_a_g_e_1_1_open_g_l_vertex_array.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddVertexBuffer**](#function-addvertexbuffer) (Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; & VertexBuffer) = 0<br> |
| virtual void | [**Bind**](#function-bind) () const = 0<br> |
| virtual void | [**EnableVertexAttribArray**](#function-enablevertexattribarray) (uint32\_t ArrayID) const = 0<br> |
| virtual const Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & | [**GetIndexBuffer**](#function-getindexbuffer) () const = 0<br> |
| virtual const std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt; & | [**GetVertexBuffers**](#function-getvertexbuffers) () const = 0<br> |
| virtual void | [**MakeVertexAttribPtr**](#function-makevertexattribptr) (uint32\_t index, int size, uint32\_t type, uint8\_t normalized, int stride, const void \* pointer) const = 0<br> |
| virtual void | [**SetIndexBuffer**](#function-setindexbuffer) (Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & IndexBuffer) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**begin**](#function-begin-12) () = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**begin**](#function-begin-22) () const = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**end**](#function-end-12) () = 0<br> |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**end**](#function-end-22) () const = 0<br> |
| virtual  | [**~VertexArray**](#function-vertexarray) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**Create**](#function-create) () <br> |


























## Public Functions Documentation




### function AddVertexBuffer 

```C++
virtual void AGE::VertexArray::AddVertexBuffer (
    Ref< VertexBuffer > & VertexBuffer
) = 0
```




<hr>



### function Bind 

```C++
virtual void AGE::VertexArray::Bind () const = 0
```




<hr>



### function EnableVertexAttribArray 

```C++
virtual void AGE::VertexArray::EnableVertexAttribArray (
    uint32_t ArrayID
) const = 0
```




<hr>



### function GetIndexBuffer 

```C++
virtual const Ref< IndexBuffer > & AGE::VertexArray::GetIndexBuffer () const = 0
```




<hr>



### function GetVertexBuffers 

```C++
virtual const std::vector< Ref< VertexBuffer > > & AGE::VertexArray::GetVertexBuffers () const = 0
```




<hr>



### function MakeVertexAttribPtr 

```C++
virtual void AGE::VertexArray::MakeVertexAttribPtr (
    uint32_t index,
    int size,
    uint32_t type,
    uint8_t normalized,
    int stride,
    const void * pointer
) const = 0
```




<hr>



### function SetIndexBuffer 

```C++
virtual void AGE::VertexArray::SetIndexBuffer (
    Ref< IndexBuffer > & IndexBuffer
) = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::VertexArray::Unbind () const = 0
```




<hr>



### function begin [1/2]

```C++
virtual std::vector< Ref< VertexBuffer > >::iterator AGE::VertexArray::begin () = 0
```




<hr>



### function begin [2/2]

```C++
virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::VertexArray::begin () const = 0
```




<hr>



### function end [1/2]

```C++
virtual std::vector< Ref< VertexBuffer > >::iterator AGE::VertexArray::end () = 0
```




<hr>



### function end [2/2]

```C++
virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::VertexArray::end () const = 0
```




<hr>



### function ~VertexArray 

```C++
inline virtual AGE::VertexArray::~VertexArray () 
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< VertexArray > AGE::VertexArray::Create () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/VertexArray.h`

