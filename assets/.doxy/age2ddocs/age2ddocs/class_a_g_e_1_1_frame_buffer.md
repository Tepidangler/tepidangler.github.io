

# Class AGE::FrameBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md)










Inherited by the following classes: [AGE::OpenGLFrameBuffer](class_a_g_e_1_1_open_g_l_frame_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
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
| virtual  | [**~FrameBuffer**](#function-framebuffer) () <br>_Virtual destructor for the_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) &gt; | [**Create**](#function-create) (const [**FrameBufferSpecification**](struct_a_g_e_1_1_frame_buffer_specification.md) & Spec) <br>_Creates a new_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _based on the specified specification. The type of_[_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _to create is determined by the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _in use._ |


























## Public Functions Documentation




### function As 

_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._ 
```C++
template<typename T>
T * AGE::FrameBuffer::As () 
```





**Returns:**

A null pointer of type T\*


This function is currently not implemented and will always throw an assertion error. It returns a null pointer of type T\*. The purpose of this function is unknown.




**Returns:**

A null pointer of type T\* 





        

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

_Virtual destructor for the_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _class._
```C++
inline virtual AGE::FrameBuffer::~FrameBuffer () 
```



This function is responsible for releasing any resources that were acquired by the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) object, such as memory or file handles. It does not return anything (void) and thus it doesn't need a Doxygen comment to document its return value.


Virtual destructor for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return anything and thus has an empty return type (void). 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new_ [_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _based on the specified specification. The type of_[_**FrameBuffer**_](class_a_g_e_1_1_frame_buffer.md) _to create is determined by the current_[_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _in use._
```C++
static Ref< FrameBuffer > AGE::FrameBuffer::Create (
    const FrameBufferSpecification & Spec
) 
```





**Parameters:**


* `Spec` The specification for the [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) to be created. This includes things like width, height and color attachments. 



**Returns:**

A reference to the newly created [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md). If the [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use does not support a [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) of that type, nullptr is returned instead.


Creates a new frame buffer based on the given specification. The type of [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) to create is determined by the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) in use.




**Parameters:**


* `Spec` The specification for the new frame buffer. This includes things like width, height and color attachments. 



**Returns:**

A reference to the newly created [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md). If no suitable [**FrameBuffer**](class_a_g_e_1_1_frame_buffer.md) could be created (e.g., due to unsupported [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md)), nullptr is returned instead. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/FrameBuffer.h`

