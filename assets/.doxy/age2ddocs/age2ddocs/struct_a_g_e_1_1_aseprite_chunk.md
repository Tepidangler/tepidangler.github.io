

# Struct AGE::AsepriteChunk



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; std::byte &gt; | [**Data**](#variable-data)  <br> |
|  uint32\_t | [**Size**](#variable-size)  <br> |
|  AsepriteChunkType | [**Type**](#variable-type)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteChunk**](#function-asepritechunk-12) () = default<br>_Default constructor for_ [_**AsepriteChunk**_](struct_a_g_e_1_1_aseprite_chunk.md) _class._ |
|   | [**AsepriteChunk**](#function-asepritechunk-22) (const [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md) &) = default<br>_Default copy constructor for the_ [_**AsepriteChunk**_](struct_a_g_e_1_1_aseprite_chunk.md) _class._ |




























## Public Attributes Documentation




### variable Data 

```C++
std::vector<std::byte> AGE::AsepriteChunk::Data;
```




<hr>



### variable Size 

```C++
uint32_t AGE::AsepriteChunk::Size;
```




<hr>



### variable Type 

```C++
AsepriteChunkType AGE::AsepriteChunk::Type;
```




<hr>
## Public Functions Documentation




### function AsepriteChunk [1/2]

_Default constructor for_ [_**AsepriteChunk**_](struct_a_g_e_1_1_aseprite_chunk.md) _class._
```C++
AGE::AsepriteChunk::AsepriteChunk () = default
```




<hr>



### function AsepriteChunk [2/2]

_Default copy constructor for the_ [_**AsepriteChunk**_](struct_a_g_e_1_1_aseprite_chunk.md) _class._
```C++
AGE::AsepriteChunk::AsepriteChunk (
    const AsepriteChunk &
) = default
```



This function is used to create a new instance of [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md) by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The existing [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md) instance to copy from. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

