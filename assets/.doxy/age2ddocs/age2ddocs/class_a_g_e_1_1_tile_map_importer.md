

# Class AGE::TileMapImporter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TileMapImporter**](class_a_g_e_1_1_tile_map_importer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  tmx\_map \* | [**ImportMap**](#function-importmap) (const std::string & FilePath) <br>_Import a tile map from the given file path._  |
|   | [**TileMapImporter**](#function-tilemapimporter-12) () = default<br>_Default constructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class._ |
|   | [**TileMapImporter**](#function-tilemapimporter-22) (const [**TileMapImporter**](class_a_g_e_1_1_tile_map_importer.md) &) = delete<br>_This function is a copy constructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class and it has been explicitly deleted to prevent copying of objects._ |
|   | [**~TileMapImporter**](#function-tilemapimporter) () = default<br>_Destructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class._ |




























## Public Functions Documentation




### function ImportMap 

_Import a tile map from the given file path._ 
```C++
tmx_map * AGE::TileMapImporter::ImportMap (
    const std::string & FilePath
) 
```



This function attempts to load a tmx\_map object from the provided file path. If the file path is empty or if there's an issue with loading the file, it returns nullptr. Otherwise, it logs that the map was loaded successfully and then returns the map.




**Parameters:**


* `FilePath` The path of the tile map file to load. 



**Returns:**

A pointer to a tmx\_map object representing the loaded tile map or nullptr if there's an issue with loading the file. 





        

<hr>



### function TileMapImporter [1/2]

_Default constructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class._
```C++
AGE::TileMapImporter::TileMapImporter () = default
```




<hr>



### function TileMapImporter [2/2]

_This function is a copy constructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class and it has been explicitly deleted to prevent copying of objects._
```C++
AGE::TileMapImporter::TileMapImporter (
    const TileMapImporter &
) = delete
```





**Parameters:**


* `other` The object to be copied.



**Returns:**

No return value as this function is declared '= delete'. 





        

<hr>



### function ~TileMapImporter 

_Destructor for the_ [_**TileMapImporter**_](class_a_g_e_1_1_tile_map_importer.md) _class._
```C++
AGE::TileMapImporter::~TileMapImporter () = default
```



This function is responsible for releasing any resources that were acquired during the lifetime of an instance of this class, such as memory or file handles. It does not perform any operations on the actual data contained within the object itself. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/TileMap/Public/TileMapImporter.h`

