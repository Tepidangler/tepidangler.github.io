

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
| virtual  | [**~VertexArray**](#function-vertexarray) () <br>_Virtual destructor for the_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**Create**](#function-create) () <br>_Creates a new_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _object based on the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._ |


























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

_Virtual destructor for the_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _class._
```C++
inline virtual AGE::VertexArray::~VertexArray () 
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or GPU resources. It does not return anything and thus has an empty return type (void).


Virtual destructor for the [**VertexArray**](class_a_g_e_1_1_vertex_array.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or GPU resources. It does not perform any operations on the actual data stored in the array. 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _object based on the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._
```C++
static Ref< VertexArray > AGE::VertexArray::Create () 
```



This function creates and returns a reference to a new [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object, which is specific to the currently used [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md). If the API is not supported or unknown, it asserts false and returns nullptr.




**Returns:**

Ref&lt;VertexArray&gt; A reference to the newly created [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object.


Creates a new [**VertexArray**](class_a_g_e_1_1_vertex_array.md) based on the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md).


This function creates and returns a reference to a new [**VertexArray**](class_a_g_e_1_1_vertex_array.md) object, which is specific to the currently used [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md). If no supported API is found, it asserts false and returns nullptr.




**Returns:**

Ref&lt;VertexArray&gt; A reference to the newly created [**VertexArray**](class_a_g_e_1_1_vertex_array.md). 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/VertexArray.h`

