

# Class AGE::FrameBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md)










Inherited by the following classes: [AGE::OpenGLFrameBuffer](class_a_g_e_1_1_open_g_l_frame_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br> |
| virtual void | [**Bind**](#function-bind) () = 0<br> |
| virtual void | [**ClearAttachment**](#function-clearattachment) (uint32\_t Index, int Value) = 0<br> |
| virtual uint32\_t | [**GetColorAttachmentRendererID**](#function-getcolorattachmentrendererid) (uint32\_t Index=0) const = 0<br> |
| virtual uint32\_t | [**GetDepthAttachmentRendererID**](#function-getdepthattachmentrendererid) () const = 0<br> |
| virtual [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-12) () = 0<br> |
| virtual const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & | [**GetSpecification**](#function-getspecification-22) () const = 0<br> |
| virtual const [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetWidthHeight**](#function-getwidthheight) () const = 0<br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) = 0<br> |
| virtual void | [**Present**](#function-present) () = 0<br> |
| virtual int | [**ReadPixel**](#function-readpixel) (uint32\_t AttachmentIndex, int x, int y) = 0<br> |
| virtual void | [**Resize**](#function-resize) (const uint32\_t Width, const uint32\_t Height) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () = 0<br> |
| virtual  | [**~FrameBuffer**](#function-framebuffer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) &gt; | [**Create**](#function-create) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br> |


























## Public Functions Documentation




### function As 

```C++
template<typename T>
T * AGE::FrameBuffer::As () 
```




<hr>



### function Bind 

```C++
virtual void AGE::FrameBuffer::Bind () = 0
```




<hr>



### function ClearAttachment 

```C++
virtual void AGE::FrameBuffer::ClearAttachment (
    uint32_t Index,
    int Value
) = 0
```




<hr>



### function GetColorAttachmentRendererID 

```C++
virtual uint32_t AGE::FrameBuffer::GetColorAttachmentRendererID (
    uint32_t Index=0
) const = 0
```




<hr>



### function GetDepthAttachmentRendererID 

```C++
virtual uint32_t AGE::FrameBuffer::GetDepthAttachmentRendererID () const = 0
```




<hr>



### function GetSpecification [1/2]

```C++
virtual FrameBufferSpecification & AGE::FrameBuffer::GetSpecification () = 0
```




<hr>



### function GetSpecification [2/2]

```C++
virtual const FrameBufferSpecification & AGE::FrameBuffer::GetSpecification () const = 0
```




<hr>



### function GetWidthHeight 

```C++
virtual const Vector2 AGE::FrameBuffer::GetWidthHeight () const = 0
```




<hr>



### function OnEvent 

```C++
virtual void AGE::FrameBuffer::OnEvent (
    Event & E
) = 0
```




<hr>



### function Present 

```C++
virtual void AGE::FrameBuffer::Present () = 0
```




<hr>



### function ReadPixel 

```C++
virtual int AGE::FrameBuffer::ReadPixel (
    uint32_t AttachmentIndex,
    int x,
    int y
) = 0
```




<hr>



### function Resize 

```C++
virtual void AGE::FrameBuffer::Resize (
    const uint32_t Width,
    const uint32_t Height
) = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::FrameBuffer::Unbind () = 0
```




<hr>



### function ~FrameBuffer 

```C++
inline virtual AGE::FrameBuffer::~FrameBuffer () 
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< FrameBuffer > AGE::FrameBuffer::Create (
    const FrameBufferSpecification & Spec
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/FrameBuffer.h`

