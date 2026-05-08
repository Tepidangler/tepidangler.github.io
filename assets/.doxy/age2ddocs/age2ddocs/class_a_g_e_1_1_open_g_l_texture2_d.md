

# Class AGE::OpenGLTexture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md)








Inherits the following classes: [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) (uint32\_t Slot=0) override const<br> |
| virtual uint64\_t | [**GetAssetID**](#function-getassetid) () override const<br> |
| virtual uint32\_t | [**GetHeight**](#function-getheight) () override const<br> |
| virtual std::string | [**GetName**](#function-getname) () override const<br> |
| virtual uint32\_t | [**GetNrChannels**](#function-getnrchannels) () const<br> |
| virtual const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & | [**GetSpecification**](#function-getspecification) () override const<br> |
| virtual std::pair&lt; uint8\_t \*, size\_t &gt; | [**GetTextureData**](#function-gettexturedata) () override<br> |
| virtual std::string | [**GetTextureFilePath**](#function-gettexturefilepath) () override const<br> |
| virtual uint32\_t | [**GetTextureID**](#function-gettextureid) () override const<br> |
| virtual uint32\_t | [**GetWidth**](#function-getwidth) () override const<br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-15) (const std::string & Path) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-25) (uint8\_t \* Image, const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-35) (const std::vector&lt; std::string &gt; & Paths) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br> |
| virtual void | [**SetAssetID**](#function-setassetid) (uint64\_t ID) override<br> |
| virtual void | [**SetData**](#function-setdata) (void \* Data, uint32\_t Size) override<br> |
| virtual void | [**SetName**](#function-setname) (const std::string & Name) override<br> |
| virtual void | [**SetTextureFilePath**](#function-settexturefilepath) (const std::string & Path) override<br> |
| virtual void | [**Unbind**](#function-unbind) () override const<br> |
| virtual bool | [**operator==**](#function-operator) (const [**Texture**](class_a_g_e_1_1_texture.md) & Other) override const<br> |
|   | [**~OpenGLTexture2D**](#function-opengltexture2d) () <br> |


## Public Functions inherited from AGE::Texture2D

See [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_texture2_d.md#function-as) () <br> |


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




## Public Static Functions inherited from AGE::Texture2D

See [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-15) (const std::string & Path) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-25) (uint8\_t \* Image, const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-35) (const std::vector&lt; std::string &gt; & Path) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br> |












































































## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::OpenGLTexture2D::Bind (
    uint32_t Slot=0
) override const
```



Implements [*AGE::Texture::Bind*](class_a_g_e_1_1_texture.md#function-bind)


<hr>



### function GetAssetID 

```C++
inline virtual uint64_t AGE::OpenGLTexture2D::GetAssetID () override const
```



Implements [*AGE::Texture::GetAssetID*](class_a_g_e_1_1_texture.md#function-getassetid)


<hr>



### function GetHeight 

```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetHeight () override const
```



Implements [*AGE::Texture::GetHeight*](class_a_g_e_1_1_texture.md#function-getheight)


<hr>



### function GetName 

```C++
inline virtual std::string AGE::OpenGLTexture2D::GetName () override const
```



Implements [*AGE::Texture::GetName*](class_a_g_e_1_1_texture.md#function-getname)


<hr>



### function GetNrChannels 

```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetNrChannels () const
```




<hr>



### function GetSpecification 

```C++
inline virtual const TextureSpecification & AGE::OpenGLTexture2D::GetSpecification () override const
```



Implements [*AGE::Texture::GetSpecification*](class_a_g_e_1_1_texture.md#function-getspecification)


<hr>



### function GetTextureData 

```C++
inline virtual std::pair< uint8_t *, size_t > AGE::OpenGLTexture2D::GetTextureData () override
```



Implements [*AGE::Texture::GetTextureData*](class_a_g_e_1_1_texture.md#function-gettexturedata)


<hr>



### function GetTextureFilePath 

```C++
inline virtual std::string AGE::OpenGLTexture2D::GetTextureFilePath () override const
```



Implements [*AGE::Texture::GetTextureFilePath*](class_a_g_e_1_1_texture.md#function-gettexturefilepath)


<hr>



### function GetTextureID 

```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetTextureID () override const
```



Implements [*AGE::Texture::GetTextureID*](class_a_g_e_1_1_texture.md#function-gettextureid)


<hr>



### function GetWidth 

```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetWidth () override const
```



Implements [*AGE::Texture::GetWidth*](class_a_g_e_1_1_texture.md#function-getwidth)


<hr>



### function OpenGLTexture2D [1/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const std::string & Path
) 
```




<hr>



### function OpenGLTexture2D [2/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    uint8_t * Image,
    const TextureSpecification & Spec
) 
```




<hr>



### function OpenGLTexture2D [3/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const std::vector< std::string > & Paths
) 
```




<hr>



### function OpenGLTexture2D [4/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const TextureSpecification & Spec
) 
```




<hr>



### function OpenGLTexture2D [5/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const Image * Img,
    uint32_t Width,
    uint32_t Height,
    int Channels,
    size_t Size
) 
```




<hr>



### function SetAssetID 

```C++
inline virtual void AGE::OpenGLTexture2D::SetAssetID (
    uint64_t ID
) override
```



Implements [*AGE::Texture::SetAssetID*](class_a_g_e_1_1_texture.md#function-setassetid)


<hr>



### function SetData 

```C++
virtual void AGE::OpenGLTexture2D::SetData (
    void * Data,
    uint32_t Size
) override
```



Implements [*AGE::Texture::SetData*](class_a_g_e_1_1_texture.md#function-setdata)


<hr>



### function SetName 

```C++
inline virtual void AGE::OpenGLTexture2D::SetName (
    const std::string & Name
) override
```



Implements [*AGE::Texture::SetName*](class_a_g_e_1_1_texture.md#function-setname)


<hr>



### function SetTextureFilePath 

```C++
inline virtual void AGE::OpenGLTexture2D::SetTextureFilePath (
    const std::string & Path
) override
```



Implements [*AGE::Texture::SetTextureFilePath*](class_a_g_e_1_1_texture.md#function-settexturefilepath)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLTexture2D::Unbind () override const
```



Implements [*AGE::Texture::Unbind*](class_a_g_e_1_1_texture.md#function-unbind)


<hr>



### function operator== 

```C++
inline virtual bool AGE::OpenGLTexture2D::operator== (
    const Texture & Other
) override const
```



Implements [*AGE::Texture::operator==*](class_a_g_e_1_1_texture.md#function-operator)


<hr>



### function ~OpenGLTexture2D 

```C++
AGE::OpenGLTexture2D::~OpenGLTexture2D () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLTexture.h`

