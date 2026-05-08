

# Class AGE::OpenGLFrameBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLFrameBuffer**](class_a_g_e_1_1_open_g_l_frame_buffer.md)








Inherits the following classes: [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Bind**](#function-bind) () override<br> |
| virtual void | [**ClearAttachment**](#function-clearattachment) (uint32\_t Index, int Value) override<br> |
| virtual uint32\_t | [**GetColorAttachmentRendererID**](#function-getcolorattachmentrendererid) (uint32\_t Index=0) override const<br> |
| virtual uint32\_t | [**GetDepthAttachmentRendererID**](#function-getdepthattachmentrendererid) () override const<br> |
| virtual [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-12) () override<br> |
| virtual const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-22) () override const<br> |
| virtual const [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetWidthHeight**](#function-getwidthheight) () override const<br> |
|  void | [**Invalidate**](#function-invalidate) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) override<br> |
|   | [**OpenGLFrameBuffer**](#function-openglframebuffer) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br> |
| virtual void | [**Present**](#function-present) () override<br> |
| virtual int | [**ReadPixel**](#function-readpixel) (uint32\_t AttachmentIndex, int x, int y) override<br> |
| virtual void | [**Resize**](#function-resize) (const uint32\_t Width, const uint32\_t Height) override<br> |
| virtual void | [**Unbind**](#function-unbind) () override<br> |
|   | [**~OpenGLFrameBuffer**](#function-openglframebuffer) () <br> |


## Public Functions inherited from AGE::FrameBuffer

See [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_frame_buffer.md#function-as) () <br> |
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
| virtual  | [**~FrameBuffer**](class_a_g_e_1_1_frame_buffer.md#function-framebuffer) () <br> |




## Public Static Functions inherited from AGE::FrameBuffer

See [AGE::FrameBuffer](class_a_g_e_1_1_frame_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_frame_buffer.md#function-create) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br> |


















































## Public Functions Documentation




### function Bind 

```C++
virtual void AGE::OpenGLFrameBuffer::Bind () override
```



Implements [*AGE::FrameBuffer::Bind*](class_a_g_e_1_1_frame_buffer.md#function-bind)


<hr>



### function ClearAttachment 

```C++
virtual void AGE::OpenGLFrameBuffer::ClearAttachment (
    uint32_t Index,
    int Value
) override
```



Implements [*AGE::FrameBuffer::ClearAttachment*](class_a_g_e_1_1_frame_buffer.md#function-clearattachment)


<hr>



### function GetColorAttachmentRendererID 

```C++
inline virtual uint32_t AGE::OpenGLFrameBuffer::GetColorAttachmentRendererID (
    uint32_t Index=0
) override const
```



Implements [*AGE::FrameBuffer::GetColorAttachmentRendererID*](class_a_g_e_1_1_frame_buffer.md#function-getcolorattachmentrendererid)


<hr>



### function GetDepthAttachmentRendererID 

```C++
inline virtual uint32_t AGE::OpenGLFrameBuffer::GetDepthAttachmentRendererID () override const
```



Implements [*AGE::FrameBuffer::GetDepthAttachmentRendererID*](class_a_g_e_1_1_frame_buffer.md#function-getdepthattachmentrendererid)


<hr>



### function GetSpecification [1/2]

```C++
inline virtual FrameBufferSpecification & AGE::OpenGLFrameBuffer::GetSpecification () override
```



Implements [*AGE::FrameBuffer::GetSpecification*](class_a_g_e_1_1_frame_buffer.md#function-getspecification-12)


<hr>



### function GetSpecification [2/2]

```C++
inline virtual const FrameBufferSpecification & AGE::OpenGLFrameBuffer::GetSpecification () override const
```



Implements [*AGE::FrameBuffer::GetSpecification*](class_a_g_e_1_1_frame_buffer.md#function-getspecification-22)


<hr>



### function GetWidthHeight 

```C++
inline virtual const Vector2 AGE::OpenGLFrameBuffer::GetWidthHeight () override const
```



Implements [*AGE::FrameBuffer::GetWidthHeight*](class_a_g_e_1_1_frame_buffer.md#function-getwidthheight)


<hr>



### function Invalidate 

```C++
void AGE::OpenGLFrameBuffer::Invalidate () 
```




<hr>



### function OnEvent 

```C++
virtual void AGE::OpenGLFrameBuffer::OnEvent (
    Event & E
) override
```



Implements [*AGE::FrameBuffer::OnEvent*](class_a_g_e_1_1_frame_buffer.md#function-onevent)


<hr>



### function OpenGLFrameBuffer 

```C++
AGE::OpenGLFrameBuffer::OpenGLFrameBuffer (
    const FrameBufferSpecification & Spec
) 
```




<hr>



### function Present 

```C++
inline virtual void AGE::OpenGLFrameBuffer::Present () override
```



Implements [*AGE::FrameBuffer::Present*](class_a_g_e_1_1_frame_buffer.md#function-present)


<hr>



### function ReadPixel 

```C++
virtual int AGE::OpenGLFrameBuffer::ReadPixel (
    uint32_t AttachmentIndex,
    int x,
    int y
) override
```



Implements [*AGE::FrameBuffer::ReadPixel*](class_a_g_e_1_1_frame_buffer.md#function-readpixel)


<hr>



### function Resize 

```C++
virtual void AGE::OpenGLFrameBuffer::Resize (
    const uint32_t Width,
    const uint32_t Height
) override
```



Implements [*AGE::FrameBuffer::Resize*](class_a_g_e_1_1_frame_buffer.md#function-resize)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLFrameBuffer::Unbind () override
```



Implements [*AGE::FrameBuffer::Unbind*](class_a_g_e_1_1_frame_buffer.md#function-unbind)


<hr>



### function ~OpenGLFrameBuffer 

```C++
AGE::OpenGLFrameBuffer::~OpenGLFrameBuffer () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLFrameBuffer.h`

