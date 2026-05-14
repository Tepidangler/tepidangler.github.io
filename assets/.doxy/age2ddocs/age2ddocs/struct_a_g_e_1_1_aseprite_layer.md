

# Struct AGE::AsepriteLayer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint16\_t | [**BlendMode**](#variable-blendmode)  <br> |
|  std::vector&lt; [**AsepriteCelChunk**](struct_a_g_e_1_1_aseprite_cel_chunk.md) &gt; | [**CelChunks**](#variable-celchunks)  <br> |
|  uint16\_t | [**Child**](#variable-child)  <br> |
|  uint16\_t | [**Flags**](#variable-flags)  <br> |
|  int | [**Layerindex**](#variable-layerindex)  <br> |
|  std::string | [**Name**](#variable-name)  <br> |
|  uint8\_t | [**Opacity**](#variable-opacity)  <br> |
|  uint16\_t | [**Type**](#variable-type)  <br> |
|  int | [**zIndex**](#variable-zindex)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteLayer**](#function-asepritelayer-13) () = default<br>_Default constructor for_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _class._ |
|   | [**AsepriteLayer**](#function-asepritelayer-23) (int LIndex, int ZIndex) <br>_Constructs an_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _object with the given layer index and z-index._ |
|   | [**AsepriteLayer**](#function-asepritelayer-33) (const [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) &) = default<br>_Copy constructor for the_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _class._ |




























## Public Attributes Documentation




### variable BlendMode 

```C++
uint16_t AGE::AsepriteLayer::BlendMode;
```




<hr>



### variable CelChunks 

```C++
std::vector<AsepriteCelChunk> AGE::AsepriteLayer::CelChunks;
```




<hr>



### variable Child 

```C++
uint16_t AGE::AsepriteLayer::Child;
```




<hr>



### variable Flags 

```C++
uint16_t AGE::AsepriteLayer::Flags;
```




<hr>



### variable Layerindex 

```C++
int AGE::AsepriteLayer::Layerindex;
```




<hr>



### variable Name 

```C++
std::string AGE::AsepriteLayer::Name;
```




<hr>



### variable Opacity 

```C++
uint8_t AGE::AsepriteLayer::Opacity;
```




<hr>



### variable Type 

```C++
uint16_t AGE::AsepriteLayer::Type;
```




<hr>



### variable zIndex 

```C++
int AGE::AsepriteLayer::zIndex;
```




<hr>
## Public Functions Documentation




### function AsepriteLayer [1/3]

_Default constructor for_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _class._
```C++
AGE::AsepriteLayer::AsepriteLayer () = default
```



This function initializes an instance of the [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) class with default values. It is used to create a new layer in [**Aseprite**](class_a_g_e_1_1_aseprite.md). 


        

<hr>



### function AsepriteLayer [2/3]

_Constructs an_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _object with the given layer index and z-index._
```C++
inline AGE::AsepriteLayer::AsepriteLayer (
    int LIndex,
    int ZIndex
) 
```





**Parameters:**


* `LIndex` The index of the layer in the [**Aseprite**](class_a_g_e_1_1_aseprite.md) document. 
* `ZIndex` The z-index of the layer, used for layering within a document. 




        

<hr>



### function AsepriteLayer [3/3]

_Copy constructor for the_ [_**AsepriteLayer**_](struct_a_g_e_1_1_aseprite_layer.md) _class._
```C++
AGE::AsepriteLayer::AsepriteLayer (
    const AsepriteLayer &
) = default
```



This function creates a new instance of [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) that is a copy of an existing one. It uses the default implementation provided by the compiler, which should work correctly as long as the members of [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) are trivially copyable.




**Parameters:**


* `other` The existing layer to be copied. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

