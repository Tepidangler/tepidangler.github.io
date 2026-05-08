

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
|   | [**BufferElement**](#function-bufferelement-12) () <br> |
|   | [**BufferElement**](#function-bufferelement-22) (ShaderDataType Type, const std::string & Name, bool normalized=false) <br> |
|  uint32\_t | [**GetComponentCount**](#function-getcomponentcount) () const<br> |




























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

```C++
inline AGE::BufferElement::BufferElement () 
```




<hr>



### function BufferElement [2/2]

```C++
inline AGE::BufferElement::BufferElement (
    ShaderDataType Type,
    const std::string & Name,
    bool normalized=false
) 
```




<hr>



### function GetComponentCount 

```C++
inline uint32_t AGE::BufferElement::GetComponentCount () const
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

