

# Class AGE::SubTexture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  const float | [**GetHeight**](#function-getheight) () const<br> |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* | [**GetTexCoords**](#function-gettexcoords) () const<br> |
|  const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture) () const<br> |
|  const float | [**GetWidth**](#function-getwidth) () const<br> |
|   | [**SubTexture2D**](#function-subtexture2d-12) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Min, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Max) <br> |
|   | [**SubTexture2D**](#function-subtexture2d-22) (void \* Data) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; | [**CreateFromCoords**](#function-createfromcoords) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & SpriteLoc, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & CellSize, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & SpriteSize=[**Vector2**](struct_a_g_e_1_1_vector2.md){1.f, 1.f}) <br> |


























## Public Functions Documentation




### function GetHeight 

```C++
inline const float AGE::SubTexture2D::GetHeight () const
```




<hr>



### function GetTexCoords 

```C++
inline const Vector2 * AGE::SubTexture2D::GetTexCoords () const
```




<hr>



### function GetTexture 

```C++
inline const Ref< Texture2D > AGE::SubTexture2D::GetTexture () const
```




<hr>



### function GetWidth 

```C++
inline const float AGE::SubTexture2D::GetWidth () const
```




<hr>



### function SubTexture2D [1/2]

```C++
AGE::SubTexture2D::SubTexture2D (
    const Ref< Texture2D > & Texture,
    const Vector2 & Min,
    const Vector2 & Max
) 
```




<hr>



### function SubTexture2D [2/2]

```C++
AGE::SubTexture2D::SubTexture2D (
    void * Data
) 
```




<hr>
## Public Static Functions Documentation




### function CreateFromCoords 

```C++
static Ref< SubTexture2D > AGE::SubTexture2D::CreateFromCoords (
    const Ref< Texture2D > & Texture,
    const Vector2 & SpriteLoc,
    const Vector2 & CellSize,
    const Vector2 & SpriteSize=Vector2 {1.f, 1.f}
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/SubTexture.h`

