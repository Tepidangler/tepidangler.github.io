

# Struct AGE::AsepriteCelChunk



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteCelChunk**](struct_a_g_e_1_1_aseprite_cel_chunk.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint16\_t | [**CelType**](#variable-celtype)  <br> |
|  uint16\_t | [**FramePosition**](#variable-frameposition)  <br> |
|  uint16\_t | [**Height**](#variable-height)  <br> |
|  uint16\_t | [**LayerIndex**](#variable-layerindex)  <br> |
|  uint8\_t | [**Opacity**](#variable-opacity)  <br> |
|  std::vector&lt; [**AsepritePixelData**](struct_a_g_e_1_1_aseprite_pixel_data.md) &gt; | [**PixelDatas**](#variable-pixeldatas)  <br> |
|  uint16\_t | [**Width**](#variable-width)  <br> |
|  int16\_t | [**x**](#variable-x)  <br> |
|  int16\_t | [**y**](#variable-y)  <br> |
|  int16\_t | [**zIndex**](#variable-zindex)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteCelChunk**](#function-asepritecelchunk) () = default<br>_Default constructor for_ [_**AsepriteCelChunk**_](struct_a_g_e_1_1_aseprite_cel_chunk.md) _class._ |
|  int | [**order**](#function-order) () const<br>_This function returns the sum of the 'LayerIndex' and 'zIndex'._  |
|   | [**~AsepriteCelChunk**](#function-asepritecelchunk) () = default<br>_Default destructor for the_ [_**AsepriteCelChunk**_](struct_a_g_e_1_1_aseprite_cel_chunk.md) _class._ |




























## Public Attributes Documentation




### variable CelType 

```C++
uint16_t AGE::AsepriteCelChunk::CelType;
```




<hr>



### variable FramePosition 

```C++
uint16_t AGE::AsepriteCelChunk::FramePosition;
```




<hr>



### variable Height 

```C++
uint16_t AGE::AsepriteCelChunk::Height;
```




<hr>



### variable LayerIndex 

```C++
uint16_t AGE::AsepriteCelChunk::LayerIndex;
```




<hr>



### variable Opacity 

```C++
uint8_t AGE::AsepriteCelChunk::Opacity;
```




<hr>



### variable PixelDatas 

```C++
std::vector<AsepritePixelData> AGE::AsepriteCelChunk::PixelDatas;
```




<hr>



### variable Width 

```C++
uint16_t AGE::AsepriteCelChunk::Width;
```




<hr>



### variable x 

```C++
int16_t AGE::AsepriteCelChunk::x;
```




<hr>



### variable y 

```C++
int16_t AGE::AsepriteCelChunk::y;
```




<hr>



### variable zIndex 

```C++
int16_t AGE::AsepriteCelChunk::zIndex;
```




<hr>
## Public Functions Documentation




### function AsepriteCelChunk 

_Default constructor for_ [_**AsepriteCelChunk**_](struct_a_g_e_1_1_aseprite_cel_chunk.md) _class._
```C++
AGE::AsepriteCelChunk::AsepriteCelChunk () = default
```




<hr>



### function order 

_This function returns the sum of the 'LayerIndex' and 'zIndex'._ 
```C++
inline int AGE::AsepriteCelChunk::order () const
```





**Returns:**

The sum of 'LayerIndex' and 'zIndex', as an integer. If either index is not set, it will return 0. 





        

<hr>



### function ~AsepriteCelChunk 

_Default destructor for the_ [_**AsepriteCelChunk**_](struct_a_g_e_1_1_aseprite_cel_chunk.md) _class._
```C++
AGE::AsepriteCelChunk::~AsepriteCelChunk () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not perform any operations on the actual data stored in the chunk. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

