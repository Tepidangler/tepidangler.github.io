

# Class AGE::Texture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Texture2D**](class_a_g_e_1_1_texture2_d.md)








Inherits the following classes: [AGE::Texture](class_a_g_e_1_1_texture.md)


Inherited by the following classes: [AGE::OpenGLTexture2D](class_a_g_e_1_1_open_g_l_texture2_d.md)




















































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br>_This function is currently not implemented. It will return a pointer to an object of type T. If called, it will assert and crash the program with the message "As() Failed!"._  |


## Public Functions inherited from AGE::Texture

See [AGE::Texture](class_a_g_e_1_1_texture.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](class_a_g_e_1_1_texture.md#function-bind) (uint32\_t Slot=0) const = 0<br> |
| virtual uint64\_t | [**GetAssetID**](class_a_g_e_1_1_texture.md#function-getassetid) () const = 0<br> |
| virtual uint32\_t | [**GetHeight**](class_a_g_e_1_1_texture.md#function-getheight) () const = 0<br> |
| virtual std::string | [**GetName**](class_a_g_e_1_1_texture.md#function-getname) () const = 0<br> |
| virtual const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & | [**GetSpecification**](class_a_g_e_1_1_texture.md#function-getspecification) () const = 0<br> |
| virtual std::pair&lt; uint8\_t \*, size\_t &gt; | [**GetTextureData**](class_a_g_e_1_1_texture.md#function-gettexturedata) () = 0<br> |
| virtual std::string | [**GetTextureFilePath**](class_a_g_e_1_1_texture.md#function-gettexturefilepath) () const = 0<br> |
| virtual uint32\_t | [**GetTextureID**](class_a_g_e_1_1_texture.md#function-gettextureid) () const = 0<br> |
| virtual uint32\_t | [**GetWidth**](class_a_g_e_1_1_texture.md#function-getwidth) () const = 0<br> |
| virtual void | [**SetAssetID**](class_a_g_e_1_1_texture.md#function-setassetid) (uint64\_t ID) = 0<br> |
| virtual void | [**SetData**](class_a_g_e_1_1_texture.md#function-setdata) (void \* Data, uint32\_t Size) = 0<br> |
| virtual void | [**SetName**](class_a_g_e_1_1_texture.md#function-setname) (const std::string & Name) = 0<br> |
| virtual void | [**SetTextureFilePath**](class_a_g_e_1_1_texture.md#function-settexturefilepath) (const std::string & Path) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_texture.md#function-unbind) () const = 0<br> |
| virtual bool | [**operator==**](class_a_g_e_1_1_texture.md#function-operator) (const [**Texture**](class_a_g_e_1_1_texture.md) & Other) const = 0<br> |
| virtual  | [**~Texture**](class_a_g_e_1_1_texture.md#function-texture) () <br>_Virtual destructor for the_ [_**Texture**_](class_a_g_e_1_1_texture.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-15) (const std::string & Path) <br>_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-25) (const tmx\_image \* Image) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the current Rendering API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-35) (const std::vector&lt; std::string &gt; & Path) <br>_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of texture is determined by the current renderer API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the given specification. The type of texture to be created is determined by the current renderer API in use._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._ |




















































## Public Functions Documentation




### function As 

_This function is currently not implemented. It will return a pointer to an object of type T. If called, it will assert and crash the program with the message "As() Failed!"._ 
```C++
template<typename T>
T * AGE::Texture2D::As () 
```





**Returns:**

nullptr Always returns nullptr.


This function is currently not implemented. It will return a pointer to an object of type T. If this function is called, it will assert and crash the program with the message "As() Failed!".




**Returns:**

nullptr Always returns nullptr. 





        

<hr>
## Public Static Functions Documentation




### function Create [1/5]

_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._
```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const std::string & Path
) 
```





**Parameters:**


* `Path` The path to the image file for the texture. 



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, or nullptr if an unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is used.


Creates a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. The type of the texture is determined by the current renderer API. 

**Parameters:**


* `Path` The path to the image file for the texture. 



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, or nullptr if an unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is used. 





        

<hr>



### function Create [2/5]

_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the current Rendering API._
```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const tmx_image * Image
) 
```



This function creates and returns a reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, which is specific to the currently used rendering API. It takes as input a pointer to an image data structure (tmx\_image). The type of texture created will depend on the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use. If no supported Rendering API is found, it asserts false and returns nullptr.




**Parameters:**


* [**Image**](class_a_g_e_1_1_image.md) Pointer to the image data that the [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object should be based on.



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object of the appropriate type for the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use. If no supported API is found, it returns nullptr. 





        

<hr>



### function Create [3/5]

_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of texture is determined by the current renderer API._
```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const std::vector< std::string > & Path
) 
```





**Parameters:**


* `Paths` A vector of strings representing the paths to the textures. 



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, or nullptr if an unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is encountered.


Creates a texture from file path(s). The type of the texture depends on the current renderer API.




**Parameters:**


* `Paths` A vector of strings representing the paths to the textures. 



**Returns:**

Ref&lt;Texture2D&gt; A reference to the created [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. Returns nullptr if the RendererAPI::API is None or Unknown. 





        

<hr>



### function Create [4/5]

_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the given specification. The type of texture to be created is determined by the current renderer API in use._
```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const TextureSpecification & Spec
) 
```





**Parameters:**


* `Spec` The specification for the texture to be created. This includes things like width, height, format etc. 



**Returns:**

A reference to the newly created [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. If no suitable [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is found or an error occurs during creation, a null reference is returned.


Creates a new [**Texture2D**](class_a_g_e_1_1_texture2_d.md) based on the specified specification.


The type of texture is determined by the current [**Renderer**](class_a_g_e_1_1_renderer.md) API in use. If no supported API is found, an assertion error will be thrown.




**Parameters:**


* `Spec` The specification for the texture to be created. This includes details like width, height, format etc. 



**Returns:**

A reference to the newly created [**Texture2D**](class_a_g_e_1_1_texture2_d.md) instance. 





        

<hr>



### function Create [5/5]

_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._
```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const Image * Img,
    uint32_t Width,
    uint32_t Height,
    int Channels,
    size_t Size
) 
```





**Parameters:**


* `Img` Pointer to an [**Image**](class_a_g_e_1_1_image.md) object, can be null if only dimensions are specified. 
* `Width` Width of the texture in pixels. 
* `Height` Height of the texture in pixels. 
* `Channels` Number of color channels in the image data. 
* `Size` Total size of the image data in bytes. 



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object, or nullptr if an unsupported [**Renderer**](class_a_g_e_1_1_renderer.md) API is used.


Creates a new [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object. The type of texture to be created is determined by the current renderer API in use.




**Parameters:**


* `Img` Pointer to an [**Image**](class_a_g_e_1_1_image.md) object, which may contain pixel data for initializing the texture. Can be nullptr if no image data is provided. 
* `Width` Width of the texture in pixels. 
* `Height` Height of the texture in pixels. 
* `Channels` Number of color channels in the texture (e.g., 3 for RGB, 4 for RGBA). 
* `Size` Total size of the image data in bytes.



**Returns:**

A reference to a [**Texture2D**](class_a_g_e_1_1_texture2_d.md) object that has been created based on the current [**Renderer**](class_a_g_e_1_1_renderer.md) API. If an unsupported or unknown [**Renderer**](class_a_g_e_1_1_renderer.md) API is detected, nullptr is returned instead. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/Texture.h`

