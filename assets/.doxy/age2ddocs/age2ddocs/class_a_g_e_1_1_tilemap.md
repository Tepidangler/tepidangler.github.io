

# Class AGE::Tilemap



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Tilemap**](class_a_g_e_1_1_tilemap.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetAssetID**](#function-getassetid) () <br>_This function returns the asset ID of an object._  |
|  std::filesystem::path | [**GetPath**](#function-getpath) () const<br>_Returns the path stored in the object._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; | [**GetScene**](#function-getscene) () <br>_Retrieves the current scene object._  |
|  Ref&lt; [**Texture**](class_a_g_e_1_1_texture.md) &gt; | [**GetTexture**](#function-gettexture) () <br>_Gets the texture associated with this_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object._ |
|  void | [**SetData**](#function-setdata) (Ref&lt; [**Texture**](class_a_g_e_1_1_texture.md) &gt; Atlas, std::filesystem::path & path) <br>_Sets the data for the tilemap._  |
|  void | [**SetScene**](#function-setscene) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br>_Sets the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _for the_[_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object._ |
|   | [**Tilemap**](#function-tilemap) (tmx\_map \* Map) <br>_Constructs a_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object from a tmx\_map pointer._ |
|   | [**~Tilemap**](#function-tilemap) () <br>_Destructor for the_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _class._ |




























## Public Functions Documentation




### function GetAssetID 

_This function returns the asset ID of an object._ 
```C++
inline UUID AGE::Tilemap::GetAssetID () 
```





**Returns:**

[**UUID**](class_a_g_e_1_1_u_u_i_d.md) The unique identifier for the asset. 





        

<hr>



### function GetPath 

_Returns the path stored in the object._ 
```C++
inline std::filesystem::path AGE::Tilemap::GetPath () const
```





**Returns:**

The path as a std::filesystem::path object. 





        

<hr>



### function GetScene 

_Retrieves the current scene object._ 
```C++
inline Ref< Scene > AGE::Tilemap::GetScene () 
```



This function returns a reference to the currently active scene in the application. The returned [**Scene**](class_a_g_e_1_1_scene.md) object can be used for various operations such as rendering, updating, and interacting with the objects within it.




**Returns:**

A reference to the current scene (Ref&lt;Scene&gt;). If no scene is set, this function will return an empty reference. 





        

<hr>



### function GetTexture 

_Gets the texture associated with this_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object._
```C++
inline Ref< Texture > AGE::Tilemap::GetTexture () 
```





**Returns:**

A reference to the [**Texture**](class_a_g_e_1_1_texture.md) object that is used by this [**Tilemap**](class_a_g_e_1_1_tilemap.md). 





        

<hr>



### function SetData 

_Sets the data for the tilemap._ 
```C++
void AGE::Tilemap::SetData (
    Ref< Texture > Atlas,
    std::filesystem::path & path
) 
```



This function sets the texture atlas and file path for the tilemap. The Atlas parameter is moved into the m\_AtlasTexture member variable, while the path parameter is assigned to m\_Path. After this operation, both parameters are cleared. 

**Parameters:**


* `Atlas` A reference to a [**Texture**](class_a_g_e_1_1_texture.md) object that will be used as the texture atlas for the tilemap. 
* `path` The file path of the tilemap data. 




        

<hr>



### function SetScene 

_Sets the_ [_**Scene**_](class_a_g_e_1_1_scene.md) _for the_[_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object._
```C++
void AGE::Tilemap::SetScene (
    Ref< Scene > scene
) 
```



This function sets the [**Scene**](class_a_g_e_1_1_scene.md) member variable of the [**Tilemap**](class_a_g_e_1_1_tilemap.md) class to a given Ref&lt;Scene&gt; object. It takes in one parameter, which is the new scene that will be set.




**Parameters:**


* `scene` The new [**Scene**](class_a_g_e_1_1_scene.md) to be set for the [**Tilemap**](class_a_g_e_1_1_tilemap.md) object. 




        

<hr>



### function Tilemap 

_Constructs a_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _object from a tmx\_map pointer._
```C++
AGE::Tilemap::Tilemap (
    tmx_map * Map
) 
```



This function takes in a pointer to a tmx\_map structure and assigns it to the member variable m\_Map. The purpose of this constructor is to initialize an instance of the [**Tilemap**](class_a_g_e_1_1_tilemap.md) class with a map data structure.




**Parameters:**


* `Map` Pointer to a tmx\_map object containing the map data. 




        

<hr>



### function ~Tilemap 

_Destructor for the_ [_**Tilemap**_](class_a_g_e_1_1_tilemap.md) _class._
```C++
AGE::Tilemap::~Tilemap () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/TileMap/Public/Tilemap.h`

