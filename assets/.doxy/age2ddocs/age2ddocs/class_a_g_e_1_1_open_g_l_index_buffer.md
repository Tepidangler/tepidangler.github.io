

# Class AGE::OpenGLIndexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLIndexBuffer**](class_a_g_e_1_1_open_g_l_index_buffer.md)








Inherits the following classes: [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override const<br>_This function binds the OpenGL Index_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual uint32\_t | [**GetCount**](#function-getcount) () override<br>_This function returns the current count value._  |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () override const<br>_Invalidates and deletes the OpenGL buffer._  |
|   | [**OpenGLIndexBuffer**](#function-openglindexbuffer) (uint32\_t \* Indices, uint32\_t Size) <br>_Constructor for_ [_**OpenGLIndexBuffer**_](class_a_g_e_1_1_open_g_l_index_buffer.md) _. Creates an index buffer object and initializes it with the given indices._ |
| virtual void | [**Unbind**](#function-unbind) () override const<br>_This function unbinds the OpenGL Element Array_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual  | [**~OpenGLIndexBuffer**](#function-openglindexbuffer) () <br>_Destructor for_ [_**OpenGLIndexBuffer**_](class_a_g_e_1_1_open_g_l_index_buffer.md) _. Deletes the buffer with ID m\_RendererID using glDeleteBuffers function._ |


## Public Functions inherited from AGE::IndexBuffer

See [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_index_buffer.md#function-as) () <br>_This function is currently not implemented and will always return a null pointer. It's intended to provide the ability to cast this_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _instance to another type, but it's not yet supported. The function will assert false with an error message indicating that_[_**As()**_](class_a_g_e_1_1_index_buffer.md#function-as) _Failed!_ |
| virtual void | [**Bind**](class_a_g_e_1_1_index_buffer.md#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetCount**](class_a_g_e_1_1_index_buffer.md#function-getcount) () = 0<br> |
| virtual void | [**InvalidateBuffer**](class_a_g_e_1_1_index_buffer.md#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_index_buffer.md#function-unbind) () const = 0<br> |
| virtual  | [**~IndexBuffer**](class_a_g_e_1_1_index_buffer.md#function-indexbuffer) () <br>_Virtual destructor for the_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _class._ |




## Public Static Functions inherited from AGE::IndexBuffer

See [AGE::IndexBuffer](class_a_g_e_1_1_index_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_index_buffer.md#function-create) (uint32\_t \* Indices, uint32\_t Count) <br> |


















































## Public Functions Documentation




### function Bind 

_This function binds the OpenGL Index_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual void AGE::OpenGLIndexBuffer::Bind () override const
```



The function uses glBindBuffer to bind the buffer with ID 'm\_RendererID' as an element array buffer (GL\_ELEMENT\_ARRAY\_BUFFER). It is used for rendering of indexed primitives, such as triangles or lines, using vertices from a vertex array.




**Returns:**

void No return value.


This function binds the OpenGL Index [**Buffer**](struct_a_g_e_1_1_buffer.md).


It uses glBindBuffer to bind the buffer with target GL\_ELEMENT\_ARRAY\_BUFFER and the ID of this buffer as argument. The purpose of binding an index buffer is to specify which vertex array object (VAO) should be used for rendering. 


        
Implements [*AGE::IndexBuffer::Bind*](class_a_g_e_1_1_index_buffer.md#function-bind)


<hr>



### function GetCount 

_This function returns the current count value._ 
```C++
inline virtual uint32_t AGE::OpenGLIndexBuffer::GetCount () override
```





**Returns:**

The current count value as a uint32\_t. 





        
Implements [*AGE::IndexBuffer::GetCount*](class_a_g_e_1_1_index_buffer.md#function-getcount)


<hr>



### function InvalidateBuffer 

_Invalidates and deletes the OpenGL buffer._ 
```C++
virtual void AGE::OpenGLIndexBuffer::InvalidateBuffer () override const
```



This function first invalidates any existing data in the buffer using glInvalidateBufferData(). Then it deletes the buffer itself with glDeleteBuffers(). The buffer's ID is passed to these functions, indicating which buffer should be affected.




**Returns:**

void


This function is used to invalidate the buffer data and delete the OpenGL index buffer.


The function first calls glInvalidateBufferData() on the OpenGL context with the renderer ID of this object as an argument, which marks the buffer's data as needing update. Then it deletes the buffer using glDeleteBuffers(), passing in the same renderer ID to remove the buffer from memory.




**Returns:**

void 





        
Implements [*AGE::IndexBuffer::InvalidateBuffer*](class_a_g_e_1_1_index_buffer.md#function-invalidatebuffer)


<hr>



### function OpenGLIndexBuffer 

_Constructor for_ [_**OpenGLIndexBuffer**_](class_a_g_e_1_1_open_g_l_index_buffer.md) _. Creates an index buffer object and initializes it with the given indices._
```C++
AGE::OpenGLIndexBuffer::OpenGLIndexBuffer (
    uint32_t * Indices,
    uint32_t Size
) 
```





**Parameters:**


* `Indices` Pointer to the array of indices that will be used to initialize the buffer. 
* `Count` The number of elements in the Indices array.

Constructs an [**OpenGLIndexBuffer**](class_a_g_e_1_1_open_g_l_index_buffer.md) object.


This function creates a new OpenGL index buffer and initializes it with the given indices. The number of indices is specified by the Count parameter.




**Parameters:**


* `Indices` Pointer to the array of indices that will be copied into the GPU memory. 
* `Count` Number of indices in the Indices array. 




        

<hr>



### function Unbind 

_This function unbinds the OpenGL Element Array_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual void AGE::OpenGLIndexBuffer::Unbind () override const
```



It binds the buffer target to GL\_ELEMENT\_ARRAY\_BUFFER and sets the buffer ID to 0, effectively unbinding it from the current context.




**Returns:**

void


This function unbinds the OpenGL Element Array [**Buffer**](struct_a_g_e_1_1_buffer.md).


It binds the buffer target to GL\_ELEMENT\_ARRAY\_BUFFER and sets the buffer ID to 0, effectively unbinding it from any rendering operations that use this buffer.




**Returns:**

void 





        
Implements [*AGE::IndexBuffer::Unbind*](class_a_g_e_1_1_index_buffer.md#function-unbind)


<hr>



### function ~OpenGLIndexBuffer 

_Destructor for_ [_**OpenGLIndexBuffer**_](class_a_g_e_1_1_open_g_l_index_buffer.md) _. Deletes the buffer with ID m\_RendererID using glDeleteBuffers function._
```C++
virtual AGE::OpenGLIndexBuffer::~OpenGLIndexBuffer () 
```





**Parameters:**


* `None` 



**Returns:**

None


Destructor for [**OpenGLIndexBuffer**](class_a_g_e_1_1_open_g_l_index_buffer.md). Deletes the buffer with ID m\_RendererID using glDeleteBuffers function.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

