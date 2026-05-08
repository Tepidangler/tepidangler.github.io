

# Class AGE::TileMapManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; | [**LoadTileMap**](#function-loadtilemap) (const std::filesystem::path & Path) <br> |
|  void | [**LoadTileMaps**](#function-loadtilemaps-12) (const std::vector&lt; std::filesystem::path &gt; & Paths) <br> |
|  void | [**LoadTileMaps**](#function-loadtilemaps-22) (void \* Addr) <br> |
|   | [**TileMapManager**](#function-tilemapmanager) () <br> |
|   | [**~TileMapManager**](#function-tilemapmanager) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) & | [**Get**](#function-get) () <br> |
|  void | [**ImageFree**](#function-imagefree) (void \* Address) <br> |
|  void \* | [**ImageLoad**](#function-imageload) (const char \* Path) <br> |


























## Public Functions Documentation




### function LoadTileMap 

```C++
Ref< Tilemap > AGE::TileMapManager::LoadTileMap (
    const std::filesystem::path & Path
) 
```




<hr>



### function LoadTileMaps [1/2]

```C++
void AGE::TileMapManager::LoadTileMaps (
    const std::vector< std::filesystem::path > & Paths
) 
```




<hr>



### function LoadTileMaps [2/2]

```C++
void AGE::TileMapManager::LoadTileMaps (
    void * Addr
) 
```




<hr>



### function TileMapManager 

```C++
AGE::TileMapManager::TileMapManager () 
```




<hr>



### function ~TileMapManager 

```C++
AGE::TileMapManager::~TileMapManager () = default
```




<hr>
## Public Static Functions Documentation




### function Get 

```C++
static inline TileMapManager & AGE::TileMapManager::Get () 
```




<hr>



### function ImageFree 

```C++
static void AGE::TileMapManager::ImageFree (
    void * Address
) 
```




<hr>



### function ImageLoad 

```C++
static void * AGE::TileMapManager::ImageLoad (
    const char * Path
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/TileMap/Public/TileMapManager.h`

