

# Struct AGE::TextureSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  ImageFormat | [**Format**](#variable-format)   = `ImageFormat::RGBA8`<br> |
|  bool | [**GenerateMips**](#variable-generatemips)   = `true`<br> |
|  uint32\_t | [**Height**](#variable-height)   = `1`<br> |
|  uint32\_t | [**Width**](#variable-width)   = `1`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**TextureSpecification**](#function-texturespecification) () = default<br>_Default constructor for the_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _class._ |
| virtual  | [**~TextureSpecification**](#function-texturespecification) () = default<br>_Virtual destructor for the_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Instance) <br>_Deserialize a_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Instance) <br>_This function serializes a_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























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



### variable Width 

```C++
uint32_t AGE::TextureSpecification::Width;
```




<hr>
## Public Functions Documentation




### function TextureSpecification 

_Default constructor for the_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _class._
```C++
AGE::TextureSpecification::TextureSpecification () = default
```



This function initializes a new instance of the [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) class with default values.


Default constructor for the [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) class.


This function initializes a new instance of the [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) class with default values. 


        

<hr>



### function ~TextureSpecification 

_Virtual destructor for the_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _class._
```C++
virtual AGE::TextureSpecification::~TextureSpecification () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not return anything and has no parameters.


Virtual destructor for the [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not perform any operations on the state of the object itself.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize a_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
static void AGE::TextureSpecification::Deserialize (
    DataReader * Serializer,
    TextureSpecification & Instance
) 
```



This function reads the Width, Height, Format and GenerateMips fields of a [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) object from a [**DataReader**](class_a_g_e_1_1_data_reader.md). The Format field is read as an uint8\_t and then cast to ImageFormat. 

**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Instance` The [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) object to be deserialized.

Deserialize a [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) from a [**DataReader**](class_a_g_e_1_1_data_reader.md).


This function reads the Width, Height, Format and GenerateMips fields of a [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) from a [**DataReader**](class_a_g_e_1_1_data_reader.md). The format is read as an uint8\_t and then cast to ImageFormat. 

**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Instance` The [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) instance to populate with deserialized data. 




        

<hr>



### function Serialize 

_This function serializes a_ [_**TextureSpecification**_](struct_a_g_e_1_1_texture_specification.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static void AGE::TextureSpecification::Serialize (
    DataWriter * Serializer,
    const TextureSpecification & Instance
) 
```





**Parameters:**


* `Serializer` Pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for writing data. 
* `Instance` The [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) instance to be serialized.



**Returns:**

void


This function serializes a [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) instance into the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` Pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for writing data. 
* `Instance` The [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) instance to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/Texture.h`

