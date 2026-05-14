

# Class AGE::SubTexture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  const float | [**GetHeight**](#function-getheight) () const<br>_Returns the height of an object._  |
|  const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* | [**GetTexCoords**](#function-gettexcoords) () const<br>_Returns the texture coordinates of an object._  |
|  const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**GetTexture**](#function-gettexture) () const<br>_Returns the texture object associated with this instance._  |
|  const float | [**GetWidth**](#function-getwidth) () const<br>_Returns the width of an object._  |
|   | [**SubTexture2D**](#function-subtexture2d-12) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Min, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Max) <br>_Constructs a_ [_**SubTexture2D**_](class_a_g_e_1_1_sub_texture2_d.md) _object from a reference to a_[_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _, and two_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects representing the minimum and maximum texture coordinates._ |
|   | [**SubTexture2D**](#function-subtexture2d-22) (void \* Data) <br>_Constructor for_ [_**SubTexture2D**_](class_a_g_e_1_1_sub_texture2_d.md) _class. It takes a void pointer to data and initializes the texture, texcoords, width and height based on the data provided._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; | [**CreateFromCoords**](#function-createfromcoords) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & SpriteLoc, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & CellSize, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & SpriteSize=[**Vector2**](struct_a_g_e_1_1_vector2.md){1.f, 1.f}) <br>_Creates a subtexture from given texture at specified coordinates._  |


























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::SubTexture2D::__pad0__;
```




<hr>
## Public Functions Documentation




### function GetHeight 

_Returns the height of an object._ 
```C++
inline const float AGE::SubTexture2D::GetHeight () const
```



This function is used to get the current height value of an object. It does not take any parameters and returns a floating-point number representing the height.




**Returns:**

A float representing the height of the object. If no height has been set, it will return 0.0.


Returns the height of an object.




**Returns:**

A constant float representing the height of the object. 





        

<hr>



### function GetTexCoords 

_Returns the texture coordinates of an object._ 
```C++
inline const Vector2 * AGE::SubTexture2D::GetTexCoords () const
```



This function returns a pointer to the constant [**Vector2**](struct_a_g_e_1_1_vector2.md) object that represents the texture coordinates of an object. These are typically used for rendering textures on polygons in computer graphics.




**Returns:**

A pointer to a constant [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the texture coordinates. 





        

<hr>



### function GetTexture 

_Returns the texture object associated with this instance._ 
```C++
inline const Ref< Texture2D > AGE::SubTexture2D::GetTexture () const
```





**Returns:**

A constant reference to the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object.


Returns the texture object associated with this instance. 

**Returns:**

A constant reference to the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. 





        

<hr>



### function GetWidth 

_Returns the width of an object._ 
```C++
inline const float AGE::SubTexture2D::GetWidth () const
```



This function returns the current value of the member variable 'm\_Width'. It is a getter method for this variable.




**Returns:**

A float representing the width of the object. If no width has been set, it will return 0.0.


Returns the width of an object.


This function returns the current value of the member variable 'm\_Width'. It is a getter for this variable and does not take any parameters.




**Returns:**

float The current width of the object. 





        

<hr>



### function SubTexture2D [1/2]

_Constructs a_ [_**SubTexture2D**_](class_a_g_e_1_1_sub_texture2_d.md) _object from a reference to a_[_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _, and two_[_**Vector2**_](struct_a_g_e_1_1_vector2.md) _objects representing the minimum and maximum texture coordinates._
```C++
AGE::SubTexture2D::SubTexture2D (
    const Ref< Texture2D > & Texture,
    const Vector2 & Min,
    const Vector2 & Max
) 
```





**Parameters:**


* [**Texture**](class_a_g_e_1_1_texture.md) A const reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. This is the texture that the subtexture will be created for. 
* `Min` A const reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object. This represents the bottom-left corner of the subtexture within the parent texture. 
* `Max` A const reference to a [**Vector2**](struct_a_g_e_1_1_vector2.md) object. This represents the top-right corner of the subtexture within the parent texture.

Constructs a [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object from a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md), and two [**Vector2**](struct_a_g_e_1_1_vector2.md) coordinates.


The constructor initializes the texture member variable with the provided [**Texture2D**](class_a_g_e_1_1_texture2_d.md) reference. It also calculates the texture coordinates for the sub-texture based on the Min and Max vectors. 

**Parameters:**


* [**Texture**](class_a_g_e_1_1_texture.md) A const reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. 
* `Min` A [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the minimum x, y coordinates of the sub-texture in the texture atlas. 
* `Max` A [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the maximum x, y coordinates of the sub-texture in the texture atlas. 




        

<hr>



### function SubTexture2D [2/2]

_Constructor for_ [_**SubTexture2D**_](class_a_g_e_1_1_sub_texture2_d.md) _class. It takes a void pointer to data and initializes the texture, texcoords, width and height based on the data provided._
```C++
AGE::SubTexture2D::SubTexture2D (
    void * Data
) 
```





**Parameters:**


* `Data` A void pointer to the data from which the initialization will be done. The exact type of this data is unknown.

Constructs a [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object from another one.


This constructor creates a new [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object by copying the data of an existing one. It sets the texture, texcoords, width and height based on the values in the provided [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object. 

**Parameters:**


* `Data` A pointer to the [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object to copy from. 




        

<hr>
## Public Static Functions Documentation




### function CreateFromCoords 

_Creates a subtexture from given texture at specified coordinates._ 
```C++
static Ref< SubTexture2D > AGE::SubTexture2D::CreateFromCoords (
    const Ref< Texture2D > & Texture,
    const Vector2 & SpriteLoc,
    const Vector2 & CellSize,
    const Vector2 & SpriteSize=Vector2 {1.f, 1.f}
) 
```



This function takes in [**Texture2D**](class_a_g_e_1_1_texture2_d.md), [**Vector2**](struct_a_g_e_1_1_vector2.md) (SpriteLoc, CellSize, SpriteSize) to calculate the min and max UVs for [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md).


Creates a subtexture from given parameters.


This function takes in parameters that define a rectangular area within a larger texture and calculates the UV coordinates for this area. It then returns a new [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object with these calculated coordinates.




**Parameters:**


* [**Texture**](class_a_g_e_1_1_texture.md) The main texture to create the subtexture from. 
* `SpriteLoc` The location of the sprite in the texture (in cells). 
* `CellSize` The size of each cell in the texture (in pixels). 
* `SpriteSize` The size of the sprite within a single cell (in cells).



**Returns:**

A reference to a new [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/SubTexture.h`

