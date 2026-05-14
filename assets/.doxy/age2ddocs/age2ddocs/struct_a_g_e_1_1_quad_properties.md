

# Struct AGE::QuadProperties



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**Alpha**](#variable-alpha)   = `1.f`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**Color**](#variable-color)   = `{ 1.f, 1.f, 1.f, Alpha }`<br> |
|  int | [**EntityID**](#variable-entityid)   = `-1`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Size**](#variable-size)   = `{ 1.f, 1.f }`<br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**TextureCoords**](#variable-texturecoords)   = `{ { 1.f, 1.f }, { 1.f, 0.f },{ 0.f, 0.f }, { 0.f, 1.f } }`<br> |
|  float | [**TilingFactor**](#variable-tilingfactor)   = `1.f`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**TintColor**](#variable-tintcolor)   = `{ 1.f,1.f,1.f,1.f }`<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**Transform**](#variable-transform)   = `{ 1.f }`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ResetProperties**](#function-resetproperties) () <br>_Resets all properties of the object to default values._  |




























## Public Attributes Documentation




### variable Alpha 

```C++
float AGE::QuadProperties::Alpha;
```




<hr>



### variable Color 

```C++
Vector4 AGE::QuadProperties::Color;
```




<hr>



### variable EntityID 

```C++
int AGE::QuadProperties::EntityID;
```




<hr>



### variable Size 

```C++
Vector2 AGE::QuadProperties::Size;
```




<hr>



### variable TextureCoords 

```C++
Vector2 AGE::QuadProperties::TextureCoords[4];
```




<hr>



### variable TilingFactor 

```C++
float AGE::QuadProperties::TilingFactor;
```




<hr>



### variable TintColor 

```C++
Vector4 AGE::QuadProperties::TintColor;
```




<hr>



### variable Transform 

```C++
Matrix4D AGE::QuadProperties::Transform;
```




<hr>
## Public Functions Documentation




### function ResetProperties 

_Resets all properties of the object to default values._ 
```C++
inline void AGE::QuadProperties::ResetProperties () 
```



This function resets all properties of an object to their initial state. The properties include Alpha, Size, Color, TilingFactor, TintColor, TextureCoords, Transform and EntityID. All are set to their respective defaults: Alpha is set to 1.0f, Size is set to {1.0f, 1.0f}, Color is set to {1.0f, 1.0f, 1.0f, 1.0f}, TilingFactor is set to 1.0f, TintColor is set to {1.0f, 1.0f, 1.0f, 1.0f}, TextureCoords are set to {{1.0f, 1.0f}, {1.0f, 0.0f}, {0.0f, 0.0f}, {0.0f, 1.0f}}, Transform is set to {1.0f} and EntityID is set to -1.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

