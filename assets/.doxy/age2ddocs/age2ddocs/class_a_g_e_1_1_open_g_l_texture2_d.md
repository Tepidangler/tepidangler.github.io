

# Class AGE::OpenGLTexture2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md)








Inherits the following classes: [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)










































































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) (uint32\_t Slot=0) override const<br>_This function binds the texture to a specific slot in the OpenGL context._  |
| virtual uint64\_t | [**GetAssetID**](#function-getassetid) () override const<br>_This function returns the Asset ID of an object._  |
| virtual uint32\_t | [**GetHeight**](#function-getheight) () override const<br>_This function returns the height of an object._  |
| virtual std::string | [**GetName**](#function-getname) () override const<br>_Returns the name of the object._  |
| virtual uint32\_t | [**GetNrChannels**](#function-getnrchannels) () const<br>_Returns the number of channels in the system._  |
| virtual const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & | [**GetSpecification**](#function-getspecification) () override const<br>_Returns the texture specification of this object._  |
| virtual std::pair&lt; uint8\_t \*, size\_t &gt; | [**GetTextureData**](#function-gettexturedata) () override<br>_This function returns the texture data along with its size._  |
| virtual std::string | [**GetTextureFilePath**](#function-gettexturefilepath) () override const<br>_Returns the file path of the texture._  |
| virtual uint32\_t | [**GetTextureID**](#function-gettextureid) () override const<br>_Returns the texture ID of this object._  |
| virtual uint32\_t | [**GetWidth**](#function-getwidth) () override const<br>_This function returns the width of an object as a uint32\_t value._  |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-15) (const std::string & Path) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-25) (const tmx\_image \* Image) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-35) (const std::vector&lt; std::string &gt; & Paths) <br> |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br>_Constructs an OpenGL 2D texture with the given specification._  |
|   | [**OpenGLTexture2D**](#function-opengltexture2d-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br> |
| virtual void | [**SetAssetID**](#function-setassetid) (uint64\_t ID) override<br>_Sets the Asset ID of an object._  |
| virtual void | [**SetData**](#function-setdata) (void \* Data, uint32\_t Size) override<br> |
| virtual void | [**SetName**](#function-setname) (const std::string & Name) override<br>_Sets the name of the object._  |
| virtual void | [**SetTextureFilePath**](#function-settexturefilepath) (const std::string & Path) override<br>_Sets the texture file path for rendering._  |
| virtual void | [**Unbind**](#function-unbind) () override const<br>_Unbinds the texture from the specified texture unit._  |
| virtual bool | [**operator==**](#function-operator) (const [**Texture**](class_a_g_e_1_1_texture.md) & Other) override const<br>_Compares this_ [_**OpenGLTexture2D**_](class_a_g_e_1_1_open_g_l_texture2_d.md) _object with another for equality._ |
|   | [**~OpenGLTexture2D**](#function-opengltexture2d) () <br>_Destructor for_ [_**OpenGLTexture2D**_](class_a_g_e_1_1_open_g_l_texture2_d.md) _class. Deletes the texture from GPU memory._ |


## Public Functions inherited from AGE::Texture2D

See [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_texture2_d.md#function-as) () <br>_This function is currently not implemented. It will return a pointer to an object of type T. If called, it will assert and crash the program with the message "As() Failed!"._  |


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




## Public Static Functions inherited from AGE::Texture2D

See [AGE::Texture2D](class_a_g_e_1_1_texture2_d.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-15) (const std::string & Path) <br>_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-25) (const tmx\_image \* Image) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the current Rendering API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-35) (const std::vector&lt; std::string &gt; & Path) <br>_Creates a reference to a_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of texture is determined by the current renderer API._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-45) (const [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) & Spec) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object based on the given specification. The type of texture to be created is determined by the current renderer API in use._ |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Create**](class_a_g_e_1_1_texture2_d.md#function-create-55) (const [**Image**](class_a_g_e_1_1_image.md) \* Img, uint32\_t Width, uint32\_t Height, int Channels, size\_t Size) <br>_Creates a new_ [_**Texture2D**_](class_a_g_e_1_1_texture2_d.md) _object. The type of the texture is determined by the current renderer API._ |












































































## Public Functions Documentation




### function Bind 

_This function binds the texture to a specific slot in the OpenGL context._ 
```C++
virtual void AGE::OpenGLTexture2D::Bind (
    uint32_t Slot=0
) override const
```





**Parameters:**


* `Slot` The index of the texture unit to which the texture should be bound.



**Returns:**

void 





        
Implements [*AGE::Texture::Bind*](class_a_g_e_1_1_texture.md#function-bind)


<hr>



### function GetAssetID 

_This function returns the Asset ID of an object._ 
```C++
inline virtual uint64_t AGE::OpenGLTexture2D::GetAssetID () override const
```





**Returns:**

The asset ID as a uint64\_t value.


This function returns the Asset ID of an object. 

**Returns:**

The uint64\_t value representing the Asset ID. 





        
Implements [*AGE::Texture::GetAssetID*](class_a_g_e_1_1_texture.md#function-getassetid)


<hr>



### function GetHeight 

_This function returns the height of an object._ 
```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetHeight () override const
```





**Returns:**

The height as a uint32\_t value.


Returns the height of an object as a uint32\_t value.


This function is used to get the current height of an object in the form of a uint32\_t value. It returns the private member variable m\_Height, which represents the height of the object.




**Returns:**

The height of the object as a uint32\_t value. 





        
Implements [*AGE::Texture::GetHeight*](class_a_g_e_1_1_texture.md#function-getheight)


<hr>



### function GetName 

_Returns the name of the object._ 
```C++
inline virtual std::string AGE::OpenGLTexture2D::GetName () override const
```





**Returns:**

The name of the object as a string.


Returns the name of the object.


This function returns a string that represents the name of the object. It is implemented as an overridden method in the base class, so it will be used when calling [**GetName()**](class_a_g_e_1_1_open_g_l_texture2_d.md#function-getname) on any derived classes.




**Returns:**

std::string The name of the object. 





        
Implements [*AGE::Texture::GetName*](class_a_g_e_1_1_texture.md#function-getname)


<hr>



### function GetNrChannels 

_Returns the number of channels in the system._ 
```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetNrChannels () const
```



This function returns the current number of channels that are active in the system. It does not take any parameters and always returns a uint32\_t value representing the number of channels.




**Returns:**

The number of channels as an unsigned 32-bit integer.


This function returns the number of channels in the system. 

**Returns:**

The number of channels as a uint32\_t value. 





        

<hr>



### function GetSpecification 

_Returns the texture specification of this object._ 
```C++
inline virtual const TextureSpecification & AGE::OpenGLTexture2D::GetSpecification () override const
```





**Returns:**

A constant reference to the texture specification (m\_Specification).


Returns the texture specification of this object.


This function returns a constant reference to the texture specification that is currently set for this object. The returned value cannot be modified by the caller.




**Returns:**

A const reference to the current [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md). 





        
Implements [*AGE::Texture::GetSpecification*](class_a_g_e_1_1_texture.md#function-getspecification)


<hr>



### function GetTextureData 

_This function returns the texture data along with its size._ 
```C++
inline virtual std::pair< uint8_t *, size_t > AGE::OpenGLTexture2D::GetTextureData () override
```





**Returns:**

A pair of uint8 pointer and size\_t, representing the texture data and its size respectively.


Retrieves the texture data along with its size.


This function returns a pair of uint8\_t pointer and size\_t value representing the texture data and its size respectively. The returned data is owned by the caller, and should not be freed or modified directly. If no texture data exists (e.g., after clearing the image), the pointer will be null and the size will be 0.




**Returns:**

A pair of uint8\_t\* and size\_t representing the texture data and its size respectively. 





        
Implements [*AGE::Texture::GetTextureData*](class_a_g_e_1_1_texture.md#function-gettexturedata)


<hr>



### function GetTextureFilePath 

_Returns the file path of the texture._ 
```C++
inline virtual std::string AGE::OpenGLTexture2D::GetTextureFilePath () override const
```





**Returns:**

The file path as a string. If no path is set, returns an empty string.


This function returns the path of a texture file. 

**Returns:**

std::string The path to the texture file. 





        
Implements [*AGE::Texture::GetTextureFilePath*](class_a_g_e_1_1_texture.md#function-gettexturefilepath)


<hr>



### function GetTextureID 

_Returns the texture ID of this object._ 
```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetTextureID () override const
```



This function returns the unique identifier for the texture associated with this object. The value is constant and does not change over time.




**Returns:**

A uint32\_t representing the texture ID.


Returns the texture ID of this object. 

**Returns:**

The texture ID as a uint32\_t value. 





        
Implements [*AGE::Texture::GetTextureID*](class_a_g_e_1_1_texture.md#function-gettextureid)


<hr>



### function GetWidth 

_This function returns the width of an object as a uint32\_t value._ 
```C++
inline virtual uint32_t AGE::OpenGLTexture2D::GetWidth () override const
```





**Returns:**

The width of the object represented by a uint32\_t.


Returns the width of the object. 

**Returns:**

The width as a uint32\_t value. 





        
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
    const tmx_image * Image
) 
```




<hr>



### function OpenGLTexture2D [3/5]

```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const std::vector< std::string > & Paths
) 
```



Constructor for [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md) class. Loads a 2D texture from the given file paths. The constructor iterates over each path in the input vector, loads an image using stbi\_load(), and creates an OpenGL texture with the loaded data. It also sets various parameters for the texture such as wrapping mode (GL\_REPEAT), minifying/magnifying filter (GL\_NEAREST). The constructor assumes that all images are in RGB or RGBA format, and it uses stbi\_image\_free() to free the loaded image data after creating the OpenGL texture.




**Parameters:**


* `Paths` A vector of strings representing the file paths to load the textures from. 




        

<hr>



### function OpenGLTexture2D [4/5]

_Constructs an OpenGL 2D texture with the given specification._ 
```C++
AGE::OpenGLTexture2D::OpenGLTexture2D (
    const TextureSpecification & Spec
) 
```



The function creates a new OpenGL texture object and initializes it with the provided [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md). It sets various parameters such as wrapping and filtering modes for the texture.




**Parameters:**


* `Spec` The [**TextureSpecification**](struct_a_g_e_1_1_texture_specification.md) that contains details about the format, width, height etc of the texture to be created. 




        

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

_Sets the Asset ID of an object._ 
```C++
inline virtual void AGE::OpenGLTexture2D::SetAssetID (
    uint64_t ID
) override
```





**Parameters:**


* `ID` The unique identifier for the asset. 



**Returns:**

void


Sets the Asset ID for an object. 

**Parameters:**


* `ID` The unique identifier of the asset. 




        
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

_Sets the name of the object._ 
```C++
inline virtual void AGE::OpenGLTexture2D::SetName (
    const std::string & Name
) override
```





**Parameters:**


* `Name` The new name to set for the object.

Sets the name of the object. 

**Parameters:**


* `Name` The new name to set for the object. 




        
Implements [*AGE::Texture::SetName*](class_a_g_e_1_1_texture.md#function-setname)


<hr>



### function SetTextureFilePath 

_Sets the texture file path for rendering._ 
```C++
inline virtual void AGE::OpenGLTexture2D::SetTextureFilePath (
    const std::string & Path
) override
```





**Parameters:**


* `Path` The new file path to be set as a string reference. 



**Returns:**

None, void function that directly modifies member variable 'm\_Path'.


Sets the texture file path.


This function sets the texture file path by taking a constant reference to a string as its argument. The string is then assigned to the member variable 'm\_Path'.




**Parameters:**


* `Path` A constant reference to the new texture file path. 




        
Implements [*AGE::Texture::SetTextureFilePath*](class_a_g_e_1_1_texture.md#function-settexturefilepath)


<hr>



### function Unbind 

_Unbinds the texture from the specified texture unit._ 
```C++
virtual void AGE::OpenGLTexture2D::Unbind () override const
```



This function binds a specific OpenGL texture to the first available texture unit (unit 0). After this operation, no further operations will affect this texture.




**Returns:**

void 





        
Implements [*AGE::Texture::Unbind*](class_a_g_e_1_1_texture.md#function-unbind)


<hr>



### function operator== 

_Compares this_ [_**OpenGLTexture2D**_](class_a_g_e_1_1_open_g_l_texture2_d.md) _object with another for equality._
```C++
inline virtual bool AGE::OpenGLTexture2D::operator== (
    const Texture & Other
) override const
```



This function compares the texture ID of this object with that of the provided [**Texture**](class_a_g_e_1_1_texture.md) object. It first casts the other object to an [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md), then checks if their texture IDs are equal.




**Parameters:**


* `Other` The [**Texture**](class_a_g_e_1_1_texture.md) object to compare against. 



**Returns:**

True if the texture IDs match; false otherwise.


Compares this [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md) with another for equality.


This function compares the texture ID of this [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md) instance with that of another [**Texture**](class_a_g_e_1_1_texture.md) instance. It first casts Other to an [**OpenGLTexture2D**](class_a_g_e_1_1_open_g_l_texture2_d.md) reference, then checks if their texture IDs are equal. The comparison is case-sensitive and does not take into account any potential differences in the other properties or states of these objects.




**Parameters:**


* `Other` - Another [**Texture**](class_a_g_e_1_1_texture.md) instance to compare with this one. 



**Returns:**

True if both instances have the same texture ID, false otherwise. 





        
Implements [*AGE::Texture::operator==*](class_a_g_e_1_1_texture.md#function-operator)


<hr>



### function ~OpenGLTexture2D 

_Destructor for_ [_**OpenGLTexture2D**_](class_a_g_e_1_1_open_g_l_texture2_d.md) _class. Deletes the texture from GPU memory._
```C++
AGE::OpenGLTexture2D::~OpenGLTexture2D () 
```



This function uses the glDeleteTextures() function to delete a single texture, identified by its ID (m\_TextureID). The texture is deleted from the GPU's memory and can no longer be used in rendering operations.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLTexture.h`

