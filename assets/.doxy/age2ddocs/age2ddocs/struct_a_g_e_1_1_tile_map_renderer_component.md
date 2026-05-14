

# Struct AGE::TileMapRendererComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**Name**](#variable-name)  <br> |
|  Ref&lt; [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; | [**TileMap**](#variable-tilemap)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; | [**GetTileMap**](#function-gettilemap) () <br>_Returns the tile map object._  |
|  void | [**SetTileMap**](#function-settilemap) (Ref&lt; [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; Map) <br>_Sets the TileMap for this object._  |
|   | [**TileMapRendererComponent**](#function-tilemaprenderercomponent-13) () = default<br>_Default constructor for_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _class._ |
|   | [**TileMapRendererComponent**](#function-tilemaprenderercomponent-23) (const [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md) &) = default<br>_Default copy constructor for the_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _class._ |
|   | [**TileMapRendererComponent**](#function-tilemaprenderercomponent-33) (const std::string & N) <br>_Constructs a_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _with the given name._ |




























## Public Attributes Documentation




### variable Name 

```C++
std::string AGE::TileMapRendererComponent::Name;
```




<hr>



### variable TileMap 

```C++
Ref<Tilemap> AGE::TileMapRendererComponent::TileMap;
```




<hr>
## Public Functions Documentation




### function GetTileMap 

_Returns the tile map object._ 
```C++
inline Ref< Tilemap > AGE::TileMapRendererComponent::GetTileMap () 
```



This function retrieves and returns the tile map object stored in the game state. The returned object can be used to access and manipulate the tile map data.




**Returns:**

Ref&lt;Tilemap&gt; A reference to the tile map object. 





        

<hr>



### function SetTileMap 

_Sets the TileMap for this object._ 
```C++
inline void AGE::TileMapRendererComponent::SetTileMap (
    Ref< Tilemap > Map
) 
```



This function sets the TileMap property of the current object to a new value. The new map is passed as an argument.




**Parameters:**


* `Map` A reference to the new [**Tilemap**](class_a_g_e_1_1_tilemap.md) that will replace the old one. 




        

<hr>



### function TileMapRendererComponent [1/3]

_Default constructor for_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _class._
```C++
AGE::TileMapRendererComponent::TileMapRendererComponent () = default
```




<hr>



### function TileMapRendererComponent [2/3]

_Default copy constructor for the_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _class._
```C++
AGE::TileMapRendererComponent::TileMapRendererComponent (
    const TileMapRendererComponent &
) = default
```



This function is used to create a new instance of the [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The existing [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md) instance to copy. 




        

<hr>



### function TileMapRendererComponent [3/3]

_Constructs a_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _with the given name._
```C++
inline AGE::TileMapRendererComponent::TileMapRendererComponent (
    const std::string & N
) 
```





**Parameters:**


* `N` The name of the component. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

