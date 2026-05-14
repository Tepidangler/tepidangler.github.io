

# Class AGE::TileMapManager



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**LoadTileMap**](#function-loadtilemap) (const std::filesystem::path & Path) <br>_Loads a tile map from the specified path into the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _._ |
|  void | [**LoadTileMaps**](#function-loadtilemaps-12) (const std::vector&lt; std::filesystem::path &gt; & Paths) <br>_Loads a list of tile maps from the given paths into the manager's collection._  |
|  void | [**LoadTileMaps**](#function-loadtilemaps-22) (void \* Addr) <br>_Loads the tile maps into memory from a specified address._  |
|   | [**TileMapManager**](#function-tilemapmanager) () <br>_Constructs a_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _object._ |
|   | [**~TileMapManager**](#function-tilemapmanager) () = default<br>_Default destructor for the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) & | [**Get**](#function-get) () <br>_Get the singleton instance of the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _. If it doesn't exist, create a new one._ |
|  void | [**ImageFree**](#function-imagefree) (void \* Address) <br>_Frees an image previously allocated with ImageAlloc._  |
|  void \* | [**ImageLoad**](#function-imageload) (const char \* Path) <br>_Loads an image from a specified path and creates a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object for it._ |


























## Public Functions Documentation




### function LoadTileMap 

_Loads a tile map from the specified path into the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _._
```C++
void AGE::TileMapManager::LoadTileMap (
    const std::filesystem::path & Path
) 
```



This function takes in a file system path, uses an importer to import the map data from that path, creates a new [**Tilemap**](class_a_g_e_1_1_tilemap.md) object with this imported data, sets its data (atlas texture and path) based on the current tile map's data, and then adds it to the list of tile maps.




**Parameters:**


* `Path` The file system path where the tile map is located. 



**Returns:**

void No return value. 





        

<hr>



### function LoadTileMaps [1/2]

_Loads a list of tile maps from the given paths into the manager's collection._ 
```C++
void AGE::TileMapManager::LoadTileMaps (
    const std::vector< std::filesystem::path > & Paths
) 
```



This function iterates over each path in the provided vector, imports the corresponding tile map using the importer, and adds it to the manager's collection. The imported tile map is then configured with the current atlas texture and path before being added to the collection.




**Parameters:**


* `Paths` A list of file paths representing the locations of the tile maps to be loaded. 




        

<hr>



### function LoadTileMaps [2/2]

_Loads the tile maps into memory from a specified address._ 
```C++
void AGE::TileMapManager::LoadTileMaps (
    void * Addr
) 
```



This function loads all the tile maps stored in memory at a given address. The address is passed as a void pointer, allowing for flexibility in terms of data types that can be loaded.




**Parameters:**


* `Addr` A pointer to the start of the tile map data. 




        

<hr>



### function TileMapManager 

_Constructs a_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _object._
```C++
AGE::TileMapManager::TileMapManager () 
```



This function initializes the [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) by creating an instance of `tmx_resource_manager` and assigning it to member variable `m_Manager`.


Constructs a [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) object. This function initializes the [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md), setting up the resource manager and tile map importer. 


        

<hr>



### function ~TileMapManager 

_Default destructor for the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _class._
```C++
AGE::TileMapManager::~TileMapManager () = default
```



This function is responsible for releasing any resources that were acquired by the [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) during its lifetime, such as memory or file handles. It does not perform any operations on the objects themselves.


Default destructor for [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md) class. 


        

<hr>
## Public Static Functions Documentation




### function Get 

_Get the singleton instance of the_ [_**TileMapManager**_](class_a_g_e_1_1_tile_map_manager.md) _. If it doesn't exist, create a new one._
```C++
static inline TileMapManager & AGE::TileMapManager::Get () 
```





**Returns:**

Reference to the single instance of [**TileMapManager**](class_a_g_e_1_1_tile_map_manager.md). 





        

<hr>



### function ImageFree 

_Frees an image previously allocated with ImageAlloc._ 
```C++
static void AGE::TileMapManager::ImageFree (
    void * Address
) 
```



This function takes a void pointer to an image that was previously allocated using the ImageAlloc function and frees it, effectively deallocating the memory used by this image. The size of the image is determined by sizeof(Texture2D).




**Parameters:**


* `Address` A void pointer to the image to be freed. This should have been obtained from a previous call to ImageAlloc. 




        

<hr>



### function ImageLoad 

_Loads an image from a specified path and creates a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object for it._
```C++
static void * AGE::TileMapManager::ImageLoad (
    const char * Path
) 
```



This function takes in a string representing the file path of the image to be loaded, loads this image using stb\_image library, generates a texture from the image data, and returns a void pointer to that texture.




**Parameters:**


* `Path` The file path of the image to load. 



**Returns:**

A void pointer to the created [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/TileMap/Public/TileMapManager.h`

