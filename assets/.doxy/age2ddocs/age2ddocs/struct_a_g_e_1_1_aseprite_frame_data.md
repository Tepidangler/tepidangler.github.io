

# Struct AGE::AsepriteFrameData



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**BytesInFrame**](#variable-bytesinframe)  <br> |
|  std::vector&lt; [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md) &gt; | [**ChunkData**](#variable-chunkdata)  <br> |
|  uint16\_t | [**FrameDuration**](#variable-frameduration)  <br> |
|  std::vector&lt; [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) &gt; | [**Layers**](#variable-layers)  <br> |
|  uint16\_t | [**MagicNumber**](#variable-magicnumber)   = `0xF1FA`<br> |
|  uint32\_t | [**NewNumOfChunks**](#variable-newnumofchunks)  <br> |
|  std::vector&lt; [**AsepritePaletteChunk**](struct_a_g_e_1_1_aseprite_palette_chunk.md) &gt; | [**NewPaletteChunks**](#variable-newpalettechunks)  <br> |
|  uint16\_t | [**NumOfChunks**](#variable-numofchunks)  <br> |
|  std::vector&lt; [**AsepriteOldPaletteChunk**](struct_a_g_e_1_1_aseprite_old_palette_chunk.md) &gt; | [**OldPaletteChunks**](#variable-oldpalettechunks)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteFrameData**](#function-asepriteframedata-12) () = default<br>_Default constructor for_ [_**AsepriteFrameData**_](struct_a_g_e_1_1_aseprite_frame_data.md) _class._ |
|   | [**AsepriteFrameData**](#function-asepriteframedata-22) (const [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) &) = default<br>_Default copy constructor for the_ [_**AsepriteFrameData**_](struct_a_g_e_1_1_aseprite_frame_data.md) _class._ |




























## Public Attributes Documentation




### variable BytesInFrame 

```C++
uint32_t AGE::AsepriteFrameData::BytesInFrame;
```




<hr>



### variable ChunkData 

```C++
std::vector<AsepriteChunk> AGE::AsepriteFrameData::ChunkData;
```




<hr>



### variable FrameDuration 

```C++
uint16_t AGE::AsepriteFrameData::FrameDuration;
```




<hr>



### variable Layers 

```C++
std::vector<AsepriteLayer> AGE::AsepriteFrameData::Layers;
```




<hr>



### variable MagicNumber 

```C++
uint16_t AGE::AsepriteFrameData::MagicNumber;
```




<hr>



### variable NewNumOfChunks 

```C++
uint32_t AGE::AsepriteFrameData::NewNumOfChunks;
```




<hr>



### variable NewPaletteChunks 

```C++
std::vector<AsepritePaletteChunk> AGE::AsepriteFrameData::NewPaletteChunks;
```




<hr>



### variable NumOfChunks 

```C++
uint16_t AGE::AsepriteFrameData::NumOfChunks;
```




<hr>



### variable OldPaletteChunks 

```C++
std::vector<AsepriteOldPaletteChunk> AGE::AsepriteFrameData::OldPaletteChunks;
```




<hr>
## Public Functions Documentation




### function AsepriteFrameData [1/2]

_Default constructor for_ [_**AsepriteFrameData**_](struct_a_g_e_1_1_aseprite_frame_data.md) _class._
```C++
AGE::AsepriteFrameData::AsepriteFrameData () = default
```




<hr>



### function AsepriteFrameData [2/2]

_Default copy constructor for the_ [_**AsepriteFrameData**_](struct_a_g_e_1_1_aseprite_frame_data.md) _class._
```C++
AGE::AsepriteFrameData::AsepriteFrameData (
    const AsepriteFrameData &
) = default
```



This function is used to create a new instance of [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The existing [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) instance to copy. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

