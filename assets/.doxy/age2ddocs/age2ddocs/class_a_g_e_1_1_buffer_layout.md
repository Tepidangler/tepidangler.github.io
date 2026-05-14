

# Class AGE::BufferLayout



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BufferLayout**](#function-bufferlayout-12) () <br>[_**BufferLayout**_](class_a_g_e_1_1_buffer_layout.md) _is a class that represents the layout of a buffer in memory. It provides methods for adding elements to the buffer and retrieving them by index. The buffer can hold any type of data, but it's typically used with primitive types like int, float, etc._ |
|   | [**BufferLayout**](#function-bufferlayout-22) (const std::initializer\_list&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt; & Elements) <br>_Constructor for the_ [_**BufferLayout**_](class_a_g_e_1_1_buffer_layout.md) _class. Initializes the buffer layout with a list of elements._ |
|  const std::vector&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt; & | [**GetElements**](#function-getelements) () const<br>_Returns a constant reference to the vector of BufferElements stored in this object._  |
|  uint32\_t | [**GetStride**](#function-getstride) () const<br>_Returns the stride value of the object._  |
|  std::vector&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt;::iterator | [**begin**](#function-begin-12) () <br> |
|  std::vector&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br> |
|  std::vector&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt;::iterator | [**end**](#function-end-12) () <br>_Returns an iterator pointing to the theoretical element past the last element of the vector._  |
|  std::vector&lt; [**BufferElement**](struct_a_g_e_1_1_buffer_element.md) &gt;::const\_iterator | [**end**](#function-end-22) () const<br>_Returns a constant iterator pointing to the past-the-end element in the buffer elements vector._  |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::BufferLayout::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::BufferLayout::__pad1__;
```




<hr>
## Public Functions Documentation




### function BufferLayout [1/2]

[_**BufferLayout**_](class_a_g_e_1_1_buffer_layout.md) _is a class that represents the layout of a buffer in memory. It provides methods for adding elements to the buffer and retrieving them by index. The buffer can hold any type of data, but it's typically used with primitive types like int, float, etc._
```C++
AGE::BufferLayout::BufferLayout () 
```



[**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) is a class that represents the layout of a buffer in memory.


This class provides methods for managing and manipulating the layout of a buffer in memory. It does not handle the actual data within the buffer, only its structure. 


        

<hr>



### function BufferLayout [2/2]

_Constructor for the_ [_**BufferLayout**_](class_a_g_e_1_1_buffer_layout.md) _class. Initializes the buffer layout with a list of elements._
```C++
inline AGE::BufferLayout::BufferLayout (
    const std::initializer_list< BufferElement > & Elements
) 
```





**Parameters:**


* `Elements` A std::initializer\_list&lt;BufferElement&gt; containing the elements to be added to the layout. 




        

<hr>



### function GetElements 

_Returns a constant reference to the vector of BufferElements stored in this object._ 
```C++
inline const std::vector< BufferElement > & AGE::BufferLayout::GetElements () const
```





**Returns:**

A constant reference to the vector of BufferElements (m\_Elements). 





        

<hr>



### function GetStride 

_Returns the stride value of the object._ 
```C++
inline uint32_t AGE::BufferLayout::GetStride () const
```





**Returns:**

The stride value as a uint32\_t. 





        

<hr>



### function begin [1/2]

```C++
inline std::vector< BufferElement >::iterator AGE::BufferLayout::begin () 
```




<hr>



### function begin [2/2]

```C++
inline std::vector< BufferElement >::const_iterator AGE::BufferLayout::begin () const
```




<hr>



### function end [1/2]

_Returns an iterator pointing to the theoretical element past the last element of the vector._ 
```C++
inline std::vector< BufferElement >::iterator AGE::BufferLayout::end () 
```





**Returns:**

An iterator to the theoretical element past the end of the vector. 





        

<hr>



### function end [2/2]

_Returns a constant iterator pointing to the past-the-end element in the buffer elements vector._ 
```C++
inline std::vector< BufferElement >::const_iterator AGE::BufferLayout::end () const
```





**Returns:**

A constant iterator pointing to the past-the-end element. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

