

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
















## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**AnimIsReady**](#function-animisready) () <br> |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-13) () = default<br> |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-23) (const [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) &) = default<br> |
|   | [**SpriteRendererComponent**](#function-spriterenderercomponent-33) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & C) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & Data) <br> |


























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
## Public Functions Documentation




### function AnimIsReady 

```C++
inline bool AGE::SpriteRendererComponent::AnimIsReady () 
```




<hr>



### function SpriteRendererComponent [1/3]

```C++
AGE::SpriteRendererComponent::SpriteRendererComponent () = default
```




<hr>



### function SpriteRendererComponent [2/3]

```C++
AGE::SpriteRendererComponent::SpriteRendererComponent (
    const SpriteRendererComponent &
) = default
```




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

```C++
static inline void AGE::SpriteRendererComponent::Deserialize (
    DataReader * Serializer,
    SpriteRendererComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::SpriteRendererComponent::Serialize (
    DataWriter * Serializer,
    const SpriteRendererComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

