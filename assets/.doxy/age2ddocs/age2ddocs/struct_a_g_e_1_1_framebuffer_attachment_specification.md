

# Struct AGE::FramebufferAttachmentSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FramebufferAttachmentSpecification**](struct_a_g_e_1_1_framebuffer_attachment_specification.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; [**FramebufferTextureSpecification**](struct_a_g_e_1_1_framebuffer_texture_specification.md) &gt; | [**Attachments**](#variable-attachments)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FramebufferAttachmentSpecification**](#function-framebufferattachmentspecification-12) () = default<br>_Default constructor for the_ [_**FramebufferAttachmentSpecification**_](struct_a_g_e_1_1_framebuffer_attachment_specification.md) _class._ |
|   | [**FramebufferAttachmentSpecification**](#function-framebufferattachmentspecification-22) (std::initializer\_list&lt; [**FramebufferTextureSpecification**](struct_a_g_e_1_1_framebuffer_texture_specification.md) &gt; attachments) <br>_Constructs a_ [_**FramebufferAttachmentSpecification**_](struct_a_g_e_1_1_framebuffer_attachment_specification.md) _object with the given list of FramebufferTextureSpecifications._ |




























## Public Attributes Documentation




### variable Attachments 

```C++
std::vector<FramebufferTextureSpecification> AGE::FramebufferAttachmentSpecification::Attachments;
```




<hr>
## Public Functions Documentation




### function FramebufferAttachmentSpecification [1/2]

_Default constructor for the_ [_**FramebufferAttachmentSpecification**_](struct_a_g_e_1_1_framebuffer_attachment_specification.md) _class._
```C++
AGE::FramebufferAttachmentSpecification::FramebufferAttachmentSpecification () = default
```



This function initializes a new instance of the [**FramebufferAttachmentSpecification**](struct_a_g_e_1_1_framebuffer_attachment_specification.md) class with default values.


Default constructor for the [**FramebufferAttachmentSpecification**](struct_a_g_e_1_1_framebuffer_attachment_specification.md) class. 


        

<hr>



### function FramebufferAttachmentSpecification [2/2]

_Constructs a_ [_**FramebufferAttachmentSpecification**_](struct_a_g_e_1_1_framebuffer_attachment_specification.md) _object with the given list of FramebufferTextureSpecifications._
```C++
inline AGE::FramebufferAttachmentSpecification::FramebufferAttachmentSpecification (
    std::initializer_list< FramebufferTextureSpecification > attachments
) 
```





**Parameters:**


* `attachments` A std::initializer\_list&lt;FramebufferTextureSpecification&gt; containing the specifications for each texture to be attached to the framebuffer.

Constructs a [**FramebufferAttachmentSpecification**](struct_a_g_e_1_1_framebuffer_attachment_specification.md) object with the given list of FramebufferTextureSpecifications.




**Parameters:**


* `attachments` A std::initializer\_list&lt;FramebufferTextureSpecification&gt; containing the specifications for each texture attachment to be used in the framebuffer. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/FrameBuffer.h`

