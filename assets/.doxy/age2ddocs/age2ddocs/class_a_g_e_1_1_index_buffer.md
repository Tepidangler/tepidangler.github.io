

# Class AGE::IndexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md)










Inherited by the following classes: [AGE::OpenGLIndexBuffer](class_a_g_e_1_1_open_g_l_index_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br>_This function is currently not implemented and will always return a null pointer. It's intended to provide the ability to cast this_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _instance to another type, but it's not yet supported. The function will assert false with an error message indicating that_[_**As()**_](class_a_g_e_1_1_index_buffer.md#function-as) _Failed!_ |
| virtual void | [**Bind**](#function-bind) () const = 0<br> |
| virtual uint32\_t | [**GetCount**](#function-getcount) () = 0<br> |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual  | [**~IndexBuffer**](#function-indexbuffer) () <br>_Virtual destructor for the_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**IndexBuffer**](class_a_g_e_1_1_index_buffer.md) &gt; | [**Create**](#function-create) (uint32\_t \* Indices, uint32\_t Count) <br> |


























## Public Functions Documentation




### function As 

_This function is currently not implemented and will always return a null pointer. It's intended to provide the ability to cast this_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _instance to another type, but it's not yet supported. The function will assert false with an error message indicating that_[_**As()**_](class_a_g_e_1_1_index_buffer.md#function-as) _Failed!_
```C++
template<typename T>
T * AGE::IndexBuffer::As () 
```





**Returns:**

nullptr Always returns nullptr.


This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown.




**Returns:**

A null pointer of type T\* 





        

<hr>



### function Bind 

```C++
virtual void AGE::IndexBuffer::Bind () const = 0
```




<hr>



### function GetCount 

```C++
virtual uint32_t AGE::IndexBuffer::GetCount () = 0
```




<hr>



### function InvalidateBuffer 

```C++
virtual void AGE::IndexBuffer::InvalidateBuffer () const = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::IndexBuffer::Unbind () const = 0
```




<hr>



### function ~IndexBuffer 

_Virtual destructor for the_ [_**IndexBuffer**_](class_a_g_e_1_1_index_buffer.md) _class._
```C++
inline virtual AGE::IndexBuffer::~IndexBuffer () 
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< IndexBuffer > AGE::IndexBuffer::Create (
    uint32_t * Indices,
    uint32_t Count
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

