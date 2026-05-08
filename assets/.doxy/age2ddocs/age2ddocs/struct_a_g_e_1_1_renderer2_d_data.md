

# Struct AGE::Renderer2DData



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md)




















## Classes

| Type | Name |
| ---: | :--- |
| struct | [**CameraData**](struct_a_g_e_1_1_renderer2_d_data_1_1_camera_data.md) <br> |
| struct | [**TexCoordData**](struct_a_g_e_1_1_renderer2_d_data_1_1_tex_coord_data.md) <br> |






## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**AtlusSlotIndex**](#variable-atlusslotindex)   = `1`<br> |
|  [**CameraData**](struct_a_g_e_1_1_renderer2_d_data_1_1_camera_data.md) | [**CameraBuffer**](#variable-camerabuffer)  <br> |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**CameraUniformBuffer**](#variable-camerauniformbuffer)  <br> |
|  uint32\_t | [**CircleIndexCount**](#variable-circleindexcount)   = `0`<br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**CircleShader**](#variable-circleshader)   = `nullptr`<br> |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**CircleVertexArray**](#variable-circlevertexarray)   = `nullptr`<br> |
|  [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CircleVertexBufferBase**](#variable-circlevertexbufferbase)   = `nullptr`<br> |
|  [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) \* | [**CircleVertexBufferPtr**](#variable-circlevertexbufferptr)   = `nullptr`<br> |
|  [**TexCoordData**](struct_a_g_e_1_1_renderer2_d_data_1_1_tex_coord_data.md) | [**CoordBuffer**](#variable-coordbuffer)  <br> |
|  Ref&lt; class [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; | [**CurrentTilemap**](#variable-currenttilemap)  <br> |
|  std::array&lt; Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt;, MaxTextureSlots &gt; | [**FontAtlasTextures**](#variable-fontatlastextures)  <br> |
|  [**ShaderLibrary**](class_a_g_e_1_1_shader_library.md) | [**Library**](#variable-library)  <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**LineShader**](#variable-lineshader)  <br> |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**LineVertexArray**](#variable-linevertexarray)  <br> |
|  [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**LineVertexBufferBase**](#variable-linevertexbufferbase)   = `nullptr`<br> |
|  [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) \* | [**LineVertexBufferPtr**](#variable-linevertexbufferptr)   = `nullptr`<br> |
|  uint32\_t | [**LineVertexCount**](#variable-linevertexcount)   = `0`<br> |
|  float | [**LineWidth**](#variable-linewidth)   = `2.f`<br> |
|  uint32\_t | [**QuadIndexCount**](#variable-quadindexcount)   = `0`<br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**QuadShader**](#variable-quadshader)   = `nullptr`<br> |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**QuadVertexArray**](#variable-quadvertexarray)   = `nullptr`<br> |
|  [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**QuadVertexBufferBase**](#variable-quadvertexbufferbase)   = `nullptr`<br> |
|  [**Vertex**](struct_a_g_e_1_1_vertex.md) \* | [**QuadVertexBufferPtr**](#variable-quadvertexbufferptr)   = `nullptr`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**QuadVertexPositions**](#variable-quadvertexpositions)  <br> |
|  [**Statistics**](struct_a_g_e_1_1_statistics.md) | [**Stats**](#variable-stats)  <br> |
|  Ref&lt; [**UniformBuffer**](class_a_g_e_1_1_uniform_buffer.md) &gt; | [**TexCoordUniformBuffer**](#variable-texcoorduniformbuffer)  <br> |
|  uint32\_t | [**TextIndexCount**](#variable-textindexcount)   = `0`<br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**TextShader**](#variable-textshader)  <br> |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**TextVertexArray**](#variable-textvertexarray)  <br> |
|  [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**TextVertexBufferBase**](#variable-textvertexbufferbase)   = `nullptr`<br> |
|  [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) \* | [**TextVertexBufferPtr**](#variable-textvertexbufferptr)   = `nullptr`<br> |
|  uint32\_t | [**TextureSlotIndex**](#variable-textureslotindex)   = `1`<br> |
|  std::array&lt; Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt;, MaxTextureSlots &gt; | [**TextureSlots**](#variable-textureslots)  <br> |
|  uint32\_t | [**TileIndexCount**](#variable-tileindexcount)   = `0`<br> |
|  std::array&lt; Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt;, MaxTextureSlots &gt; | [**TileSetTextures**](#variable-tilesettextures)  <br> |
|  Ref&lt; [**Shader**](class_a_g_e_1_1_shader.md) &gt; | [**TileShader**](#variable-tileshader)  <br> |
|  Ref&lt; [**VertexArray**](class_a_g_e_1_1_vertex_array.md) &gt; | [**TileVertexArray**](#variable-tilevertexarray)  <br> |
|  [**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* | [**TileVertexBufferBase**](#variable-tilevertexbufferbase)  <br> |
|  [**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) \* | [**TileVertexBufferPtr**](#variable-tilevertexbufferptr)  <br> |
|  uint32\_t | [**TileVertexCount**](#variable-tilevertexcount)   = `0`<br> |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**TileVertexPositions**](#variable-tilevertexpositions)  <br> |
|  uint32\_t | [**TilesetSlotIndex**](#variable-tilesetslotindex)   = `1`<br> |
|  std::unordered\_map&lt; std::string, Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; &gt; | [**VertexBuffers**](#variable-vertexbuffers)  <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**WhiteTexture**](#variable-whitetexture)   = `nullptr`<br> |


## Public Static Attributes

| Type | Name |
| ---: | :--- |
|  const uint32\_t | [**MaxIndexCount**](#variable-maxindexcount)   = `MaxQuadCount \* 6`<br> |
|  const uint32\_t | [**MaxQuadCount**](#variable-maxquadcount)   = `20000`<br> |
|  const uint32\_t | [**MaxTextureSlots**](#variable-maxtextureslots)   = `32`<br> |
|  const uint32\_t | [**MaxVertices**](#variable-maxvertices)   = `MaxQuadCount \* 4`<br> |














## Public Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**VertexBuffer**](class_a_g_e_1_1_vertex_buffer.md) &gt; | [**GetVertexBuffer**](#function-getvertexbuffer) (const std::string & Name) <br> |




























## Public Attributes Documentation




### variable AtlusSlotIndex 

```C++
uint32_t AGE::Renderer2DData::AtlusSlotIndex;
```




<hr>



### variable CameraBuffer 

```C++
CameraData AGE::Renderer2DData::CameraBuffer;
```




<hr>



### variable CameraUniformBuffer 

```C++
Ref<UniformBuffer> AGE::Renderer2DData::CameraUniformBuffer;
```




<hr>



### variable CircleIndexCount 

```C++
uint32_t AGE::Renderer2DData::CircleIndexCount;
```




<hr>



### variable CircleShader 

```C++
Ref<Shader> AGE::Renderer2DData::CircleShader;
```




<hr>



### variable CircleVertexArray 

```C++
Ref<VertexArray> AGE::Renderer2DData::CircleVertexArray;
```




<hr>



### variable CircleVertexBufferBase 

```C++
CircleVertex* AGE::Renderer2DData::CircleVertexBufferBase;
```




<hr>



### variable CircleVertexBufferPtr 

```C++
CircleVertex* AGE::Renderer2DData::CircleVertexBufferPtr;
```




<hr>



### variable CoordBuffer 

```C++
TexCoordData AGE::Renderer2DData::CoordBuffer;
```




<hr>



### variable CurrentTilemap 

```C++
Ref<class Tilemap> AGE::Renderer2DData::CurrentTilemap;
```




<hr>



### variable FontAtlasTextures 

```C++
std::array<Ref<Texture2D>, MaxTextureSlots> AGE::Renderer2DData::FontAtlasTextures;
```




<hr>



### variable Library 

```C++
ShaderLibrary AGE::Renderer2DData::Library;
```




<hr>



### variable LineShader 

```C++
Ref<Shader> AGE::Renderer2DData::LineShader;
```




<hr>



### variable LineVertexArray 

```C++
Ref<VertexArray> AGE::Renderer2DData::LineVertexArray;
```




<hr>



### variable LineVertexBufferBase 

```C++
LineVertex* AGE::Renderer2DData::LineVertexBufferBase;
```




<hr>



### variable LineVertexBufferPtr 

```C++
LineVertex* AGE::Renderer2DData::LineVertexBufferPtr;
```




<hr>



### variable LineVertexCount 

```C++
uint32_t AGE::Renderer2DData::LineVertexCount;
```




<hr>



### variable LineWidth 

```C++
float AGE::Renderer2DData::LineWidth;
```




<hr>



### variable QuadIndexCount 

```C++
uint32_t AGE::Renderer2DData::QuadIndexCount;
```




<hr>



### variable QuadShader 

```C++
Ref<Shader> AGE::Renderer2DData::QuadShader;
```




<hr>



### variable QuadVertexArray 

```C++
Ref<VertexArray> AGE::Renderer2DData::QuadVertexArray;
```




<hr>



### variable QuadVertexBufferBase 

```C++
Vertex* AGE::Renderer2DData::QuadVertexBufferBase;
```




<hr>



### variable QuadVertexBufferPtr 

```C++
Vertex* AGE::Renderer2DData::QuadVertexBufferPtr;
```




<hr>



### variable QuadVertexPositions 

```C++
Vector4 AGE::Renderer2DData::QuadVertexPositions[4];
```




<hr>



### variable Stats 

```C++
Statistics AGE::Renderer2DData::Stats;
```




<hr>



### variable TexCoordUniformBuffer 

```C++
Ref<UniformBuffer> AGE::Renderer2DData::TexCoordUniformBuffer;
```




<hr>



### variable TextIndexCount 

```C++
uint32_t AGE::Renderer2DData::TextIndexCount;
```




<hr>



### variable TextShader 

```C++
Ref<Shader> AGE::Renderer2DData::TextShader;
```




<hr>



### variable TextVertexArray 

```C++
Ref<VertexArray> AGE::Renderer2DData::TextVertexArray;
```




<hr>



### variable TextVertexBufferBase 

```C++
TextVertex* AGE::Renderer2DData::TextVertexBufferBase;
```




<hr>



### variable TextVertexBufferPtr 

```C++
TextVertex* AGE::Renderer2DData::TextVertexBufferPtr;
```




<hr>



### variable TextureSlotIndex 

```C++
uint32_t AGE::Renderer2DData::TextureSlotIndex;
```




<hr>



### variable TextureSlots 

```C++
std::array<Ref<Texture2D>, MaxTextureSlots> AGE::Renderer2DData::TextureSlots;
```




<hr>



### variable TileIndexCount 

```C++
uint32_t AGE::Renderer2DData::TileIndexCount;
```




<hr>



### variable TileSetTextures 

```C++
std::array<Ref<Texture2D>, MaxTextureSlots> AGE::Renderer2DData::TileSetTextures;
```




<hr>



### variable TileShader 

```C++
Ref<Shader> AGE::Renderer2DData::TileShader;
```




<hr>



### variable TileVertexArray 

```C++
Ref<VertexArray> AGE::Renderer2DData::TileVertexArray;
```




<hr>



### variable TileVertexBufferBase 

```C++
TilemapVertex* AGE::Renderer2DData::TileVertexBufferBase;
```




<hr>



### variable TileVertexBufferPtr 

```C++
TilemapVertex* AGE::Renderer2DData::TileVertexBufferPtr;
```




<hr>



### variable TileVertexCount 

```C++
uint32_t AGE::Renderer2DData::TileVertexCount;
```




<hr>



### variable TileVertexPositions 

```C++
Vector4 AGE::Renderer2DData::TileVertexPositions[6];
```




<hr>



### variable TilesetSlotIndex 

```C++
uint32_t AGE::Renderer2DData::TilesetSlotIndex;
```




<hr>



### variable VertexBuffers 

```C++
std::unordered_map<std::string, Ref<VertexBuffer> > AGE::Renderer2DData::VertexBuffers;
```




<hr>



### variable WhiteTexture 

```C++
Ref<Texture2D> AGE::Renderer2DData::WhiteTexture;
```




<hr>
## Public Static Attributes Documentation




### variable MaxIndexCount 

```C++
const uint32_t AGE::Renderer2DData::MaxIndexCount;
```




<hr>



### variable MaxQuadCount 

```C++
const uint32_t AGE::Renderer2DData::MaxQuadCount;
```




<hr>



### variable MaxTextureSlots 

```C++
const uint32_t AGE::Renderer2DData::MaxTextureSlots;
```




<hr>



### variable MaxVertices 

```C++
const uint32_t AGE::Renderer2DData::MaxVertices;
```




<hr>
## Public Functions Documentation




### function GetVertexBuffer 

```C++
inline Ref< VertexBuffer > AGE::Renderer2DData::GetVertexBuffer (
    const std::string & Name
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Pipeline.h`

