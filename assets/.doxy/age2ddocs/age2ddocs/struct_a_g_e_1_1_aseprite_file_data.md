

# Struct AGE::AsepriteFileData



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) &gt; | [**Frames**](#variable-frames)  <br> |
|  [**AsepriteHeader**](struct_a_g_e_1_1_aseprite_header.md) | [**Header**](#variable-header)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AsepriteFileData**](#function-asepritefiledata-13) () = default<br>_Default constructor for_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class._ |
|   | [**AsepriteFileData**](#function-asepritefiledata-23) (const [**AsepriteHeader**](struct_a_g_e_1_1_aseprite_header.md) & HeaderData) <br>_Constructs an instance of the_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class using a const reference to an_[_**AsepriteHeader**_](struct_a_g_e_1_1_aseprite_header.md) _object._ |
|   | [**AsepriteFileData**](#function-asepritefiledata-33) (const [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) &) = default<br>_Default copy constructor for the_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class._ |




























## Public Attributes Documentation




### variable Frames 

```C++
std::vector<AsepriteFrameData> AGE::AsepriteFileData::Frames;
```




<hr>



### variable Header 

```C++
AsepriteHeader AGE::AsepriteFileData::Header;
```




<hr>
## Public Functions Documentation




### function AsepriteFileData [1/3]

_Default constructor for_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class._
```C++
AGE::AsepriteFileData::AsepriteFileData () = default
```



This function initializes an instance of the [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) class with default values. It is used to create a new object without any specific initialization.




**Returns:**

An instance of [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) with all fields initialized to their default values. 





        

<hr>



### function AsepriteFileData [2/3]

_Constructs an instance of the_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class using a const reference to an_[_**AsepriteHeader**_](struct_a_g_e_1_1_aseprite_header.md) _object._
```C++
inline AGE::AsepriteFileData::AsepriteFileData (
    const AsepriteHeader & HeaderData
) 
```





**Parameters:**


* `HeaderData` A const reference to an [**AsepriteHeader**](struct_a_g_e_1_1_aseprite_header.md) object containing header data for the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file. 




        

<hr>



### function AsepriteFileData [3/3]

_Default copy constructor for the_ [_**AsepriteFileData**_](struct_a_g_e_1_1_aseprite_file_data.md) _class._
```C++
AGE::AsepriteFileData::AsepriteFileData (
    const AsepriteFileData &
) = default
```



This function is used to create a new instance of [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) by copying an existing one. It uses the '= default' syntax, which tells the compiler to generate the body of this function using the default behavior provided by the compiler.




**Parameters:**


* `other` The existing [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) instance to copy. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

