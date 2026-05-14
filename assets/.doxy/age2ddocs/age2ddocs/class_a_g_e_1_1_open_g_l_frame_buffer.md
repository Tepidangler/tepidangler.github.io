

# Class AGE::OpenGLFrameBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md)








Inherits the following classes: [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override<br>_This function binds the OpenGL framebuffer to be used for rendering operations._  |
| virtual void | [**ClearAttachment**](#function-clearattachment) (uint32\_t Index, int Value) override<br>_Clears a specific color attachment at the given index with a specified value._  |
| virtual uint32\_t | [**GetColorAttachmentRendererID**](#function-getcolorattachmentrendererid) (uint32\_t Index=0) override const<br>_Get the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _ID for a specific Color Attachment._ |
| virtual uint32\_t | [**GetDepthAttachmentRendererID**](#function-getdepthattachmentrendererid) () override const<br>_This function returns the ID of the depth attachment renderer._  |
| virtual [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-12) () override<br>_Gets the specification of the frame buffer._  |
| virtual const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-22) () override const<br>_Returns the specification of the frame buffer._  |
| virtual const [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetWidthHeight**](#function-getwidthheight) () override const<br>_Returns the width and height of an object as a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _._ |
|  void | [**Invalidate**](#function-invalidate) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) override<br>_Handles events for the_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class._ |
|   | [**OpenGLFrameBuffer**](#function-openglframebuffer) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br>_Constructor for_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class._ |
| virtual void | [**Present**](#function-present) () override<br>_This function is used for presenting some content or data._  |
| virtual int | [**ReadPixel**](#function-readpixel) (uint32\_t AttachmentIndex, int x, int y) override<br>_Reads a single pixel from the OpenGL framebuffer._  |
| virtual void | [**Resize**](#function-resize) (const uint32\_t Width, const uint32\_t Height) override<br>_Resizes the OpenGL_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _to a new size._ |
| virtual void | [**Unbind**](#function-unbind) () override<br>_Unbinds the current frame buffer._  |
|   | [**~OpenGLFrameBuffer**](#function-openglframebuffer) () <br>_Destructor for the_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class. This function deletes both color and depth attachments associated with the frame buffer object._ |


## Public Functions inherited from AGE::FrameBuffer

See [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_frame_buffer.md#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
| virtual void | [**Bind**](class_a_g_e_1_1_frame_buffer.md#function-bind) () = 0<br> |
| virtual void | [**ClearAttachment**](class_a_g_e_1_1_frame_buffer.md#function-clearattachment) (uint32\_t Index, int Value) = 0<br> |
| virtual uint32\_t | [**GetColorAttachmentRendererID**](class_a_g_e_1_1_frame_buffer.md#function-getcolorattachmentrendererid) (uint32\_t Index=0) const = 0<br> |
| virtual uint32\_t | [**GetDepthAttachmentRendererID**](class_a_g_e_1_1_frame_buffer.md#function-getdepthattachmentrendererid) () const = 0<br> |
| virtual [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](class_a_g_e_1_1_frame_buffer.md#function-getspecification-12) () = 0<br> |
| virtual const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](class_a_g_e_1_1_frame_buffer.md#function-getspecification-22) () const = 0<br> |
| virtual const [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetWidthHeight**](class_a_g_e_1_1_frame_buffer.md#function-getwidthheight) () const = 0<br> |
| virtual void | [**OnEvent**](class_a_g_e_1_1_frame_buffer.md#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) = 0<br> |
| virtual void | [**Present**](class_a_g_e_1_1_frame_buffer.md#function-present) () = 0<br> |
| virtual int | [**ReadPixel**](class_a_g_e_1_1_frame_buffer.md#function-readpixel) (uint32\_t AttachmentIndex, int x, int y) = 0<br> |
| virtual void | [**Resize**](class_a_g_e_1_1_frame_buffer.md#function-resize) (const uint32\_t Width, const uint32\_t Height) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_frame_buffer.md#function-unbind) () = 0<br> |
| virtual  | [**~FrameBuffer**](class_a_g_e_1_1_frame_buffer.md#function-framebuffer) () <br>_Virtual destructor for the_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _class._ |




## Public Static Functions inherited from AGE::FrameBuffer

See [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_frame_buffer.md#function-create) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br>_Creates a new_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _based on the specified specification. The type of_[_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _to create is determined by the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _in use._ |


















































## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::OpenGLFrameBuffer::__pad0__;
```




<hr>
## Public Functions Documentation




### function Bind 

_This function binds the OpenGL framebuffer to be used for rendering operations._ 
```C++
virtual void AGE::OpenGLFrameBuffer::Bind () override
```



The function first calls glBindFramebuffer with GL\_FRAMEBUFFER and m\_RendererID as arguments, which binds the framebuffer object with the given ID. Then it sets the viewport using glViewport with (0, 0) and (m\_Specification.Width, m\_Specification.Height) as arguments, setting the dimensions of the rendering area to match the size of the framebuffer's client area.


Binds the OpenGL framebuffer object for rendering.


This function binds the framebuffer object associated with this instance of `OpenGLFrameBuffer` to the GL\_FRAMEBUFFER target, and sets the viewport dimensions according to the specification provided when the framebuffer was created.




**Returns:**

void 





        
Implements [*AGE::FrameBuffer::Bind*](class_a_g_e_1_1_frame_buffer.md#function-bind)


<hr>



### function ClearAttachment 

_Clears a specific color attachment at the given index with a specified value._ 
```C++
virtual void AGE::OpenGLFrameBuffer::ClearAttachment (
    uint32_t Index,
    int Value
) override
```



This function clears the color attachment at the provided index to the specified value using OpenGL's glClearTexImage function. It first checks if the provided index is within the valid range of color attachments, and then retrieves the corresponding specification for that attachment. The texture format from the specification is used in the call to glClearTexImage. If the index is out of bounds or there are no color attachments at all, it will assert with an error message.




**Parameters:**


* `Index` The zero-based index of the color attachment to clear. 
* `Value` The value to which to clear the specified color attachment.

Clears a specific color attachment at the given index with a specified value.


This function clears a color attachment at the provided index to a specified value using OpenGL's glClearTexImage function. The function first checks if the provided index is within the valid range of color attachments, and throws an assertion error if it isn't. Then, it retrieves the specification for the corresponding color attachment and uses this information to clear the texture with the specified value.




**Parameters:**


* `Index` The index of the color attachment to be cleared. 
* `Value` The value to which the color attachment should be cleared. 




        
Implements [*AGE::FrameBuffer::ClearAttachment*](class_a_g_e_1_1_frame_buffer.md#function-clearattachment)


<hr>



### function GetColorAttachmentRendererID 

_Get the_ [_**Renderer**_](class_a_g_e_1_1_renderer.md) _ID for a specific Color Attachment._
```C++
inline virtual uint32_t AGE::OpenGLFrameBuffer::GetColorAttachmentRendererID (
    uint32_t Index=0
) override const
```





**Parameters:**


* `Index` The index of the color attachment to get the renderer ID from. Default is 0. 



**Returns:**

The [**Renderer**](class_a_g_e_1_1_renderer.md) ID of the specified color attachment, or 0 if the index is out of range.


Get the ID of a color attachment at a given index.


This function retrieves the ID of a color attachment at a specified index in the framebuffer object. The default index is 0, which corresponds to the first color attachment. If an invalid index is provided (i.e., it's greater than or equal to the number of available color attachments), the program will assert and terminate.




**Parameters:**


* `Index` The zero-based index of the color attachment to retrieve. Default is 0. 



**Returns:**

The ID of the color attachment at the specified index. 





        
Implements [*AGE::FrameBuffer::GetColorAttachmentRendererID*](class_a_g_e_1_1_frame_buffer.md#function-getcolorattachmentrendererid)


<hr>



### function GetDepthAttachmentRendererID 

_This function returns the ID of the depth attachment renderer._ 
```C++
inline virtual uint32_t AGE::OpenGLFrameBuffer::GetDepthAttachmentRendererID () override const
```





**Returns:**

The ID of the depth attachment renderer as a uint32\_t value.


Returns the ID of the depth attachment renderer.


This function returns the unique identifier for the depth attachment renderer, which is used to reference and manipulate it in various rendering operations.




**Returns:**

The ID of the depth attachment renderer as a uint32\_t value. 





        
Implements [*AGE::FrameBuffer::GetDepthAttachmentRendererID*](class_a_g_e_1_1_frame_buffer.md#function-getdepthattachmentrendererid)


<hr>



### function GetSpecification [1/2]

_Gets the specification of the frame buffer._ 
```C++
inline virtual FrameBufferSpecification & AGE::OpenGLFrameBuffer::GetSpecification () override
```



This function returns a reference to the current specification of the frame buffer. The caller can use this information to determine how the frame buffer is configured and what it supports.




**Returns:**

A reference to the current [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object representing the specification of the frame buffer.


Gets the specification of the frame buffer.


This function returns a reference to the current specification of the frame buffer. The caller can modify this specification as needed, and these changes will be reflected in any views that are using the frame buffer.




**Returns:**

A reference to the current [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object. 





        
Implements [*AGE::FrameBuffer::GetSpecification*](class_a_g_e_1_1_frame_buffer.md#function-getspecification-12)


<hr>



### function GetSpecification [2/2]

_Returns the specification of the frame buffer._ 
```C++
inline virtual const FrameBufferSpecification & AGE::OpenGLFrameBuffer::GetSpecification () override const
```



This function returns a reference to the specification object that holds details about the current state of the frame buffer. The returned value is constant and should not be modified by the caller.




**Returns:**

A const reference to the [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object representing the current state of the frame buffer.


Returns the specification of the frame buffer.


This function returns a constant reference to the specification object that holds details about the current state of the frame buffer. The returned value is immutable and can be used for reading, but not for modification.




**Returns:**

A const reference to the [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object representing the current state of the frame buffer. 





        
Implements [*AGE::FrameBuffer::GetSpecification*](class_a_g_e_1_1_frame_buffer.md#function-getspecification-22)


<hr>



### function GetWidthHeight 

_Returns the width and height of an object as a_ [_**Vector2**_](struct_a_g_e_1_1_vector2.md) _._
```C++
inline virtual const Vector2 AGE::OpenGLFrameBuffer::GetWidthHeight () override const
```



This function retrieves the width and height from the m\_Specification member variable and returns them in a [**Vector2**](struct_a_g_e_1_1_vector2.md) format. The width is cast to float before being returned.




**Returns:**

A [**Vector2**](struct_a_g_e_1_1_vector2.md) containing the width and height of the object. 





        
Implements [*AGE::FrameBuffer::GetWidthHeight*](class_a_g_e_1_1_frame_buffer.md#function-getwidthheight)


<hr>



### function Invalidate 

```C++
void AGE::OpenGLFrameBuffer::Invalidate () 
```




<hr>



### function OnEvent 

_Handles events for the_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class._
```C++
virtual void AGE::OpenGLFrameBuffer::OnEvent (
    Event & E
) override
```



This function takes an event as input and processes it based on its type. The exact behavior of this function depends on the specifics of the [**Event**](class_a_g_e_1_1_event.md) class, which is not defined in this file.




**Parameters:**


* `E` Reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs processing.

Handles events for the [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md) class.


This function takes an [**Event**](class_a_g_e_1_1_event.md) object as input and handles it according to its type. The exact behavior of this function depends on the specific implementation of the [**Event**](class_a_g_e_1_1_event.md) class, which is not specified here.




**Parameters:**


* `E` An instance of the [**Event**](class_a_g_e_1_1_event.md) class that needs to be handled. 




        
Implements [*AGE::FrameBuffer::OnEvent*](class_a_g_e_1_1_frame_buffer.md#function-onevent)


<hr>



### function OpenGLFrameBuffer 

_Constructor for_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class._
```C++
AGE::OpenGLFrameBuffer::OpenGLFrameBuffer (
    const FrameBufferSpecification & Spec
) 
```



This constructor takes a [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object as input, which contains the specifications of the frame buffer to be created. It iterates over the Attachments in the specification and separates them into color attachments (those that are not depth formats) and depth attachment (the one that is). Finally, it calls Invalidate() function to create the actual frame buffer object with OpenGL.




**Parameters:**


* `Spec` The [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object containing specifications for the frame buffer.

Constructor for [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md) class.


This constructor initializes an instance of the [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md) class with a [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object. It processes the attachments in the specification and separates them into color and depth attachments, based on their format. The Invalidate() function is then called to generate the frame buffer object (FBO) and its associated textures.




**Parameters:**


* `Spec` A const reference to a [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) object containing information about the attachments for this frame buffer. 




        

<hr>



### function Present 

_This function is used for presenting some content or data._ 
```C++
inline virtual void AGE::OpenGLFrameBuffer::Present () override
```





**Returns:**

Nothing is returned as this function is a pure virtual function in the base class. It does not return any value.


This function is used for presenting something in the system.




**Returns:**

Nothing is returned as this function is a pure virtual one and does not provide any meaningful return value. 





        
Implements [*AGE::FrameBuffer::Present*](class_a_g_e_1_1_frame_buffer.md#function-present)


<hr>



### function ReadPixel 

_Reads a single pixel from the OpenGL framebuffer._ 
```C++
virtual int AGE::OpenGLFrameBuffer::ReadPixel (
    uint32_t AttachmentIndex,
    int x,
    int y
) override
```



This function reads a single pixel at the specified (x, y) coordinates in the color attachment of the framebuffer. The pixel data is returned as an integer value.




**Parameters:**


* `AttachmentIndex` Index of the color attachment to read from. It should be less than the number of elements in m\_ColorAttachments array. 
* `x` X-coordinate of the pixel to read. 
* `y` Y-coordinate of the pixel to read.



**Returns:**

The integer value of the pixel at (x, y) coordinates in the specified color attachment.


Reads a single pixel from the OpenGL framebuffer.


This function reads a single pixel at the specified (x, y) coordinates in the color attachment of the OpenGL framebuffer. The pixel data is returned as an integer value.




**Parameters:**


* `AttachmentIndex` Index of the color attachment to read from. Must be less than the number of elements in m\_ColorAttachments array. 
* `x` Horizontal position of the pixel to read, starting at 0 for leftmost column. 
* `y` Vertical position of the pixel to read, starting at 0 for top row.



**Returns:**

The integer value of the pixel data at (x, y). 





        
Implements [*AGE::FrameBuffer::ReadPixel*](class_a_g_e_1_1_frame_buffer.md#function-readpixel)


<hr>



### function Resize 

_Resizes the OpenGL_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _to a new size._
```C++
virtual void AGE::OpenGLFrameBuffer::Resize (
    const uint32_t Width,
    const uint32_t Height
) override
```



This function resizes the framebuffer to the specified width and height, provided they are within the maximum allowed size (s\_MaxFramebufferSize). If the dimensions are invalid or exceed the maximum size, it logs a warning message and returns without changing anything.




**Parameters:**


* `Width` The new width for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md). 
* `Height` The new height for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md).

Resizes the OpenGL [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) to a specified width and height.


The function checks if the provided dimensions are within the maximum framebuffer size limit (s\_MaxFramebufferSize). If they are, it updates the m\_Specification object with the new dimensions and calls Invalidate() to regenerate the framebuffer. If the dimensions are not valid, a warning is logged and no action is taken.




**Parameters:**


* `Width` The desired width for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md). Must be greater than zero and less or equal to s\_MaxFramebufferSize. 
* `Height` The desired height for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md). Must be greater than zero and less or equal to s&lt;｜begin▁of▁sentence｜&gt;MaxFramebufferSize. 




        
Implements [*AGE::FrameBuffer::Resize*](class_a_g_e_1_1_frame_buffer.md#function-resize)


<hr>



### function Unbind 

_Unbinds the current frame buffer._ 
```C++
virtual void AGE::OpenGLFrameBuffer::Unbind () override
```



This function binds the default frame buffer to the OpenGL context using glBindFramebuffer(). The GL\_FRAMEBUFFER target is used, and 0 is passed as argument to unbind the currently bound frame buffer.




**Returns:**

void


Unbinds the current frame buffer.


This function binds the default frame buffer to the OpenGL context using glBindFramebuffer(). The GL\_FRAMEBUFFER target is used, and 0 is passed as argument to unbind the currently bound frame buffer.




**Returns:**

void 





        
Implements [*AGE::FrameBuffer::Unbind*](class_a_g_e_1_1_frame_buffer.md#function-unbind)


<hr>



### function ~OpenGLFrameBuffer 

_Destructor for the_ [_**OpenGLFrameBuffer**_](class_a_g_e_1_1_open_g_l_frame_buffer.md) _class. This function deletes both color and depth attachments associated with the frame buffer object._
```C++
AGE::OpenGLFrameBuffer::~OpenGLFrameBuffer () 
```



Destructor for the [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md) class. This function deletes the framebuffer and its associated color and depth attachments from GPU memory. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLFrameBuffer.h`

