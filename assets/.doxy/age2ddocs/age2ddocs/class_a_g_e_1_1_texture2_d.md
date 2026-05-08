

# Class AGE::Texture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Texture2D**](class_a_g_e_1_1_texture2_d.md)








Inherits the following classes: [AGE::Texture](class_a_g_e_1_1_texture.md)


Inherited by the following classes: [AGE::OpenGLTexture2D](class_a_g_e_1_1_open_g_l_texture2_d.md)




















































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br> |


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
| virtual  | [**~Texture**](class_a_g_e_1_1_texture.md#function-texture) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-15) (const std::string & Path) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-25) (uint8\_t \* Image, const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-35) (const std::vector&lt; std::string &gt; & Path) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](#function-create-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br> |




















































## Public Functions Documentation




### function As 

```C++
template<typename T>
T * AGE::Texture2D::As () 
```




<hr>
## Public Static Functions Documentation




### function Create [1/5]

```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const std::string & Path
) 
```




<hr>



### function Create [2/5]

```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    uint8_t * Image,
    const TextureSpecification & Spec
) 
```




<hr>



### function Create [3/5]

```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const std::vector< std::string > & Path
) 
```




<hr>



### function Create [4/5]

```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const TextureSpecification & Spec
) 
```




<hr>



### function Create [5/5]

```C++
static Ref< Texture2D > AGE::Texture2D::Create (
    const Image * Img,
    uint32_t Width,
    uint32_t Height,
    int Channels,
    size_t Size
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/Texture.h`

