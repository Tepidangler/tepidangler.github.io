

# Class AGE::VertexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md)










Inherited by the following classes: [AGE::OpenGLVertexBuffer](class_a_g_e_1_1_open_g_l_vertex_buffer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-12) (float \* Verticies, uint32\_t Size) = 0<br> |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-22) (const void \* Verticies, uint32\_t Size) = 0<br> |
|  T \* | [**As**](#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
| virtual void | [**Bind**](#function-bind) () const = 0<br> |
| virtual [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CreateCircle**](#function-createcircle) ([**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, float Thickness, float Fade, int EntID) = 0<br> |
| virtual [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**CreateLine**](#function-createline) ([**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position0, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position1, int EntID=-1) = 0<br> |
| virtual [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**CreateQuad**](#function-createquad) ([**Vertex**](struct_a_g_e_1_1_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) = 0<br> |
| virtual [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**CreateText**](#function-createtext) ([**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TexID, int EntID) = 0<br> |
| virtual [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* | [**CreateTile**](#function-createtile) ([**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) = 0<br> |
| virtual const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & | [**GetLayout**](#function-getlayout) () const = 0<br> |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**SetLayout**](#function-setlayout) (const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & Layout) = 0<br> |
| virtual void | [**Unbind**](#function-unbind) () const = 0<br> |
| virtual  | [**~VertexBuffer**](#function-vertexbuffer) () <br>_Virtual destructor for the_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](#function-create-13) ([**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) \* Vertices, uint32\_t Size) <br> |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](#function-create-23) (uint32\_t Size) <br>_Creates a new_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _of the specified size. The type and usage of the buffer are determined by the current Rendering API in use._ |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](#function-create-33) (float \* Vertices=nullptr, uint32\_t Size=0) <br>_Creates a new vertex buffer object._  |


























## Public Functions Documentation




### function AddDataToBuffer [1/2]

```C++
virtual void AGE::VertexBuffer::AddDataToBuffer (
    float * Verticies,
    uint32_t Size
) = 0
```




<hr>



### function AddDataToBuffer [2/2]

```C++
virtual void AGE::VertexBuffer::AddDataToBuffer (
    const void * Verticies,
    uint32_t Size
) = 0
```




<hr>



### function As 

_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._ 
```C++
template<typename T>
T * AGE::VertexBuffer::As () 
```





**Returns:**

Returns a null pointer of type T\*


This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown.




**Returns:**

A pointer to an object of type T\* which is currently always null. 





        

<hr>



### function Bind 

```C++
virtual void AGE::VertexBuffer::Bind () const = 0
```




<hr>



### function CreateCircle 

```C++
virtual CircleVertex * AGE::VertexBuffer::CreateCircle (
    CircleVertex * Target,
    Matrix4D Transform,
    Vector4 * Position,
    Vector4 Color,
    float Thickness,
    float Fade,
    int EntID
) = 0
```




<hr>



### function CreateLine 

```C++
virtual LineVertex * AGE::VertexBuffer::CreateLine (
    LineVertex * Target,
    Vector4 Color,
    Vector3 Position0,
    Vector3 Position1,
    int EntID=-1
) = 0
```




<hr>



### function CreateQuad 

```C++
virtual Vertex * AGE::VertexBuffer::CreateQuad (
    Vertex * Target,
    Vector4 Color,
    Vector4 * Position,
    Vector2 Size,
    Matrix4D Transform,
    const Vector2 * TexCoords,
    float TilingFactor,
    float ID,
    int EnttID
) = 0
```




<hr>



### function CreateText 

```C++
virtual TextVertex * AGE::VertexBuffer::CreateText (
    TextVertex * Target,
    Matrix4D Transform,
    Vector4 * Position,
    Vector4 Color,
    Vector2 * TexCoords,
    float TexID,
    int EntID
) = 0
```




<hr>



### function CreateTile 

```C++
virtual TileVertex * AGE::VertexBuffer::CreateTile (
    TileVertex * Target,
    Vector4 Color,
    Vector4 * Position,
    Vector2 Size,
    Matrix4D Transform,
    const Vector2 * TexCoords,
    float TilingFactor,
    float ID,
    int EnttID
) = 0
```




<hr>



### function GetLayout 

```C++
virtual const BufferLayout & AGE::VertexBuffer::GetLayout () const = 0
```




<hr>



### function InvalidateBuffer 

```C++
virtual void AGE::VertexBuffer::InvalidateBuffer () const = 0
```




<hr>



### function SetLayout 

```C++
virtual void AGE::VertexBuffer::SetLayout (
    const BufferLayout & Layout
) = 0
```




<hr>



### function Unbind 

```C++
virtual void AGE::VertexBuffer::Unbind () const = 0
```




<hr>



### function ~VertexBuffer 

_Virtual destructor for the_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _class._
```C++
inline virtual AGE::VertexBuffer::~VertexBuffer () 
```



This function is responsible for releasing any resources that were acquired by the [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) object, such as memory or GPU resources. It does not return anything and thus has an empty return type (void). 


        

<hr>
## Public Static Functions Documentation




### function Create [1/3]

```C++
static Ref< VertexBuffer > AGE::VertexBuffer::Create (
    Matrix3D * Vertices,
    uint32_t Size
) 
```




<hr>



### function Create [2/3]

_Creates a new_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _of the specified size. The type and usage of the buffer are determined by the current Rendering API in use._
```C++
static Ref< VertexBuffer > AGE::VertexBuffer::Create (
    uint32_t Size
) 
```





**Parameters:**


* `Size` The size of the vertex buffer to create, in bytes. 



**Returns:**

A reference to the newly created [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md).


Creates a new [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) of the specified size. The type and usage of the buffer are determined by the current Rendering API in use.




**Parameters:**


* `Size` The size of the vertex buffer to create, in bytes. 



**Returns:**

A reference to the newly created [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md). If the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is not supported or an unknown error occurs, a nullptr will be returned instead. 





        

<hr>



### function Create [3/3]

_Creates a new vertex buffer object._ 
```C++
static Ref< VertexBuffer > AGE::VertexBuffer::Create (
    float * Vertices=nullptr,
    uint32_t Size=0
) 
```



This function creates and initializes a new [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) object based on the current rendering API in use. The data for the vertices is passed as an array of floats, with the size of this array also provided. If an unsupported rendering API is currently in use, nullptr is returned. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/RenderBuffer.h`

