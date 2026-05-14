

# Class AGE::SpriteSheetUtils



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SpriteSheetUtils**](class_a_g_e_1_1_sprite_sheet_utils.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**SetTexCoords**](#function-settexcoords) (const Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; SubTex, [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) & Properties, bool Reverse=false) <br>_Sets the texture coordinates for a quad based on a subtexture and whether to reverse the order of the tex coords._  |


























## Public Static Functions Documentation




### function SetTexCoords 

_Sets the texture coordinates for a quad based on a subtexture and whether to reverse the order of the tex coords._ 
```C++
static void AGE::SpriteSheetUtils::SetTexCoords (
    const Ref< SubTexture2D > SubTex,
    QuadProperties & Properties,
    bool Reverse=false
) 
```





**Parameters:**


* `SubTex` A reference to the subtexture from which to get the tex coords. 
* `Properties` The [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object that holds the texture coordinates. 
* [**Reverse**](class_a_g_e_1_1_reverse.md) A boolean indicating whether or not to reverse the order of the tex coords.

Sets the texture coordinates for a quad based on a subtexture and whether to reverse the order of the tex coords.




**Parameters:**


* `SubTex` The subtexture from which to get the texture coordinates. 
* `Properties` A reference to the [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object that holds the texture coordinates. 
* [**Reverse**](class_a_g_e_1_1_reverse.md) A boolean indicating whether or not to reverse the order of the tex coords. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Sprite/Public/SpriteAPI.h`

