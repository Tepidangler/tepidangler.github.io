

# Struct AGE::SpriteRendererComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Animation**](class_a_g_e_1_1_animation.md) | [**AnimInstance**](#variable-animinstance)  <br> |
|  std::vector&lt; [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) &gt; | [**AnimTextures**](#variable-animtextures)  <br> |
|  std::filesystem::path | [**AsepriteFile**](#variable-asepritefile)   = `""`<br> |
|  std::string | [**AsepriteName**](#variable-asepritename)   = `"None"`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**Color**](#variable-color)   = `{ 1.f }`<br> |
|  int | [**CurrentAnimationID**](#variable-currentanimationid)   = `-1`<br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**DiagTexture**](#variable-diagtexture)  <br> |
|  CharMovementStatus | [**MovementStatus**](#variable-movementstatus)   = `CharMovementStatus::Idle`<br> |
|  [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) | [**QuadProps**](#variable-quadprops)  <br> |
|  std::string | [**RigidBodyType**](#variable-rigidbodytype)   = `"Dynamic"`<br> |
|  Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; | [**SubTexture**](#variable-subtexture)  <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Texture**](#variable-texture)  <br> |
|  float | [**TileHeight**](#variable-tileheight)  <br> |
|  int | [**TileID**](#variable-tileid)   = `-1`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**TileLocation**](#variable-tilelocation)  <br> |
|  float | [**TileWidth**](#variable-tilewidth)  <br> |
|  int | [**TilesLayer**](#variable-tileslayer)   = `-1`<br> |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  bool | [**bTile**](#variable-btile)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**AnimIsReady**](#function-animisready) () <br>_This function checks if any animation is ready to load._  |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-13) () = default<br>_Default constructor for the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _class._ |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-23) (const [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) &) = default<br>_Default copy constructor for the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _class._ |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-33) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & C) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & Data) <br>_This function deserializes a_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & Data) <br>_This function serializes the sprite renderer component data into a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


























## Public Attributes Documentation




### variable AnimInstance 

```C++
Animation AGE::SpriteRendererComponent::AnimInstance;
```




<hr>



### variable AnimTextures 

```C++
std::vector<AnimationSpecification> AGE::SpriteRendererComponent::AnimTextures;
```




<hr>



### variable AsepriteFile 

```C++
std::filesystem::path AGE::SpriteRendererComponent::AsepriteFile;
```




<hr>



### variable AsepriteName 

```C++
std::string AGE::SpriteRendererComponent::AsepriteName;
```




<hr>



### variable Color 

```C++
Vector4 AGE::SpriteRendererComponent::Color;
```




<hr>



### variable CurrentAnimationID 

```C++
int AGE::SpriteRendererComponent::CurrentAnimationID;
```




<hr>



### variable DiagTexture 

```C++
Ref<Texture2D> AGE::SpriteRendererComponent::DiagTexture;
```




<hr>



### variable MovementStatus 

```C++
CharMovementStatus AGE::SpriteRendererComponent::MovementStatus;
```




<hr>



### variable QuadProps 

```C++
QuadProperties AGE::SpriteRendererComponent::QuadProps;
```




<hr>



### variable RigidBodyType 

```C++
std::string AGE::SpriteRendererComponent::RigidBodyType;
```




<hr>



### variable SubTexture 

```C++
Ref<SubTexture2D> AGE::SpriteRendererComponent::SubTexture;
```




<hr>



### variable Texture 

```C++
Ref<Texture2D> AGE::SpriteRendererComponent::Texture;
```




<hr>



### variable TileHeight 

```C++
float AGE::SpriteRendererComponent::TileHeight;
```




<hr>



### variable TileID 

```C++
int AGE::SpriteRendererComponent::TileID;
```




<hr>



### variable TileLocation 

```C++
Vector2 AGE::SpriteRendererComponent::TileLocation;
```




<hr>



### variable TileWidth 

```C++
float AGE::SpriteRendererComponent::TileWidth;
```




<hr>



### variable TilesLayer 

```C++
int AGE::SpriteRendererComponent::TilesLayer;
```




<hr>



### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::SpriteRendererComponent::__pad0__;
```




<hr>



### variable bTile 

```C++
bool AGE::SpriteRendererComponent::bTile;
```




<hr>
## Public Functions Documentation




### function AnimIsReady 

_This function checks if any animation is ready to load._ 
```C++
inline bool AGE::SpriteRendererComponent::AnimIsReady () 
```



It iterates over the AnimTextures vector and returns true as soon as it finds an animation that matches the current MovementStatus and is ready to load (i.e., IsReadyToLoad() returns true). If no such animation is found, it returns false.




**Returns:**

bool - Returns true if any animation is ready to load, false otherwise. 





        

<hr>



### function SpriteRendererComponent [1/3]

_Default constructor for the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _class._
```C++
AGE::SpriteRendererComponent::SpriteRendererComponent () = default
```




<hr>



### function SpriteRendererComponent [2/3]

_Default copy constructor for the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _class._
```C++
AGE::SpriteRendererComponent::SpriteRendererComponent (
    const SpriteRendererComponent &
) = default
```



This function is used to create a new instance of the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) class by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The existing [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) instance to copy. 




        

<hr>



### function SpriteRendererComponent [3/3]

```C++
inline AGE::SpriteRendererComponent::SpriteRendererComponent (
    const Vector4 & C
) 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes a_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
static inline void AGE::SpriteRendererComponent::Deserialize (
    DataReader * Serializer,
    SpriteRendererComponent & Data
) 
```



The function reads data from the serialized format and populates the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) with it. It does not return anything as it directly modifies the passed in [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) reference.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides the serialized data. 
* `Data` Reference to the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) which will be populated by this function. 




        

<hr>



### function Serialize 

_This function serializes the sprite renderer component data into a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::SpriteRendererComponent::Serialize (
    DataWriter * Serializer,
    const SpriteRendererComponent & Data
) 
```





**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the data will be written. 
* `Data` The [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) whose data is being serialized.



**Returns:**

None 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

