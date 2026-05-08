

# Class AGE::Renderer2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginScene**](#function-beginscene-12) (const [**Camera**](class_a_g_e_1_1_camera.md) & Camera, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform) <br> |
|  void | [**BeginScene**](#function-beginscene-22) (const [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br> |
|  void | [**DrawCircle**](#function-drawcircle) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, float Thickness=1.f, float Fade=.005f, int EntityID=-1) <br> |
|  void | [**DrawLine**](#function-drawline) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Pos0, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Pos1, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br> |
|  void | [**DrawQuad**](#function-drawquad-13) (const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) & Props) <br> |
|  void | [**DrawQuad**](#function-drawquad-23) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) & Props) <br> |
|  void | [**DrawQuad**](#function-drawquad-33) (const Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; & Subtexture, const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) & Props) <br> |
|  void | [**DrawRect**](#function-drawrect-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Position, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Size, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br> |
|  void | [**DrawRect**](#function-drawrect-22) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br> |
|  void | [**DrawSprite**](#function-drawsprite) ([**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & SRC) <br> |
|  void | [**DrawString**](#function-drawstring) (const [**StringProperties**](struct_a_g_e_1_1_string_properties.md) & Props) <br> |
|  void | [**DrawTileMap**](#function-drawtilemap) (const Ref&lt; [**Tilemap**](class_a_g_e_1_1_tilemap.md) &gt; & Map, const [**TilemapProperties**](struct_a_g_e_1_1_tilemap_properties.md) & Props) <br> |
|  void | [**EndScene**](#function-endscene) () <br> |
|  void | [**Flush**](#function-flush) () <br> |
|  float | [**GetLineWidth**](#function-getlinewidth) () <br> |
|  [**Statistics**](struct_a_g_e_1_1_statistics.md) | [**GetStats**](#function-getstats) () <br> |
|  void | [**Init**](#function-init) () <br> |
|  void | [**SetLineWidth**](#function-setlinewidth) (float Width) <br> |
|  void | [**Shutdown**](#function-shutdown) () <br> |


























## Public Static Functions Documentation




### function BeginScene [1/2]

```C++
static void AGE::Renderer2D::BeginScene (
    const Camera & Camera,
    const Matrix4D & Transform
) 
```




<hr>



### function BeginScene [2/2]

```C++
static void AGE::Renderer2D::BeginScene (
    const EditorCamera & Camera
) 
```




<hr>



### function DrawCircle 

```C++
static void AGE::Renderer2D::DrawCircle (
    const Matrix4D & Transform,
    const Vector4 & Color,
    float Thickness=1.f,
    float Fade=.005f,
    int EntityID=-1
) 
```




<hr>



### function DrawLine 

```C++
static void AGE::Renderer2D::DrawLine (
    const Vector3 & Pos0,
    const Vector3 & Pos1,
    const Vector4 & Color,
    int EntityID=-1
) 
```




<hr>



### function DrawQuad [1/3]

```C++
static void AGE::Renderer2D::DrawQuad (
    const QuadProperties & Props
) 
```




<hr>



### function DrawQuad [2/3]

```C++
static void AGE::Renderer2D::DrawQuad (
    const Ref< Texture2D > & Texture,
    const QuadProperties & Props
) 
```




<hr>



### function DrawQuad [3/3]

```C++
static void AGE::Renderer2D::DrawQuad (
    const Ref< SubTexture2D > & Subtexture,
    const QuadProperties & Props
) 
```




<hr>



### function DrawRect [1/2]

```C++
static void AGE::Renderer2D::DrawRect (
    const Vector3 & Position,
    const Vector2 & Size,
    const Vector4 & Color,
    int EntityID=-1
) 
```




<hr>



### function DrawRect [2/2]

```C++
static void AGE::Renderer2D::DrawRect (
    const Matrix4D & Transform,
    const Vector4 & Color,
    int EntityID=-1
) 
```




<hr>



### function DrawSprite 

```C++
static void AGE::Renderer2D::DrawSprite (
    SpriteRendererComponent & SRC
) 
```




<hr>



### function DrawString 

```C++
static void AGE::Renderer2D::DrawString (
    const StringProperties & Props
) 
```




<hr>



### function DrawTileMap 

```C++
static void AGE::Renderer2D::DrawTileMap (
    const Ref< Tilemap > & Map,
    const TilemapProperties & Props
) 
```




<hr>



### function EndScene 

```C++
static void AGE::Renderer2D::EndScene () 
```




<hr>



### function Flush 

```C++
static void AGE::Renderer2D::Flush () 
```




<hr>



### function GetLineWidth 

```C++
static float AGE::Renderer2D::GetLineWidth () 
```




<hr>



### function GetStats 

```C++
static Statistics AGE::Renderer2D::GetStats () 
```




<hr>



### function Init 

```C++
static void AGE::Renderer2D::Init () 
```




<hr>



### function SetLineWidth 

```C++
static void AGE::Renderer2D::SetLineWidth (
    float Width
) 
```




<hr>



### function Shutdown 

```C++
static void AGE::Renderer2D::Shutdown () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Renderer2D.h`

