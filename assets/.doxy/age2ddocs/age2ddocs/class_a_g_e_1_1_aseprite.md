

# Class AGE::Aseprite



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Aseprite**](class_a_g_e_1_1_aseprite.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Aseprite**](#function-aseprite-13) () = default<br> |
|   | [**Aseprite**](#function-aseprite-23) (const [**Aseprite**](class_a_g_e_1_1_aseprite.md) &) = delete<br> |
|   | [**Aseprite**](#function-aseprite-33) (const [**Aseprite**](class_a_g_e_1_1_aseprite.md) &&) = delete<br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**CreateImage**](#function-createimage) (const std::string & Filename, bool ShouldCreateTexture, bool ShouldFlipOnLoad=false) <br> |
|  void | [**ReadData**](#function-readdata) (const std::filesystem::path & Filepath) <br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
|  std::vector&lt; [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) &gt; & | [**GetSpriteFrameData**](#function-getspriteframedata) (const std::string & SpriteName) <br> |




## Public Functions Documentation




### function Aseprite [1/3]

```C++
AGE::Aseprite::Aseprite () = default
```




<hr>



### function Aseprite [2/3]

```C++
AGE::Aseprite::Aseprite (
    const Aseprite &
) = delete
```




<hr>



### function Aseprite [3/3]

```C++
AGE::Aseprite::Aseprite (
    const Aseprite &&
) = delete
```




<hr>



### function CreateImage 

```C++
Ref< Texture2D > AGE::Aseprite::CreateImage (
    const std::string & Filename,
    bool ShouldCreateTexture,
    bool ShouldFlipOnLoad=false
) 
```




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

```C++
std::vector< AsepriteFrameData > & AGE::Aseprite::GetSpriteFrameData (
    const std::string & SpriteName
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/Aseprite.h`

