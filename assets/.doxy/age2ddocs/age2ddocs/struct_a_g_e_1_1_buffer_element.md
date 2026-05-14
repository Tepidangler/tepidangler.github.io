

# Struct AGE::BufferElement



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**BufferElement**](struct_a_g_e_1_1_buffer_element.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**DataStepRate**](#variable-datasteprate)   = `0`<br> |
|  ShaderDataType | [**DataType**](#variable-datatype)  <br> |
|  uint32\_t | [**Index**](#variable-index)   = `0`<br> |
|  std::string | [**Name**](#variable-name)   = `""`<br> |
|  bool | [**Normalized**](#variable-normalized)   = `false`<br> |
|  uint32\_t | [**Offset**](#variable-offset)   = `0`<br> |
|  uint32\_t | [**Size**](#variable-size)   = `0`<br> |
|  uint32\_t | [**Slot**](#variable-slot)   = `0`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BufferElement**](#function-bufferelement-12) () <br>_Default constructor for_ [_**BufferElement**_](struct_a_g_e_1_1_buffer_element.md) _class._ |
|   | [**BufferElement**](#function-bufferelement-22) (ShaderDataType Type, const std::string & Name, bool normalized=false) <br>[_**BufferElement**_](struct_a_g_e_1_1_buffer_element.md) _is a class representing an element in a buffer. It holds information about the name, type of data, size and offset of the data, as well as whether it's normalized or not._ |
|  uint32\_t | [**GetComponentCount**](#function-getcomponentcount) () const<br>_GetComponentCount returns the number of components in a shader data type._  |




























## Public Attributes Documentation




### variable DataStepRate 

```C++
uint32_t AGE::BufferElement::DataStepRate;
```




<hr>



### variable DataType 

```C++
ShaderDataType AGE::BufferElement::DataType;
```




<hr>



### variable Index 

```C++
uint32_t AGE::BufferElement::Index;
```




<hr>



### variable Name 

```C++
std::string AGE::BufferElement::Name;
```




<hr>



### variable Normalized 

```C++
bool AGE::BufferElement::Normalized;
```




<hr>



### variable Offset 

```C++
uint32_t AGE::BufferElement::Offset;
```




<hr>



### variable Size 

```C++
uint32_t AGE::BufferElement::Size;
```




<hr>



### variable Slot 

```C++
uint32_t AGE::BufferElement::Slot;
```




<hr>
## Public Functions Documentation




### function BufferElement [1/2]

_Default constructor for_ [_**BufferElement**_](struct_a_g_e_1_1_buffer_element.md) _class._
```C++
inline AGE::BufferElement::BufferElement () 
```




<hr>



### function BufferElement [2/2]

[_**BufferElement**_](struct_a_g_e_1_1_buffer_element.md) _is a class representing an element in a buffer. It holds information about the name, type of data, size and offset of the data, as well as whether it's normalized or not._
```C++
inline AGE::BufferElement::BufferElement (
    ShaderDataType Type,
    const std::string & Name,
    bool normalized=false
) 
```





**Parameters:**


* `Type` The type of shader data (e.g., float, int). 
* `Name` The name of the buffer element. 
* `normalized` A boolean indicating if the data is normalized. Default value is false. 




        

<hr>



### function GetComponentCount 

_GetComponentCount returns the number of components in a shader data type._ 
```C++
inline uint32_t AGE::BufferElement::GetComponentCount () const
```



This function takes into account the current value of DataType and returns the appropriate number of components. The return values are as follows:
* For DataType = 0, it returns 1 (Unknown ShaderDataType).
* For DataType = 1 to 4 inclusive, it returns 1.
* For DataType = 5 to 6 inclusive, it returns 9.
* For DataType = 7 to 8 inclusive, it returns 2.
* For DataType = 9 to 10 inclusive, it returns 3.
* For DataType = 11, it returns 4 (Unknown ShaderDataType).






**Returns:**

uint32\_t The number of components in the shader data type. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

