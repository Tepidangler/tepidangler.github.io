

# Class AGE::OpenGLVertexArray



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLVertexArray**](class_a_g_e_1_1_open_g_l_vertex_array.md)








Inherits the following classes: [AGE::VertexArray](class_a_g_e_1_1_vertex_array.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddVertexBuffer**](#function-addvertexbuffer) (Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; & VertexBuffer) override<br> |
| virtual void | [**Bind**](#function-bind) () override const<br>_This function binds the vertex array object._  |
| virtual void | [**EnableVertexAttribArray**](#function-enablevertexattribarray) (uint32\_t ArrayID) override const<br>_This function enables a vertex attribute array._  |
| virtual const Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & | [**GetIndexBuffer**](#function-getindexbuffer) () override const<br>_Returns the index buffer associated with this object._  |
| virtual const std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt; & | [**GetVertexBuffers**](#function-getvertexbuffers) () override const<br>_Returns a constant reference to the vertex buffers associated with this object._  |
| virtual void | [**MakeVertexAttribPtr**](#function-makevertexattribptr) (uint32\_t index, int size, uint32\_t type, uint8\_t normalized, int stride, const void \* pointer) override const<br>_This function sets up the vertex attribute pointer for a specific index. It takes in parameters such as size of data, type of data (GL\_FLOAT or GL\_INT), whether the data is normalized, stride and pointer to the data. The function uses glVertexAttribPointer OpenGL function to set up the vertex attribute pointer._  |
|   | [**OpenGLVertexArray**](#function-openglvertexarray) () <br> |
| virtual void | [**SetIndexBuffer**](#function-setindexbuffer) (Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; & IndexBuffer) override<br>_This function sets the index buffer for the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) _Array._ |
| virtual void | [**Unbind**](#function-unbind) () override const<br>_This function unbinds the current vertex array object._  |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**begin**](#function-begin-12) () override<br>_Returns an iterator pointing to the beginning of the vertex buffer list._  |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**begin**](#function-begin-22) () override const<br>_Returns a constant iterator pointing to the beginning of the vertex buffer list._  |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::iterator | [**end**](#function-end-12) () override<br>_Returns an iterator pointing to the theoretical element that follows the last element of the container. This function is used in range-based for loops and similar contexts where a sentinel value is needed._  |
| virtual std::vector&lt; Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt;::const\_iterator | [**end**](#function-end-22) () override const<br>_Returns a constant iterator pointing to the theoretical element past the last element of the vertex buffer vector._  |
|   | [**~OpenGLVertexArray**](#function-openglvertexarray) () override<br>_Destructor for_ [_**OpenGLVertexArray**_](class_a_g_e_1_1_open_g_l_vertex_array.md) _class. Deletes the vertex array object from GPU memory._ |


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
| virtual  | [**~VertexArray**](class_a_g_e_1_1_vertex_array.md#function-vertexarray) () <br>_Virtual destructor for the_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _class._ |




## Public Static Functions inherited from AGE::VertexArray

See [AGE::VertexArray](class_a_g_e_1_1_vertex_array.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_array.md#function-create) () <br>_Creates a new_ [_**VertexArray**_](class_a_g_e_1_1_vertex_array.md) _object based on the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._ |


















































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

_This function binds the vertex array object._ 
```C++
virtual void AGE::OpenGLVertexArray::Bind () override const
```



It uses OpenGL's glBindVertexArray() function to bind this [**Vertex**](struct_a_g_e_1_1_vertex.md) Array Object (VAO). The VAO is an object that contains all of the state needed to supply vertex data, such as what vertex arrays to use, how to interpret them, and how to render them.




**Returns:**

void 





        
Implements [*AGE::VertexArray::Bind*](class_a_g_e_1_1_vertex_array.md#function-bind)


<hr>



### function EnableVertexAttribArray 

_This function enables a vertex attribute array._ 
```C++
virtual void AGE::OpenGLVertexArray::EnableVertexAttribArray (
    uint32_t ArrayID
) override const
```





**Parameters:**


* `ArrayID` The ID of the vertex attribute array to be enabled. 



**Returns:**

void 





        
Implements [*AGE::VertexArray::EnableVertexAttribArray*](class_a_g_e_1_1_vertex_array.md#function-enablevertexattribarray)


<hr>



### function GetIndexBuffer 

_Returns the index buffer associated with this object._ 
```C++
inline virtual const Ref< IndexBuffer > & AGE::OpenGLVertexArray::GetIndexBuffer () override const
```





**Returns:**

A constant reference to the index buffer.


Returns the index buffer associated with this object. 

**Returns:**

A constant reference to the index buffer. 





        
Implements [*AGE::VertexArray::GetIndexBuffer*](class_a_g_e_1_1_vertex_array.md#function-getindexbuffer)


<hr>



### function GetVertexBuffers 

_Returns a constant reference to the vertex buffers associated with this object._ 
```C++
inline virtual const std::vector< Ref< VertexBuffer > > & AGE::OpenGLVertexArray::GetVertexBuffers () override const
```





**Returns:**

A constant reference to the vector of [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) objects.


Returns a constant reference to the vertex buffers of this object. 

**Returns:**

A constant reference to the vector of vertex buffers (m\_VertexBuffers). 





        
Implements [*AGE::VertexArray::GetVertexBuffers*](class_a_g_e_1_1_vertex_array.md#function-getvertexbuffers)


<hr>



### function MakeVertexAttribPtr 

_This function sets up the vertex attribute pointer for a specific index. It takes in parameters such as size of data, type of data (GL\_FLOAT or GL\_INT), whether the data is normalized, stride and pointer to the data. The function uses glVertexAttribPointer OpenGL function to set up the vertex attribute pointer._ 
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





**Parameters:**


* `index` The index of the generic vertex attribute to be modified. 
* `size` Specifies the number of components per generic vertex attribute. Must be 1, 2, 3, or 4. 
* `type` Specifies the data type of each component in the array. Must be GL\_FLOAT or GL\_INT. 
* `normalized` If true, the integer values are treated as a stream of normalized fixed-point values. 
* `stride` The byte offset between consecutive generic vertex attributes. 
* `pointer` Specifies a pointer to the first component of the array. 



**Returns:**

void 





        
Implements [*AGE::VertexArray::MakeVertexAttribPtr*](class_a_g_e_1_1_vertex_array.md#function-makevertexattribptr)


<hr>



### function OpenGLVertexArray 

```C++
AGE::OpenGLVertexArray::OpenGLVertexArray () 
```




<hr>



### function SetIndexBuffer 

_This function sets the index buffer for the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) _Array._
```C++
virtual void AGE::OpenGLVertexArray::SetIndexBuffer (
    Ref< IndexBuffer > & IndexBuffer
) override
```





**Parameters:**


* [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) A reference to an Index [**Buffer**](struct_a_g_e_1_1_buffer.md) object. 




        
Implements [*AGE::VertexArray::SetIndexBuffer*](class_a_g_e_1_1_vertex_array.md#function-setindexbuffer)


<hr>



### function Unbind 

_This function unbinds the current vertex array object._ 
```C++
virtual void AGE::OpenGLVertexArray::Unbind () override const
```





**Parameters:**


* `None` 



**Returns:**

void 





        
Implements [*AGE::VertexArray::Unbind*](class_a_g_e_1_1_vertex_array.md#function-unbind)


<hr>



### function begin [1/2]

_Returns an iterator pointing to the beginning of the vertex buffer list._ 
```C++
inline virtual std::vector< Ref< VertexBuffer > >::iterator AGE::OpenGLVertexArray::begin () override
```



This function returns an iterator that points to the first element in the vector of vertex buffers. If there are no elements, the returned iterator will be equal to [**end()**](class_a_g_e_1_1_open_g_l_vertex_array.md#function-end-12).




**Returns:**

An iterator pointing to the start of the vertex buffer list.


Returns an iterator pointing to the first element in the vertex buffer list. 

**Returns:**

An iterator pointing to the first element in the vertex buffer list. If the container is empty, the returned iterator will be equal to [**end()**](class_a_g_e_1_1_open_g_l_vertex_array.md#function-end-12). 





        
Implements [*AGE::VertexArray::begin*](class_a_g_e_1_1_vertex_array.md#function-begin-12)


<hr>



### function begin [2/2]

_Returns a constant iterator pointing to the beginning of the vertex buffer list._ 
```C++
inline virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::OpenGLVertexArray::begin () override const
```



This function returns an iterator that points to the first element in the vector of [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) objects, which represents the start of the vertex buffers collection. The returned iterator can be used with standard container functions like std::advance or std::next to move through the collection.




**Returns:**

A constant iterator pointing to the beginning of the vertex buffer list. If no elements exist in the vector, the returned iterator will equal [**end()**](class_a_g_e_1_1_open_g_l_vertex_array.md#function-end-12).


Returns a constant iterator pointing to the beginning of the vertex buffer list. 

**Returns:**

A constant iterator pointing to the first element in the vertex buffer list. If the container is empty, the returned iterator will be equal to [**end()**](class_a_g_e_1_1_open_g_l_vertex_array.md#function-end-12). 





        
Implements [*AGE::VertexArray::begin*](class_a_g_e_1_1_vertex_array.md#function-begin-22)


<hr>



### function end [1/2]

_Returns an iterator pointing to the theoretical element that follows the last element of the container. This function is used in range-based for loops and similar contexts where a sentinel value is needed._ 
```C++
inline virtual std::vector< Ref< VertexBuffer > >::iterator AGE::OpenGLVertexArray::end () override
```





**Returns:**

An iterator to the theoretical element that follows the last element of the container.


Returns an iterator pointing to the theoretical element that follows the last element of the container. This function returns an iterator to an imaginary element following the last actual element in the vector, which is valid but does not point to any real data (as vectors are sparse containers).




**Returns:**

An iterator to the theoretical element that follows the end of the sequence controlled by the container. 





        
Implements [*AGE::VertexArray::end*](class_a_g_e_1_1_vertex_array.md#function-end-12)


<hr>



### function end [2/2]

_Returns a constant iterator pointing to the theoretical element past the last element of the vertex buffer vector._ 
```C++
inline virtual std::vector< Ref< VertexBuffer > >::const_iterator AGE::OpenGLVertexArray::end () override const
```





**Returns:**

A constant iterator pointing to the theoretical element past the end of the vertex buffer vector.


Returns an iterator pointing to the past-the-end element in the container. 

**Returns:**

A constant iterator pointing to the past-the-end element of the container. 





        
Implements [*AGE::VertexArray::end*](class_a_g_e_1_1_vertex_array.md#function-end-22)


<hr>



### function ~OpenGLVertexArray 

_Destructor for_ [_**OpenGLVertexArray**_](class_a_g_e_1_1_open_g_l_vertex_array.md) _class. Deletes the vertex array object from GPU memory._
```C++
AGE::OpenGLVertexArray::~OpenGLVertexArray () override
```



This function is responsible for deleting a [**Vertex**](struct_a_g_e_1_1_vertex.md) Array Object (VAO) from GPU memory. The VAO was created during initialization and holds references to other data such as buffers, attributes etc. that are used in rendering operations. After deletion, this VAO can no longer be used by the OpenGL context.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLVertexArray.h`

