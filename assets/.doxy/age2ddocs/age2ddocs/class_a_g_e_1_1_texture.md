

# Class AGE::Texture



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Texture**](class_a_g_e_1_1_texture.md)










Inherited by the following classes: [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) (uint32\_t Slot=0) const = 0<br> |
| virtual uint64\_t | [**GetAssetID**](#function-getassetid) () const = 0<br> |
| virtual uint32\_t | [**GetHeight**](#function-getheight) () const = 0<br> |
| virtual std::string | [**GetName**](#function-getname) () const = 0<br> |
| virtual const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & | [**GetSpecification**](#function-getspecification) () const = 0<br> |
| virtual std::pair&lt; uint8\_t \*, size\_t &gt; | [**GetTextureData**](#function-gettexturedata) () = 0<br> |
| virtual std::string | [**GetTextureFilePath**](#function-gettexturefilepath) () const = 0<br> |
| virtual uint32\_t | [**GetTextureID**](#function-gettextureid) () const = 0<br> |
| virtual uint32\_t | [**GetWidth**](#function-getwidth) () const = 0<br> |
| virtual void | [**SetAssetID**](#function-setassetid) (uint64\_t ID) = 0<br> |
| virtual void | [**SetData**](#function-setdata) (void \* Data, uint32\_t Size) = 0<br> |
| virtual void | [**SetName**](#function-setname) (const std::string & Name) = 0<br> |
| virtual void | [**SetTextureFilePath**](#function-settexturefilepath) (const std::string & Path) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual bool | [**operator==**](#function-operator) (const [**Texture**](class_a_g_e_1_1_texture.md) & Other) const = 0<br> |
| virtual  | [**~Texture**](#function-texture) () <br>_Virtual destructor for the_ [_**Texture**_](class_a_g_e_1_1_texture.md) _class._ |




























## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::Texture::Bind (
    uint32_t Slot=0
) const = 0
```




<hr>



### function GetAssetID 

```C++
virtual uint64_t AGE::Texture::GetAssetID () const = 0
```




<hr>



### function GetHeight 

```C++
virtual uint32_t AGE::Texture::GetHeight () const = 0
```




<hr>



### function GetName 

```C++
virtual std::string AGE::Texture::GetName () const = 0
```




<hr>



### function GetSpecification 

```C++
virtual const TextureSpecification & AGE::Texture::GetSpecification () const = 0
```




<hr>



### function GetTextureData 

```C++
virtual std::pair< uint8_t *, size_t > AGE::Texture::GetTextureData () = 0
```




<hr>



### function GetTextureFilePath 

```C++
virtual std::string AGE::Texture::GetTextureFilePath () const = 0
```




<hr>



### function GetTextureID 

```C++
virtual uint32_t AGE::Texture::GetTextureID () const = 0
```




<hr>



### function GetWidth 

```C++
virtual uint32_t AGE::Texture::GetWidth () const = 0
```




<hr>



### function SetAssetID 

```C++
virtual void AGE::Texture::SetAssetID (
    uint64_t ID
) = 0
```




<hr>



### function SetData 

```C++
virtual void AGE::Texture::SetData (
    void * Data,
    uint32_t Size
) = 0
```




<hr>



### function SetName 

```C++
virtual void AGE::Texture::SetName (
    const std::string & Name
) = 0
```




<hr>



### function SetTextureFilePath 

```C++
virtual void AGE::Texture::SetTextureFilePath (
    const std::string & Path
) = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::Texture::Unbind () const = 0
```




<hr>



### function operator== 

```C++
virtual bool AGE::Texture::operator== (
    const Texture & Other
) const = 0
```




<hr>



### function ~Texture 

_Virtual destructor for the_ [_**Texture**_](class_a_g_e_1_1_texture.md) _class._
```C++
inline virtual AGE::Texture::~Texture () 
```



This function is responsible for releasing any resources that were acquired by the [**Texture**](class_a_g_e_1_1_texture.md) object, such as memory or file handles. It does not return anything and thus has an empty return type (void).


Virtual destructor for the [**Texture**](class_a_g_e_1_1_texture.md) class.


This function is a virtual destructor that cleans up any resources used by an instance of the [**Texture**](class_a_g_e_1_1_texture.md) class. It does not take any parameters and returns nothing. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Texture/Public/Texture.h`

