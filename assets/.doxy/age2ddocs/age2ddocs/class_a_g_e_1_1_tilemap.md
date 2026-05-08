

# Class AGE::Tilemap



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Tilemap**](class_a_g_e_1_1_tilemap.md)








Inherits the following classes: std::enable_shared_from_this< Tilemap >


































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**BindData**](#function-binddata) () <br> |
|  void | [**BuildTilemapData**](#function-buildtilemapdata) () <br> |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetAssetID**](#function-getassetid) () <br> |
|  std::vector&lt; [**TilesetData**](struct_a_g_e_1_1_tileset_data.md) &gt; & | [**GetData**](#function-getdata) () <br> |
|  std::pair&lt; uint32\_t, uint32\_t &gt; | [**GetMapDimensions**](#function-getmapdimensions) () <br> |
|  const uint32\_t | [**GetNumberOfLayers**](#function-getnumberoflayers) () <br> |
|  std::filesystem::path | [**GetPath**](#function-getpath) () const<br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene) () <br> |
|  std::map&lt; uint32\_t, std::vector&lt; [**Vector2**](struct_a_g_e_1_1_vector2.md) \* &gt; &gt; & | [**GetUVs**](#function-getuvs) () <br> |
|  void | [**SetPath**](#function-setpath) (const std::filesystem::path & Path) <br> |
|  void | [**SetScene**](#function-setscene) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; & scene) <br> |
|  void | [**SetShaderData**](#function-setshaderdata) () <br> |
|  void | [**SetTileLocations**](#function-settilelocations) () <br> |
|   | [**Tilemap**](#function-tilemap) (tmx\_map \* Map) <br> |
|   | [**~Tilemap**](#function-tilemap) () <br> |




























## Public Functions Documentation




### function BindData 

```C++
void AGE::Tilemap::BindData () 
```




<hr>



### function BuildTilemapData 

```C++
void AGE::Tilemap::BuildTilemapData () 
```




<hr>



### function GetAssetID 

```C++
inline UUID AGE::Tilemap::GetAssetID () 
```




<hr>



### function GetData 

```C++
inline std::vector< TilesetData > & AGE::Tilemap::GetData () 
```




<hr>



### function GetMapDimensions 

```C++
inline std::pair< uint32_t, uint32_t > AGE::Tilemap::GetMapDimensions () 
```




<hr>



### function GetNumberOfLayers 

```C++
const uint32_t AGE::Tilemap::GetNumberOfLayers () 
```




<hr>



### function GetPath 

```C++
inline std::filesystem::path AGE::Tilemap::GetPath () const
```




<hr>



### function GetScene 

```C++
inline Ref< Scene > AGE::Tilemap::GetScene () 
```




<hr>



### function GetUVs 

```C++
inline std::map< uint32_t, std::vector< Vector2 * > > & AGE::Tilemap::GetUVs () 
```




<hr>



### function SetPath 

```C++
inline void AGE::Tilemap::SetPath (
    const std::filesystem::path & Path
) 
```




<hr>



### function SetScene 

```C++
void AGE::Tilemap::SetScene (
    Ref< Scene > & scene
) 
```




<hr>



### function SetShaderData 

```C++
void AGE::Tilemap::SetShaderData () 
```




<hr>



### function SetTileLocations 

```C++
void AGE::Tilemap::SetTileLocations () 
```




<hr>



### function Tilemap 

```C++
AGE::Tilemap::Tilemap (
    tmx_map * Map
) 
```




<hr>



### function ~Tilemap 

```C++
AGE::Tilemap::~Tilemap () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/TileMap/Public/Tilemap.h`

