

# Class AGE::AssetPak



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AssetPak**](class_a_g_e_1_1_asset_pak.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AssetPak**](#function-assetpak-13) () = default<br>_Default constructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._ |
|   | [**AssetPak**](#function-assetpak-23) (const [**AssetPak**](class_a_g_e_1_1_asset_pak.md) &) = delete<br>_This function is a copy constructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class and it has been explicitly deleted to prevent copying of objects._ |
|   | [**AssetPak**](#function-assetpak-33) ([**AssetPak**](class_a_g_e_1_1_asset_pak.md) &&) = delete<br>_Move constructor for_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._ |
|   | [**~AssetPak**](#function-assetpak) () = default<br>_Default destructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._ |




























## Public Functions Documentation




### function AssetPak [1/3]

_Default constructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._
```C++
AGE::AssetPak::AssetPak () = default
```




<hr>



### function AssetPak [2/3]

_This function is a copy constructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class and it has been explicitly deleted to prevent copying of objects._
```C++
AGE::AssetPak::AssetPak (
    const AssetPak &
) = delete
```





**Parameters:**


* `other` The object to be copied. 




        

<hr>



### function AssetPak [3/3]

_Move constructor for_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._
```C++
AGE::AssetPak::AssetPak (
    AssetPak &&
) = delete
```



This function is marked as deleted to prevent copying of [**AssetPak**](class_a_g_e_1_1_asset_pak.md) objects, which would not be efficient or safe. It should only be used when moving an existing object into a new one.




**Parameters:**


* `other` The temporary object being moved from. 




        

<hr>



### function ~AssetPak 

_Default destructor for the_ [_**AssetPak**_](class_a_g_e_1_1_asset_pak.md) _class._
```C++
AGE::AssetPak::~AssetPak () = default
```



This function is used to clean up any resources that are being held by an instance of the [**AssetPak**](class_a_g_e_1_1_asset_pak.md) class. It should be called when an object of this class is no longer needed, to ensure proper memory management and prevent potential issues with dangling pointers or other resource leaks. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Assets/Public/AssetManager.h`

