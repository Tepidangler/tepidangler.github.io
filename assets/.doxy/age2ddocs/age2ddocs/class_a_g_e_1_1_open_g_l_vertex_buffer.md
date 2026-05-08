

# Class AGE::OpenGLVertexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md)








Inherits the following classes: [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-12) (float \* Verticies, uint32\_t Size) override<br> |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-22) (const void \* Verticies, uint32\_t Size) override<br> |
| virtual void | [**Bind**](#function-bind) () override const<br> |
| virtual [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CreateCircle**](#function-createcircle) ([**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, float Thickness, float Fade, int EntID) override<br> |
| virtual [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**CreateLine**](#function-createline) ([**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position0, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position1, int EntID) override<br> |
| virtual [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**CreateQuad**](#function-createquad) ([**Vertex**](struct_a_g_e_1_1_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) override<br> |
| virtual [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**CreateText**](#function-createtext) ([**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TexID, int EntID) override<br> |
| virtual [**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* | [**CreateTile**](#function-createtile) ([**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* UV, uint32\_t TSID, int EnttID) override<br> |
| virtual const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & | [**GetLayout**](#function-getlayout) () override const<br> |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () override const<br> |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-13) (uint32\_t Size) <br> |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-23) ([**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) \* Vertices, uint32\_t Size) <br> |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-33) (float \* Vertices, uint32\_t Size) <br> |
| virtual void | [**SetLayout**](#function-setlayout) (const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & Layout) override<br> |
| virtual void | [**Unbind**](#function-unbind) () override const<br> |
| virtual  | [**~OpenGLVertexBuffer**](#function-openglvertexbuffer) () <br> |


## Public Functions inherited from AGE::VertexBuffer

See [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**AddDataToBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-12) (float \* Verticies, uint32\_t Size) = 0<br> |
| virtual void | [**AddDataToBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-22) (const void \* Verticies, uint32\_t Size) = 0<br> |
|  T \* | [**As**](class_a_g_e_1_1_vertex_buffer.md#function-as) () <br> |
| virtual void | [**Bind**](class_a_g_e_1_1_vertex_buffer.md#function-bind) () const = 0<br> |
| virtual [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CreateCircle**](class_a_g_e_1_1_vertex_buffer.md#function-createcircle) ([**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, float Thickness, float Fade, int EntID) = 0<br> |
| virtual [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**CreateLine**](class_a_g_e_1_1_vertex_buffer.md#function-createline) ([**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position0, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position1, int EntID=-1) = 0<br> |
| virtual [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**CreateQuad**](class_a_g_e_1_1_vertex_buffer.md#function-createquad) ([**Vertex**](struct_a_g_e_1_1_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) = 0<br> |
| virtual [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**CreateText**](class_a_g_e_1_1_vertex_buffer.md#function-createtext) ([**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TexID, int EntID) = 0<br> |
| virtual [**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* | [**CreateTile**](class_a_g_e_1_1_vertex_buffer.md#function-createtile) ([**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* UV, uint32\_t TSID, int EnttID) = 0<br> |
| virtual const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & | [**GetLayout**](class_a_g_e_1_1_vertex_buffer.md#function-getlayout) () const = 0<br> |
| virtual void | [**InvalidateBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**SetLayout**](class_a_g_e_1_1_vertex_buffer.md#function-setlayout) (const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & Layout) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_vertex_buffer.md#function-unbind) () const = 0<br> |
| virtual  | [**~VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-vertexbuffer) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetRendererID**](#function-getrendererid) () <br> |


## Public Static Functions inherited from AGE::VertexBuffer

See [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-13) ([**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) \* Vertices, uint32\_t Size) <br> |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-23) (uint32\_t Size) <br> |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-33) (float \* Vertices=nullptr, uint32\_t Size=0) <br> |


















































## Public Functions Documentation




### function AddDataToBuffer [1/2]

```C++
virtual void AGE::OpenGLVertexBuffer::AddDataToBuffer (
    float * Verticies,
    uint32_t Size
) override
```



Implements [*AGE::VertexBuffer::AddDataToBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-12)


<hr>



### function AddDataToBuffer [2/2]

```C++
virtual void AGE::OpenGLVertexBuffer::AddDataToBuffer (
    const void * Verticies,
    uint32_t Size
) override
```



Implements [*AGE::VertexBuffer::AddDataToBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-22)


<hr>



### function Bind 

```C++
virtual void AGE::OpenGLVertexBuffer::Bind () override const
```



Implements [*AGE::VertexBuffer::Bind*](class_a_g_e_1_1_vertex_buffer.md#function-bind)


<hr>



### function CreateCircle 

```C++
virtual CircleVertex * AGE::OpenGLVertexBuffer::CreateCircle (
    CircleVertex * Target,
    Matrix4D Transform,
    Vector4 * Position,
    Vector4 Color,
    float Thickness,
    float Fade,
    int EntID
) override
```



Implements [*AGE::VertexBuffer::CreateCircle*](class_a_g_e_1_1_vertex_buffer.md#function-createcircle)


<hr>



### function CreateLine 

```C++
virtual LineVertex * AGE::OpenGLVertexBuffer::CreateLine (
    LineVertex * Target,
    Vector4 Color,
    Vector3 Position0,
    Vector3 Position1,
    int EntID
) override
```



Implements [*AGE::VertexBuffer::CreateLine*](class_a_g_e_1_1_vertex_buffer.md#function-createline)


<hr>



### function CreateQuad 

```C++
virtual Vertex * AGE::OpenGLVertexBuffer::CreateQuad (
    Vertex * Target,
    Vector4 Color,
    Vector4 * Position,
    Vector2 Size,
    Matrix4D Transform,
    const Vector2 * TexCoords,
    float TilingFactor,
    float ID,
    int EnttID
) override
```



Implements [*AGE::VertexBuffer::CreateQuad*](class_a_g_e_1_1_vertex_buffer.md#function-createquad)


<hr>



### function CreateText 

```C++
virtual TextVertex * AGE::OpenGLVertexBuffer::CreateText (
    TextVertex * Target,
    Matrix4D Transform,
    Vector4 * Position,
    Vector4 Color,
    Vector2 * TexCoords,
    float TexID,
    int EntID
) override
```



Implements [*AGE::VertexBuffer::CreateText*](class_a_g_e_1_1_vertex_buffer.md#function-createtext)


<hr>



### function CreateTile 

```C++
virtual TilemapVertex * AGE::OpenGLVertexBuffer::CreateTile (
    TilemapVertex * Target,
    Vector4 Color,
    Vector4 * Position,
    Matrix4D Transform,
    const Vector2 * UV,
    uint32_t TSID,
    int EnttID
) override
```



Implements [*AGE::VertexBuffer::CreateTile*](class_a_g_e_1_1_vertex_buffer.md#function-createtile)


<hr>



### function GetLayout 

```C++
inline virtual const BufferLayout & AGE::OpenGLVertexBuffer::GetLayout () override const
```



Implements [*AGE::VertexBuffer::GetLayout*](class_a_g_e_1_1_vertex_buffer.md#function-getlayout)


<hr>



### function InvalidateBuffer 

```C++
virtual void AGE::OpenGLVertexBuffer::InvalidateBuffer () override const
```



Implements [*AGE::VertexBuffer::InvalidateBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-invalidatebuffer)


<hr>



### function OpenGLVertexBuffer [1/3]

```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    uint32_t Size
) 
```




<hr>



### function OpenGLVertexBuffer [2/3]

```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    Matrix3D * Vertices,
    uint32_t Size
) 
```




<hr>



### function OpenGLVertexBuffer [3/3]

```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    float * Vertices,
    uint32_t Size
) 
```




<hr>



### function SetLayout 

```C++
inline virtual void AGE::OpenGLVertexBuffer::SetLayout (
    const BufferLayout & Layout
) override
```



Implements [*AGE::VertexBuffer::SetLayout*](class_a_g_e_1_1_vertex_buffer.md#function-setlayout)


<hr>



### function Unbind 

```C++
virtual void AGE::OpenGLVertexBuffer::Unbind () override const
```



Implements [*AGE::VertexBuffer::Unbind*](class_a_g_e_1_1_vertex_buffer.md#function-unbind)


<hr>



### function ~OpenGLVertexBuffer 

```C++
virtual AGE::OpenGLVertexBuffer::~OpenGLVertexBuffer () 
```




<hr>
## Public Static Functions Documentation




### function GetRendererID 

```C++
static inline uint32_t AGE::OpenGLVertexBuffer::GetRendererID () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

