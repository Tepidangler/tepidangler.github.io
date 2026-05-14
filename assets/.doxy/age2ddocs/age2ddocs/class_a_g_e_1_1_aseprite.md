

# Class AGE::Aseprite



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Aseprite**](class_a_g_e_1_1_aseprite.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Aseprite**](#function-aseprite-13) () = default<br>_Default constructor for_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _class._ |
|   | [**Aseprite**](#function-aseprite-23) (const [**Aseprite**](class_a_g_e_1_1_aseprite.md) &) = delete<br>_Copy constructor for class_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _is deleted to prevent copying of objects._ |
|   | [**Aseprite**](#function-aseprite-33) (const [**Aseprite**](class_a_g_e_1_1_aseprite.md) &&) = delete<br>_This function is a move constructor for the class_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _and it's marked as deleted to prevent copying of objects._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**CreateImage**](#function-createimage) (const std::string & Filename, bool ShouldCreateTexture, bool ShouldFlipOnLoad=false) <br>_Creates an image from the given_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file._ _\ This function reads data from a specified_[_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file, processes it and creates an image object. The created image can optionally be converted into a texture._ _._ |
|  void | [**ReadData**](#function-readdata) (const std::filesystem::path & Filepath) <br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
|  std::vector&lt; [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) &gt; & | [**GetSpriteFrameData**](#function-getspriteframedata) (const std::string & SpriteName) <br>_Get the frame data of a specific sprite._  |




## Public Functions Documentation




### function Aseprite [1/3]

_Default constructor for_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _class._
```C++
AGE::Aseprite::Aseprite () = default
```



This function initializes an instance of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) class with its default values. It does not take any parameters and returns nothing.


Default constructor for [**Aseprite**](class_a_g_e_1_1_aseprite.md) class.


This function initializes an instance of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) class with its default values. 


        

<hr>



### function Aseprite [2/3]

_Copy constructor for class_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _is deleted to prevent copying of objects._
```C++
AGE::Aseprite::Aseprite (
    const Aseprite &
) = delete
```



The copy constructor is implicitly provided by the compiler, but it's not needed in this context as we don't want to allow copies of our [**Aseprite**](class_a_g_e_1_1_aseprite.md) objects. This function simply throws a compilation error if someone tries to use it.




**Parameters:**


* `other` The object being copied. Not used because copying is disabled.

Copy constructor for class [**Aseprite**](class_a_g_e_1_1_aseprite.md) is deleted to prevent copying.


This function is marked as deleted in the C++11 standard, which means that if an attempt is made to copy an object of this type, a compile-time error will be generated instead of a run-time exception.




**Parameters:**


* `other` The instance of [**Aseprite**](class_a_g_e_1_1_aseprite.md) to be copied. This parameter is named 'other' for clarity and it represents the instance being copied.



**Returns:**

No return value as this function does not provide any meaningful output. It simply prevents copying of objects of class [**Aseprite**](class_a_g_e_1_1_aseprite.md). 





        

<hr>



### function Aseprite [3/3]

_This function is a move constructor for the class_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _and it's marked as deleted to prevent copying of objects._
```C++
AGE::Aseprite::Aseprite (
    const Aseprite &&
) = delete
```





**Parameters:**


* `other` The object to be moved from.

This is a deleted copy constructor for the class [**Aseprite**](class_a_g_e_1_1_aseprite.md). It prevents copying of objects of this type. 

**Parameters:**


* `other` The object to be copied. 




        

<hr>



### function CreateImage 

_Creates an image from the given_ [_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file._ _\ This function reads data from a specified_[_**Aseprite**_](class_a_g_e_1_1_aseprite.md) _file, processes it and creates an image object. The created image can optionally be converted into a texture._ _._
```C++
Ref< Texture2D > AGE::Aseprite::CreateImage (
    const std::string & Filename,
    bool ShouldCreateTexture,
    bool ShouldFlipOnLoad=false
) 
```




 \ 

**Parameters:**


* `Filename` The name of the [**Aseprite**](class_a_g_e_1_1_aseprite.md) file to read from.
 \ 
* `ShouldCreateTexture` If true, a texture will be created from the image data. Otherwise, only the image object is returned.
 \ 
* `ShouldFlipOnLoad` If true, the loaded image will be flipped vertically.
 \ 



**Returns:**

A reference to the created image or texture (if any). Returns nullptr if no image was created and the function should not create a texture.
 \ 





        

<hr>



### function ReadData 

```C++
void AGE::Aseprite::ReadData (
    const std::filesystem::path & Filepath
) 
```




<hr>
## Protected Functions Documentation




### function GetSpriteFrameData 

_Get the frame data of a specific sprite._ 
```C++
std::vector< AsepriteFrameData > & AGE::Aseprite::GetSpriteFrameData (
    const std::string & SpriteName
) 
```



This function retrieves the frame data for a given sprite name from the [**Aseprite**](class_a_g_e_1_1_aseprite.md) data map. If the sprite does not exist in the map, an exception is thrown.




**Parameters:**


* `SpriteName` The name of the sprite to retrieve the frame data for. 



**Returns:**

Reference to the vector of frames associated with the given sprite name. 




**Exception:**


* `std::out_of_range` If the provided sprite name does not exist in the [**Aseprite**](class_a_g_e_1_1_aseprite.md) data map.

Get the frame data of a specific sprite.


This function retrieves the frame data for a given sprite name from the [**Aseprite**](class_a_g_e_1_1_aseprite.md) data map. If the sprite does not exist, it will return an empty vector.




**Parameters:**


* `SpriteName` The name of the sprite to retrieve the frame data for. 



**Returns:**

std::vector&lt;AsepriteFrameData&gt;& Reference to the frame data vector of the specified sprite. If the sprite does not exist, it will return an empty vector. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Aseprite.h`

