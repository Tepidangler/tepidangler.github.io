

# Class AGE::FBXParser



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FBXParser**](#function-fbxparser) () = default<br>_Default constructor for the_ [_**FBXParser**_](class_a_g_e_1_1_f_b_x_parser.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**FreeScene**](#function-freescene) (ufbx\_scene \* scene) <br>_This function frees an allocated ufbx\_scene._  |
|  [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) & | [**Get**](#function-get) () <br>_This function returns a reference to the singleton instance of the_ [_**FBXParser**_](class_a_g_e_1_1_f_b_x_parser.md) _class. If an instance does not already exist, it will be created._ |
|  ufbx\_scene \* | [**LoadFile**](#function-loadfile) (const std::filesystem::path & Path) <br>_Loads a FBX file into memory and returns the loaded scene._  |


























## Public Functions Documentation




### function FBXParser 

_Default constructor for the_ [_**FBXParser**_](class_a_g_e_1_1_f_b_x_parser.md) _class._
```C++
AGE::FBXParser::FBXParser () = default
```



This function initializes an instance of the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) class with default values. It does not perform any specific operations or require any parameters to be set.




**Returns:**

A new instance of the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) class with all fields initialized to their default values.


Default constructor for the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) class. 


        

<hr>
## Public Static Functions Documentation




### function FreeScene 

_This function frees an allocated ufbx\_scene._ 
```C++
static void AGE::FBXParser::FreeScene (
    ufbx_scene * scene
) 
```





**Parameters:**


* `scene` Pointer to the ufbx\_scene that needs to be freed.



**Returns:**

None


This function frees an allocated ufbx\_scene. 

**Parameters:**


* `scene` Pointer to the ufbx\_scene that needs to be freed. 



**Returns:**

None 





        

<hr>



### function Get 

_This function returns a reference to the singleton instance of the_ [_**FBXParser**_](class_a_g_e_1_1_f_b_x_parser.md) _class. If an instance does not already exist, it will be created._
```C++
static inline FBXParser & AGE::FBXParser::Get () 
```





**Returns:**

A reference to the single instance of the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) class.


This function returns a reference to the singleton instance of the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) class. If an instance does not already exist, it will be created. 

**Returns:**

A reference to the [**FBXParser**](class_a_g_e_1_1_f_b_x_parser.md) instance. 





        

<hr>



### function LoadFile 

_Loads a FBX file into memory and returns the loaded scene._ 
```C++
static ufbx_scene * AGE::FBXParser::LoadFile (
    const std::filesystem::path & Path
) 
```



This function loads an FBX file from the specified path, adjusting transforms if necessary. The target axes are left-handed with Y as up, and the target unit is set to be 0.01 meters. If the loading fails for any reason, it logs an error message and returns nullptr.




**Parameters:**


* `Path` The file system path of the FBX file to load. 



**Returns:**

A pointer to the loaded ufbx\_scene if successful, otherwise nullptr.


Loads an FBX file into a ufbx\_scene object.


If the file cannot be loaded for any reason (e.g., it does not exist or is corrupt), an error message will be logged and nullptr will be returned. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Parser/Public/FbxParser.h`

