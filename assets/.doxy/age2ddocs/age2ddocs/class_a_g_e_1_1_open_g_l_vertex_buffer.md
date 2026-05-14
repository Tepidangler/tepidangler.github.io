

# Class AGE::OpenGLVertexBuffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md)








Inherits the following classes: [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-12) (float \* Verticies, uint32\_t Size) override<br>_Adds data to the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual void | [**AddDataToBuffer**](#function-adddatatobuffer-22) (const void \* Verticies, uint32\_t Size) override<br>_Adds data to the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual void | [**Bind**](#function-bind) () override const<br>_This function binds the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _to the GL\_ARRAY\_BUFFER target._ |
| virtual [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CreateCircle**](#function-createcircle) ([**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, float Thickness, float Fade, int EntID) override<br>_Creates a circle in the vertex buffer._  |
| virtual [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**CreateLine**](#function-createline) ([**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position0, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position1, int EntID) override<br>_Creates a line vertex in the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**CreateQuad**](#function-createquad) ([**Vertex**](struct_a_g_e_1_1_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) override<br>_Creates a quad in the OpenGL vertex buffer._  |
| virtual [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**CreateText**](#function-createtext) ([**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TexID, int EntID) override<br>_This function creates a text vertex in an OpenGL vertex buffer._  |
| virtual [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* | [**CreateTile**](#function-createtile) ([**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) override<br>_Creates a tile with the given parameters and stores it in the provided_ [_**TileVertex**_](struct_a_g_e_1_1_tile_vertex.md) _object._ |
| virtual const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & | [**GetLayout**](#function-getlayout) () override const<br>_Returns the layout of this buffer._  |
| virtual void | [**InvalidateBuffer**](#function-invalidatebuffer) () override const<br>_Invalidates and deletes the OpenGL vertex buffer._  |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-13) (uint32\_t Size) <br>_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _with a given size._ |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-23) ([**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) \* Vertices, uint32\_t Size) <br>_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _object._ |
|   | [**OpenGLVertexBuffer**](#function-openglvertexbuffer-33) (float \* Vertices, uint32\_t Size) <br>_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _with given vertices and size._ |
| virtual void | [**SetLayout**](#function-setlayout) (const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & Layout) override<br>_Sets the layout for a buffer._  |
| virtual void | [**Unbind**](#function-unbind) () override const<br>_Unbinds the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._ |
| virtual  | [**~OpenGLVertexBuffer**](#function-openglvertexbuffer) () <br>_Destructor for_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _. Deletes the vertex buffer object from GPU memory._ |


## Public Functions inherited from AGE::VertexBuffer

See [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)

| Type | Name |
| ---: | :--- |
| virtual void | [**AddDataToBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-12) (float \* Verticies, uint32\_t Size) = 0<br> |
| virtual void | [**AddDataToBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-22) (const void \* Verticies, uint32\_t Size) = 0<br> |
|  T \* | [**As**](class_a_g_e_1_1_vertex_buffer.md#function-as) () <br>_This function is currently not implemented and will always throw an assertion. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
| virtual void | [**Bind**](class_a_g_e_1_1_vertex_buffer.md#function-bind) () const = 0<br> |
| virtual [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CreateCircle**](class_a_g_e_1_1_vertex_buffer.md#function-createcircle) ([**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, float Thickness, float Fade, int EntID) = 0<br> |
| virtual [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**CreateLine**](class_a_g_e_1_1_vertex_buffer.md#function-createline) ([**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position0, [**Vector3**](struct_a_g_e_1_1_vector3.md) Position1, int EntID=-1) = 0<br> |
| virtual [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**CreateQuad**](class_a_g_e_1_1_vertex_buffer.md#function-createquad) ([**Vertex**](struct_a_g_e_1_1_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) = 0<br> |
| virtual [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**CreateText**](class_a_g_e_1_1_vertex_buffer.md#function-createtext) ([**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* Target, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TexID, int EntID) = 0<br> |
| virtual [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* | [**CreateTile**](class_a_g_e_1_1_vertex_buffer.md#function-createtile) ([**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) \* Target, [**Vector4**](struct_a_g_e_1_1_vector4.md) Color, [**Vector4**](struct_a_g_e_1_1_vector4.md) \* Position, [**Vector2**](struct_a_g_e_1_1_vector2.md) Size, [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Transform, const [**Vector2**](struct_a_g_e_1_1_vector2.md) \* TexCoords, float TilingFactor, float ID, int EnttID) = 0<br> |
| virtual const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & | [**GetLayout**](class_a_g_e_1_1_vertex_buffer.md#function-getlayout) () const = 0<br> |
| virtual void | [**InvalidateBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-invalidatebuffer) () const = 0<br> |
| virtual void | [**SetLayout**](class_a_g_e_1_1_vertex_buffer.md#function-setlayout) (const [**BufferLayout**](class_a_g_e_1_1_buffer_layout.md) & Layout) = 0<br> |
| virtual void | [**Unbind**](class_a_g_e_1_1_vertex_buffer.md#function-unbind) () const = 0<br> |
| virtual  | [**~VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md#function-vertexbuffer) () <br>_Virtual destructor for the_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetRendererID**](#function-getrendererid) () <br>_Returns the renderer ID of the current scene._  |


## Public Static Functions inherited from AGE::VertexBuffer

See [AGE::VertexBuffer](class_a_g_e_1_1_vertex_buffer.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-13) ([**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) \* Vertices, uint32\_t Size) <br> |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-23) (uint32\_t Size) <br>_Creates a new_ [_**VertexBuffer**_](class_a_g_e_1_1_vertex_buffer.md) _of the specified size. The type and usage of the buffer are determined by the current Rendering API in use._ |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**Create**](class_a_g_e_1_1_vertex_buffer.md#function-create-33) (float \* Vertices=nullptr, uint32\_t Size=0) <br>_Creates a new vertex buffer object._  |


















































## Public Functions Documentation




### function AddDataToBuffer [1/2]

_Adds data to the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual void AGE::OpenGLVertexBuffer::AddDataToBuffer (
    float * Verticies,
    uint32_t Size
) override
```



This function binds the buffer and adds new data to it using glBufferSubData. The data is added at the beginning of the buffer, replacing any existing data.




**Parameters:**


* `Verticies` Pointer to an array of floats containing the data to be added. 
* `Size` The size in bytes of the data to be added.



**Returns:**

void


Adds data to the OpenGL [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md).


This function binds the buffer and then uses glBufferSubData to add new data at the beginning of the buffer. The size of the data is specified by the Size parameter, which should be the number of floats in the Verticies array.




**Parameters:**


* `Verticies` Pointer to an array of float values representing the vertices to add to the buffer. 
* `Size` The size of the Verticies array, expressed as a uint32\_t. This should be equal to the number of floats in the Verticies array.



**Returns:**

void 





        
Implements [*AGE::VertexBuffer::AddDataToBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-12)


<hr>



### function AddDataToBuffer [2/2]

_Adds data to the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual void AGE::OpenGLVertexBuffer::AddDataToBuffer (
    const void * Verticies,
    uint32_t Size
) override
```



This function binds the buffer and updates its contents with new vertex data. The size of the data is specified by the 'Size' parameter, which should match the actual size of the data being added. The data itself is passed as a pointer to the 'Verticies' parameter.




**Parameters:**


* `Verticies` A pointer to the data that will be copied into the buffer. 
* `Size` The size in bytes of the data pointed to by 'Verticies'.



**Returns:**

void


Adds data to the OpenGL [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md).


This function binds the buffer and then uses glBufferSubData to add new data at the beginning of the buffer. The size of the data is specified by the Size parameter, and the actual data is pointed to by the Verticies pointer.




**Parameters:**


* `Verticies` A pointer to the data that will be added to the buffer. 
* `Size` The size in bytes of the data being added.



**Returns:**

void 





        
Implements [*AGE::VertexBuffer::AddDataToBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-adddatatobuffer-22)


<hr>



### function Bind 

_This function binds the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _to the GL\_ARRAY\_BUFFER target._
```C++
virtual void AGE::OpenGLVertexBuffer::Bind () override const
```



The function uses glBindBuffer() from the OpenGL library to bind the buffer with ID m\_RendererID to the GL\_ARRAY\_BUFFER target. It is used when rendering vertex data in an OpenGL context.




**Returns:**

void No return value. This function only modifies the state of the OpenGL context, not returning any information.


This function binds the OpenGL [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md) to the GL\_ARRAY\_BUFFER target.


The function uses glBindBuffer with arguments (GL\_ARRAY\_BUFFER, m\_RendererID) to bind the buffer. It is used when rendering vertex arrays and it sets the current vertex array buffer to be the one we want to use.




**Returns:**

void No return value. 





        
Implements [*AGE::VertexBuffer::Bind*](class_a_g_e_1_1_vertex_buffer.md#function-bind)


<hr>



### function CreateCircle 

_Creates a circle in the vertex buffer._ 
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



This function takes an array of positions, applies a transformation to each position, and stores them into the target [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) object. The color, thickness, fade factor, and entity ID are also stored for each vertex.




**Parameters:**


* `Target` Pointer to the [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) object where the circle will be created. 
* `Transform` The transformation matrix that will be applied to the positions. 
* `Position` An array of [**Vector4**](struct_a_g_e_1_1_vector4.md) objects representing the positions of the vertices of the circle. 
* `Color` The color of the circle. 
* `Thickness` The thickness of the lines making up the circle. 
* `Fade` The fade factor of the circle. 
* `EntID` The entity ID associated with the circle.



**Returns:**

Pointer to the [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) object where the circle was created.


Creates a circle vertex in the [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md).


This function takes an array of positions, applies a transformation to each position, and stores the transformed position, local position, color, thickness, fade, and entity ID into a [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) struct. The function returns the updated target pointer.




**Parameters:**


* `Target` Pointer to the [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) that will be populated with data. 
* `Transform` The transformation matrix to apply to each position. 
* `Position` Array of positions to transform and store in the vertex. 
* `Color` The color of the circle. 
* `Thickness` The thickness of the circle lines. 
* `Fade` The fade value for the circle. 
* `EntID` The entity ID associated with the circle.



**Returns:**

Pointer to the updated [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) struct. 





        
Implements [*AGE::VertexBuffer::CreateCircle*](class_a_g_e_1_1_vertex_buffer.md#function-createcircle)


<hr>



### function CreateLine 

_Creates a line vertex in the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual LineVertex * AGE::OpenGLVertexBuffer::CreateLine (
    LineVertex * Target,
    Vector4 Color,
    Vector3 Position0,
    Vector3 Position1,
    int EntID
) override
```



This function takes in parameters to create two vertices that form a line. The first vertex has its position set to Position0, color set to Color and LineEntityID set to EntID. The second vertex is similar but uses Position1 for its position. 

**Parameters:**


* `Target` Pointer to the target [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md) object where the new line will be added. 
* `Color` The color of the line. 
* `Position0` The starting point of the line. 
* `Position1` The ending point of the line. 
* `EntID` The entity ID associated with this line. 



**Returns:**

Pointer to the next available memory location in the [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md) object after adding two vertices.


Creates a line vertex in the OpenGL [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md).


This function creates two vertices that form a line segment. The first vertex has its position set to Position0, color set to Color and LineEntityID set to EntID. The second vertex is similar but uses Position1 for its position.




**Parameters:**


* `Target` Pointer to the target [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) object where the new vertices will be created. 
* `Color` The color of the line segment. 
* `Position0` The starting point of the line segment. 
* `Position1` The ending point of the line segment. 
* `EntID` The entity ID associated with the line segment.



**Returns:**

Pointer to the next available [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) object after two vertices have been created. 





        
Implements [*AGE::VertexBuffer::CreateLine*](class_a_g_e_1_1_vertex_buffer.md#function-createline)


<hr>



### function CreateQuad 

_Creates a quad in the OpenGL vertex buffer._ 
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



This function takes in various parameters to create a quad, such as color, position, size, texture coordinates, tiling factor, and entity ID. It then populates an array of vertices with these details. The resulting array is returned by reference.




**Parameters:**


* `Target` Pointer to the first element of the vertex array to be filled. 
* `Color` The color of the quad. 
* `Position` An array of positions for each vertex of the quad. 
* `Size` The size of the quad. 
* `Transform` The transformation matrix that will be applied to the vertices' positions. 
* `TexCoords` An array of texture coordinates for each vertex of the quad. 
* `TilingFactor` The tiling factor for the texture. 
* `ID` The ID of the texture being used. 
* `EnttID` The entity ID associated with the quad.



**Returns:**

Pointer to the filled vertex array.


Creates a quad in the OpenGL vertex buffer.


This function takes an array of vertices, colors, positions, texture coordinates, and other parameters to create a quad in the vertex buffer. The quad is created by filling four vertices with data from the provided arguments.




**Parameters:**


* `Target` Pointer to the first element of the target array of vertices. 
* `Color` The color of the quad. 
* `Position` An array of positions for each vertex of the quad. 
* `Size` The size of the quad. 
* `Transform` The transformation matrix applied to the quad's position. 
* `TexCoords` An array of texture coordinates for each vertex of the quad. 
* `TilingFactor` The tiling factor used in the texture mapping. 
* `ID` The ID of the texture used by the quad. 
* `EnttID` The ID of the entity associated with the quad.



**Returns:**

Pointer to the next available position after creating the quad. 





        
Implements [*AGE::VertexBuffer::CreateQuad*](class_a_g_e_1_1_vertex_buffer.md#function-createquad)


<hr>



### function CreateText 

_This function creates a text vertex in an OpenGL vertex buffer._ 
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



The function takes in several parameters including the target [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) pointer, a transformation matrix, position vectors, color, texture coordinates and texture ID. It then populates each of these values into the target [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) object for each vertex in the quadrilateral.




**Parameters:**


* `Target` Pointer to the [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) that will be filled with data. 
* `Transform` The transformation matrix used to transform the position vectors. 
* `Position` An array of [**Vector4**](struct_a_g_e_1_1_vector4.md) positions which represent the vertices of a text quadrilateral. 
* `Color` The color of the text. 
* `TexCoords` An array of [**Vector2**](struct_a_g_e_1_1_vector2.md) texture coordinates for each vertex in the text quadrilateral. 
* `TexID` The ID of the texture to be used for rendering the text. 
* `EntID` The entity ID associated with the text.



**Returns:**

Pointer to the filled [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) object.


This function creates a text vertex in an OpenGL vertex buffer.


The function takes in several parameters such as the target [**TextVertex**](struct_a_g_e_1_1_text_vertex.md), transformation matrix, position vector, color, texture coordinates, texture ID and entity ID. It then populates each of these values into the target [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) object for each vertex in the quadrilateral.




**Parameters:**


* `Target` Pointer to a [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) that will be filled with data. 
* `Transform` The transformation matrix used to transform the position vector. 
* `Position` An array of [**Vector4**](struct_a_g_e_1_1_vector4.md) positions which represent the vertices of the text. 
* `Color` The color of the text vertex. 
* `TexCoords` An array of [**Vector2**](struct_a_g_e_1_1_vector2.md) texture coordinates for each vertex in the quadrilateral. 
* `TexID` The ID of the texture to be used for rendering the text. 
* `EntID` The entity ID associated with this text vertex.



**Returns:**

Pointer to the filled [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) object. 





        
Implements [*AGE::VertexBuffer::CreateText*](class_a_g_e_1_1_vertex_buffer.md#function-createtext)


<hr>



### function CreateTile 

_Creates a tile with the given parameters and stores it in the provided_ [_**TileVertex**_](struct_a_g_e_1_1_tile_vertex.md) _object._
```C++
virtual TileVertex * AGE::OpenGLVertexBuffer::CreateTile (
    TileVertex * Target,
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



This function takes an array of positions, texture coordinates, color, tiling factor, entity ID, and transforms them into vertex data for a quadrilateral tile. The resulting vertex data is stored in the provided `TileVertex` object. 

**Parameters:**


* `Target` Pointer to the [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) object where the created tile will be stored. 
* `Color` The color of the tile. 
* `Position` An array of positions that define the corners of the tile. 
* `Size` The size of the tile. 
* `Transform` A transformation matrix applied to the positions. 
* `TexCoords` An array of texture coordinates for each corner of the tile. 
* `TilingFactor` The tiling factor used in the texture mapping. 
* `ID` The ID of the texture used by the tile. 
* `EnttID` The entity ID associated with the tile.



**Returns:**

Pointer to the `TileVertex` object where the created tile is stored.


This function creates a tile with the given parameters.


The function takes in an array of positions, texture coordinates, color, tiling factor, entity ID and transforms them into vertices for a quadrilateral mesh. It then updates the target [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) object with these vertex attributes. 

**Parameters:**


* `Target` Pointer to the [**TileVertex**](struct_a_g_e_1_1_tile_vertex.md) object that will be updated. 
* `Color` The color of the tile. 
* `Position` An array of positions for each vertex of the tile. 
* `Size` The size of the tile. 
* `Transform` The transformation matrix applied to the vertices. 
* `TexCoords` An array of texture coordinates for each vertex of the tile. 
* `TilingFactor` The tiling factor used in the texture mapping. 
* `ID` The ID of the texture being used. 
* `EnttID` The entity ID associated with the tile.



**Returns:**

Pointer to the updated Target object. 





        
Implements [*AGE::VertexBuffer::CreateTile*](class_a_g_e_1_1_vertex_buffer.md#function-createtile)


<hr>



### function GetLayout 

_Returns the layout of this buffer._ 
```C++
inline virtual const BufferLayout & AGE::OpenGLVertexBuffer::GetLayout () override const
```





**Returns:**

A constant reference to the buffer's layout. 





        
Implements [*AGE::VertexBuffer::GetLayout*](class_a_g_e_1_1_vertex_buffer.md#function-getlayout)


<hr>



### function InvalidateBuffer 

_Invalidates and deletes the OpenGL vertex buffer._ 
```C++
virtual void AGE::OpenGLVertexBuffer::InvalidateBuffer () override const
```



This function first invalidates any existing data in the buffer using glInvalidateBufferData(). Then it deletes the buffer itself with glDeleteBuffers(). The buffer's ID is passed to these functions as a constant reference, ensuring that no changes are made to the buffer after its destruction.




**Returns:**

void


Invalidates and deletes the OpenGL vertex buffer.


This function first invalidates any existing data in the buffer using glInvalidateBufferData(). It then deletes the buffer itself with glDeleteBuffers() using the renderer ID of this object as argument. The buffer is marked for deletion and its memory becomes available for reuse by other objects, effectively invalidating it.




**Returns:**

void 





        
Implements [*AGE::VertexBuffer::InvalidateBuffer*](class_a_g_e_1_1_vertex_buffer.md#function-invalidatebuffer)


<hr>



### function OpenGLVertexBuffer [1/3]

_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _with a given size._
```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    uint32_t Size
) 
```



This function creates an OpenGL buffer and initializes it with the specified size, data type (`GL_ARRAY_BUFFER`), and usage pattern (`GL_DYNAMIC_DRAW`). The created buffer is bound to the target `GL_ARRAY_BUFFER`.




**Parameters:**


* `Size` The size of the buffer in bytes.

Constructs an [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md) with a specified size.


This function creates an OpenGL buffer and initializes it with the given size. The buffer is created as dynamic, meaning its content can be changed frequently without needing to reallocate memory.




**Parameters:**


* `Size` The size of the buffer in bytes. 




        

<hr>



### function OpenGLVertexBuffer [2/3]

_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _object._
```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    Matrix3D * Vertices,
    uint32_t Size
) 
```



This function creates a buffer and binds it to the target GL\_ARRAY\_BUFFER, then initializes its data with the provided vertices. The size of the data is specified by the Size parameter.




**Parameters:**


* `Vertices` Pointer to an array of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) objects representing the vertices for initialization. 
* `Size` Number of bytes in the Vertices array.



**Returns:**

None


Constructor for [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md). Initializes a vertex buffer object with the given vertices and size. The buffer is created as dynamic, meaning its content can be changed frequently.




**Parameters:**


* `Vertices` Pointer to an array of [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) objects representing the vertices. 
* `Size` Number of elements in the Vertices array. 




        

<hr>



### function OpenGLVertexBuffer [3/3]

_Constructs an_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _with given vertices and size._
```C++
AGE::OpenGLVertexBuffer::OpenGLVertexBuffer (
    float * Vertices,
    uint32_t Size
) 
```



This function creates a new OpenGL vertex buffer object (VBO) using the `glCreateBuffers` function, assigns it a unique ID, binds it for use, and fills it with data using `glBufferData`. The data is specified as an array of floats and its size in bytes.




**Parameters:**


* `Vertices` Pointer to the first element of the vertices array. 
* `Size` Number of bytes to allocate memory for the buffer object's data store.

Constructs an [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md) with given vertices and size.


This function creates a new OpenGL vertex buffer object (VBO) using the `glCreateBuffers` function, assigns it a unique ID, binds it to the GL\_ARRAY\_BUFFER target, and fills it with data of specified size and content. 

**Parameters:**


* `Vertices` Pointer to an array of float values representing vertices. 
* `Size` The size in bytes of the buffer object's new data store. 




        

<hr>



### function SetLayout 

_Sets the layout for a buffer._ 
```C++
inline virtual void AGE::OpenGLVertexBuffer::SetLayout (
    const BufferLayout & Layout
) override
```





**Parameters:**


* `Layout` The new layout to be set. 




        
Implements [*AGE::VertexBuffer::SetLayout*](class_a_g_e_1_1_vertex_buffer.md#function-setlayout)


<hr>



### function Unbind 

_Unbinds the OpenGL_ [_**Vertex**_](struct_a_g_e_1_1_vertex.md) __[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _._
```C++
virtual void AGE::OpenGLVertexBuffer::Unbind () override const
```



This function binds an OpenGL buffer to a target with zero as its argument. In this case, it's binding GL\_ARRAY\_BUFFER to 0, effectively unbinding it.




**Returns:**

void


This function unbinds the OpenGL [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md).


It binds the buffer target to GL\_ARRAY\_BUFFER and sets the buffer id to 0, effectively unbinding it from the current context.




**Returns:**

void 





        
Implements [*AGE::VertexBuffer::Unbind*](class_a_g_e_1_1_vertex_buffer.md#function-unbind)


<hr>



### function ~OpenGLVertexBuffer 

_Destructor for_ [_**OpenGLVertexBuffer**_](class_a_g_e_1_1_open_g_l_vertex_buffer.md) _. Deletes the vertex buffer object from GPU memory._
```C++
virtual AGE::OpenGLVertexBuffer::~OpenGLVertexBuffer () 
```



This function is responsible for deleting a [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md) Object (VBO) from the GPU's memory. It does this by calling glDeleteBuffers with the ID of the VBO to be deleted. The VBO ID is stored in m\_RendererID member variable.




**Returns:**

void


Destructor for [**OpenGLVertexBuffer**](class_a_g_e_1_1_open_g_l_vertex_buffer.md). Deletes the vertex buffer object from GPU memory.


This function is responsible for deleting a [**Vertex**](struct_a_g_e_1_1_vertex.md) [**Buffer**](struct_a_g_e_1_1_buffer.md) Object (VBO) from the GPU's memory. The VBO was previously created and initialized by some other part of the program.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function GetRendererID 

_Returns the renderer ID of the current scene._ 
```C++
static inline uint32_t AGE::OpenGLVertexBuffer::GetRendererID () 
```



This function returns the unique identifier for the renderer used by the current scene. The returned value is a uint32\_t, which represents an unsigned integer type in C++.




**Returns:**

A uint32\_t representing the renderer ID of the current scene. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLBuffer.h`

