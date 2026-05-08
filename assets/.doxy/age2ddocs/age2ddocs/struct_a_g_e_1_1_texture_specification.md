

# Struct AGE::TextureSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  ImageFormat | [**Format**](#variable-format)   = `ImageFormat::RGBA8`<br> |
|  bool | [**GenerateMips**](#variable-generatemips)   = `true`<br> |
|  uint32\_t | [**Height**](#variable-height)   = `1`<br> |
|  bool | [**IsArray**](#variable-isarray)   = `false`<br> |
|  uint32\_t | [**Width**](#variable-width)   = `1`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**TextureSpecification**](#function-texturespecification) () = default<br> |
| virtual  | [**~TextureSpecification**](#function-texturespecification) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Instance) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Instance) <br> |


























## Public Attributes Documentation




### variable Format 

```C++
ImageFormat AGE::TextureSpecification::Format;
```




<hr>



### variable GenerateMips 

```C++
bool AGE::TextureSpecification::GenerateMips;
```




<hr>



### variable Height 

```C++
uint32_t AGE::TextureSpecification::Height;
```




<hr>



### variable IsArray 

```C++
bool AGE::TextureSpecification::IsArray;
```




<hr>



### variable Width 

```C++
uint32_t AGE::TextureSpecification::Width;
```




<hr>
## Public Functions Documentation




### function TextureSpecification 

```C++
AGE::TextureSpecification::TextureSpecification () = default
```




<hr>



### function ~TextureSpecification 

```C++
virtual AGE::TextureSpecification::~TextureSpecification () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static void AGE::TextureSpecification::Deserialize (
    DataReader * Serializer,
    TextureSpecification & Instance
) 
```




<hr>



### function Serialize 

```C++
static void AGE::TextureSpecification::Serialize (
    DataWriter * Serializer,
    const TextureSpecification & Instance
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/Texture.h`

