

# Class AGE::Renderer2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginScene**](#function-beginscene-12) (const [**Camera**](class_a_g_e_1_1_camera.md) & Camera, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform) <br>_Begins a 2D scene with the specified camera and transformation._  |
|  void | [**BeginScene**](#function-beginscene-22) (const [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) & Camera) <br>_Begin a 2D scene with the given camera._  |
|  void | [**DrawCircle**](#function-drawcircle) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, float Thickness=1.f, float Fade=.005f, int EntityID=-1) <br>_Draw a circle on the screen using the provided parameters._  |
|  void | [**DrawLine**](#function-drawline) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Pos0, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Pos1, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br>_Draw a line in the 3D scene._  |
|  void | [**DrawQuad**](#function-drawquad-13) (const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) Props) <br>_Draw a quadrilateral with the specified properties._  |
|  void | [**DrawQuad**](#function-drawquad-23) (const Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & Texture, const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) Props) <br>_Draw a quad with the given properties and texture._  _\*_ _\* This function is used to draw a single quad in the 2D graphics pipeline. It takes as input the texture, quad properties (color, size, transform, texture coordinates, tiling factor, entity ID), and it updates the vertex buffer accordingly. If the current batch of quads exceeds the maximum index count, it will start a new batch._ _\*_ _\*._ |
|  void | [**DrawQuad**](#function-drawquad-33) (const Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; & Subtexture, const [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) Props) <br>_Draw a quad using the provided properties and subtexture._  |
|  void | [**DrawRect**](#function-drawrect-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Position, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Size, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br>_Draws a 2D rectangle on the screen._  |
|  void | [**DrawRect**](#function-drawrect-22) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Color, int EntityID=-1) <br>_Draws a 2D rectangle using lines._  |
|  void | [**DrawSprite**](#function-drawsprite) ([**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & SRC) <br>_Draws a 2D sprite based on the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _provided._ |
|  void | [**DrawString**](#function-drawstring) (const [**StringProperties**](struct_a_g_e_1_1_string_properties.md) & Props) <br> |
|  void | [**DrawTile**](#function-drawtile) (const [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) & SRC) <br>_Draws a single tile using the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _data._ _\*_ _\* This function updates necessary buffers and statistics as needed, based on the details provided by the_[_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _._ _\*_ _\*._ |
|  void | [**DrawTileMapLayers**](#function-drawtilemaplayers) ([**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md) & TMRC, tmx\_map \* Map, std::vector&lt; tmx\_layer \* &gt; layers) <br>_Draws a tile map layer using the provided_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _, tmx\_map and vector of tmx\_layer objects._ |
|  void | [**EndScene**](#function-endscene) () <br>_This function is used to end the current scene rendering in a 2D context. It calls the Flush2D method of the currently active GraphicsPipeline object, which should handle any remaining rendering tasks for this frame._  |
|  void | [**Flush**](#function-flush) () <br>_This function flushes the 2D rendering pipeline._  |
|  float | [**GetLineWidth**](#function-getlinewidth) () <br>_This function returns the current line width._  |
|  [**Statistics**](struct_a_g_e_1_1_statistics.md) | [**GetStats**](#function-getstats) () <br>_Get the statistics of the 2D renderer._  |
|  void | [**Init**](#function-init) () <br>_Initializes the_ [_**Renderer2D**_](class_a_g_e_1_1_renderer2_d.md) _object._ |
|  void | [**SetLineWidth**](#function-setlinewidth) (float Width) <br>_Set the line width for rendering._  |
|  void | [**Shutdown**](#function-shutdown) () <br>_Shuts down the_ [_**Renderer2D**_](class_a_g_e_1_1_renderer2_d.md) _instance._ |


























## Public Static Functions Documentation




### function BeginScene [1/2]

_Begins a 2D scene with the specified camera and transformation._ 
```C++
static void AGE::Renderer2D::BeginScene (
    const Camera & Camera,
    const Matrix4D & Transform
) 
```



This function starts a new batch for rendering 2D objects, using the provided camera and transformation matrix. The camera is used to calculate the view-projection matrix that will be applied during rendering.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) A const reference to the camera object representing the current scene's viewpoint. 
* `Transform` A const reference to a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing any additional transformations to apply to this batch of objects.

Begins a 2D scene with the specified camera and transformation.


This function starts a new batch for rendering 2D objects using the provided camera and transformation matrix. The camera is used to calculate the view-projection matrix, which is then passed to the graphics pipeline.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) A const reference to the camera object representing the current scene's viewpoint. 
* `Transform` A const reference to a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the transformation of the objects in the scene. 




        

<hr>



### function BeginScene [2/2]

_Begin a 2D scene with the given camera._ 
```C++
static void AGE::Renderer2D::BeginScene (
    const EditorCamera & Camera
) 
```



This function begins a new 2D scene using the provided [**EditorCamera**](class_a_g_e_1_1_editor_camera.md). It calculates the [**World**](class_a_g_e_1_1_world.md) View Projection Matrix (WVPM) based on the camera's projection, view matrix and world matrix. The WVPM is then set as the CameraUniformBuffer data. Finally, it starts a batch for rendering 2D objects.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) The [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) to use for this scene.

Begins a 2D scene with the provided camera.


This function sets up the necessary data for rendering 2D graphics using the given camera. It calculates the [**World**](class_a_g_e_1_1_world.md) View Projection Matrix (WVPM) based on the camera's projection, view matrix and world matrix. The WVPM is then set as a uniform buffer in the graphics pipeline. Finally, it starts a new batch of 2D rendering commands.




**Parameters:**


* [**Camera**](class_a_g_e_1_1_camera.md) A reference to an [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) object representing the camera for the scene.



**Returns:**

void 





        

<hr>



### function DrawCircle 

_Draw a circle on the screen using the provided parameters._ 
```C++
static void AGE::Renderer2D::DrawCircle (
    const Matrix4D & Transform,
    const Vector4 & Color,
    float Thickness=1.f,
    float Fade=.005f,
    int EntityID=-1
) 
```



This function is used to draw a circle on the screen with the given transform, color, thickness, fade and entity ID. The function first checks if there are enough indices in the buffer for another circle. If not, it calls `NextBatch()` to create a new batch. Then, it creates a circle using the provided parameters and increments the index count and circle count stats.




**Parameters:**


* `Transform` The transformation matrix of the circle. 
* `Color` The color of the circle. 
* `Thickness` The thickness of the circle's outline. 
* `Fade` The fade value for the circle. 
* `EntityID` The ID of the entity associated with the circle. 




        

<hr>



### function DrawLine 

_Draw a line in the 3D scene._ 
```C++
static void AGE::Renderer2D::DrawLine (
    const Vector3 & Pos0,
    const Vector3 & Pos1,
    const Vector4 & Color,
    int EntityID=-1
) 
```



This function is used to draw a line segment in the 3D scene with a specified color and positions. The line is drawn between two points, Pos0 and Pos1. The color of the line can be customized by passing a [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the RGBA values. The EntityID parameter allows for identification of which entity (if any) this line corresponds to.




**Parameters:**


* `Pos0` A constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the start point of the line segment. 
* `Pos1` A constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the end point of the line segment. 
* `Color` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the RGBA color values for the line. 
* `EntityID` An integer value that represents the ID of the entity associated with this line (if any).



**Returns:**

void


Draw a line in the 3D scene.


This function is used to draw a line segment in the 3D scene with a specified color and positions. The line will be drawn between two points, Pos0 and Pos1. The color of the line can also be specified using the Color parameter. The EntityID provides an identifier for the entity associated with this line.




**Parameters:**


* `Pos0` The starting position of the line segment. 
* `Pos1` The ending position of the line segment. 
* `Color` The RGBA color of the line segment. 
* `EntityID` An identifier for the entity associated with this line. 




        

<hr>



### function DrawQuad [1/3]

_Draw a quadrilateral with the specified properties._ 
```C++
static void AGE::Renderer2D::DrawQuad (
    const QuadProperties Props
) 
```



This function draws a quadrilateral on the screen using the provided [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object. The quad is drawn in the current graphics pipeline and its vertices are added to the vertex buffer if there's enough space. If not, it calls `NextBatch2D` to start a new batch.




**Parameters:**


* `Props` A structure containing properties of the quadrilateral such as color, size, transformation matrix, texture coordinates, tiling factor and entity ID.

Draw a quadrilateral with the specified properties.


This function draws a quadrilateral on the screen using the provided [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object. It checks if there are enough indices to draw another quad, and if not, it calls RenderCommand::s\_GraphicsPipeline-&gt;NextBatch2D() to start a new batch. Then it creates a quad with the specified properties and increments the index count by 6. Finally, it updates the stats for quads drawn.




**Parameters:**


* `Props` The [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object containing all the information about the quad to be drawn. This includes color, size, transformation matrix, texture coordinates, tiling factor, and entity ID. 




        

<hr>



### function DrawQuad [2/3]

_Draw a quad with the given properties and texture._  _\*_ _\* This function is used to draw a single quad in the 2D graphics pipeline. It takes as input the texture, quad properties (color, size, transform, texture coordinates, tiling factor, entity ID), and it updates the vertex buffer accordingly. If the current batch of quads exceeds the maximum index count, it will start a new batch._ _\*_ _\*._
```C++
static void AGE::Renderer2D::DrawQuad (
    const Ref< Texture2D > & Texture,
    const QuadProperties Props
) 
```




 \*

**Parameters:**


* [**Texture**](class_a_g_e_1_1_texture.md) The reference to the texture that should be used for rendering this quad.
 \*
* `Props` A structure containing all properties necessary for rendering (tint color, size, transform, texture coordinates, tiling factor, entity ID).
 




        

<hr>



### function DrawQuad [3/3]

_Draw a quad using the provided properties and subtexture._ 
```C++
static void AGE::Renderer2D::DrawQuad (
    const Ref< SubTexture2D > & Subtexture,
    const QuadProperties Props
) 
```



This function is used to draw a single quad in 2D space. It takes a reference to a [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md), which contains information about the texture of the quad, as well as a [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) struct that holds various properties related to the quad, such as its color, size, transformation matrix, texture coordinates, tiling factor and entity ID.


The function first checks if there are enough indices in the current batch for another quad. If not, it calls RenderCommand::s\_GraphicsPipeline-&gt;NextBatch2D() to start a new batch. It then retrieves the texture from the subtexture and checks if it is already bound (i.e., its pointer exists within the TextureSlots array).


If the texture is not yet bound, it binds it by incrementing the TextureSlotIndex and adding a new entry to the TextureSlots array. It then creates a quad in the vertex buffer using RenderCommand::s\_GraphicsPipeline-&gt;GetData().VertexBuffers["Quad"]-&gt;CreateQuad(), increments QuadIndexCount by 6 (since each quad is made up of two triangles, thus 6 indices), and increases the QuadCount statistic.




**Parameters:**


* `Subtexture` A reference to a [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object containing information about the texture of the quad. 
* `Props` A struct containing various properties related to the quad, such as its color, size, transformation matrix, texture coordinates, tiling factor and entity ID. 




        

<hr>



### function DrawRect [1/2]

_Draws a 2D rectangle on the screen._ 
```C++
static void AGE::Renderer2D::DrawRect (
    const Vector3 & Position,
    const Vector2 & Size,
    const Vector4 & Color,
    int EntityID=-1
) 
```



This function takes in a position, size and color to draw a rectangle on the screen. The rectangle is defined by four lines - two horizontal and two vertical.




**Parameters:**


* `Position` The center of the rectangle. 
* `Size` The width and height of the rectangle. 
* `Color` The color of the rectangle. 
* `EntityID` An identifier for the entity associated with this rectangle.



**Returns:**

void


Draws a 2D rectangle on the screen.


This function takes in a position, size and color to draw a rectangle on the screen. The rectangle is defined by four lines forming a quadrilateral.




**Parameters:**


* `Position` The center position of the rectangle. 
* `Size` The width and height of the rectangle. 
* `Color` The color of the rectangle. 
* `EntityID` An identifier for the entity associated with this rectangle.



**Returns:**

void 





        

<hr>



### function DrawRect [2/2]

_Draws a 2D rectangle using lines._ 
```C++
static void AGE::Renderer2D::DrawRect (
    const Matrix4D & Transform,
    const Vector4 & Color,
    int EntityID=-1
) 
```



This function takes in a transformation matrix, color and entity ID as parameters to draw a 2D rectangle on the screen. The transformation matrix is used to transform the vertices of the rectangle into world space. The color specifies the color of the rectangle and the entity ID can be used for further processing or identification of the drawn object.




**Parameters:**


* `Transform` A constant reference to a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the transformation matrix. 
* `Color` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object representing the color of the rectangle. 
* `EntityID` An integer representing the entity ID of the drawn object.



**Returns:**

void


Draws a 2D rectangle using lines.


This function takes in a transformation matrix, color and entity ID as parameters to draw a 2D rectangle on the screen. The transformation matrix is used to transform the vertices of the rectangle into their corresponding positions on the screen. The color specifies the color of the rectangle and the entity ID can be used for any purpose such as debugging or identification purposes.




**Parameters:**


* `Transform` A constant reference to a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the transformation matrix. 
* `Color` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object representing the color of the rectangle. 
* `EntityID` An integer representing the entity ID.



**Returns:**

void 





        

<hr>



### function DrawSprite 

_Draws a 2D sprite based on the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _provided._
```C++
static void AGE::Renderer2D::DrawSprite (
    SpriteRendererComponent & SRC
) 
```



The function checks if there is a texture or animation textures in the component and draws accordingly. If neither are present, it draws a quad with no texture.




**Parameters:**


* `SRC` Reference to the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) that contains all necessary information for drawing the sprite.

Draws a 2D sprite based on the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) provided.


The function checks if there is a [**Texture**](class_a_g_e_1_1_texture.md) or SubTexture in the [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md), and then calls the appropriate drawing functions accordingly. If neither are present, it draws a quad with no texture. 


        

<hr>



### function DrawString 

```C++
static void AGE::Renderer2D::DrawString (
    const StringProperties & Props
) 
```




<hr>



### function DrawTile 

_Draws a single tile using the_ [_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _data._ _\*_ _\* This function updates necessary buffers and statistics as needed, based on the details provided by the_[_**SpriteRendererComponent**_](struct_a_g_e_1_1_sprite_renderer_component.md) _._ _\*_ _\*._
```C++
static void AGE::Renderer2D::DrawTile (
    const SpriteRendererComponent & SRC
) 
```




 \*

**Parameters:**


* `SRC` The [**SpriteRendererComponent**](struct_a_g_e_1_1_sprite_renderer_component.md) containing all the information about the tile to be drawn.
 




        

<hr>



### function DrawTileMapLayers 

_Draws a tile map layer using the provided_ [_**TileMapRendererComponent**_](struct_a_g_e_1_1_tile_map_renderer_component.md) _, tmx\_map and vector of tmx\_layer objects._
```C++
static void AGE::Renderer2D::DrawTileMapLayers (
    TileMapRendererComponent & TMRC,
    tmx_map * Map,
    std::vector< tmx_layer * > layers
) 
```



This function prepares buffers for rendering tiles by creating index buffer, vertex array, and vertex buffers. It also sets up their layouts and pushes them into respective vectors in the graphics pipeline data structure. The function then iterates over the layers in reverse order to ensure correct drawing order (back-to-front).




**Parameters:**


* `TMRC` Reference to a [**TileMapRendererComponent**](struct_a_g_e_1_1_tile_map_renderer_component.md) object that holds rendering related information. 
* `Map` Pointer to a tmx\_map object representing the tile map. 
* `layers` Vector of pointers to tmx\_layer objects representing different layers in the tile map.



**Returns:**

void 





        

<hr>



### function EndScene 

_This function is used to end the current scene rendering in a 2D context. It calls the Flush2D method of the currently active GraphicsPipeline object, which should handle any remaining rendering tasks for this frame._ 
```C++
static void AGE::Renderer2D::EndScene () 
```





**Returns:**

void


This function is used to end the current rendering scene. It flushes all pending draw calls in the 2D graphics pipeline.




**Returns:**

void 





        

<hr>



### function Flush 

_This function flushes the 2D rendering pipeline._ 
```C++
static void AGE::Renderer2D::Flush () 
```



The [**RenderCommand**](class_a_g_e_1_1_render_command.md) class' s\_GraphicsPipeline member is accessed and its Flush2D() method is called to flush all pending draw calls in the 2D graphics pipeline.




**Returns:**

void No return value.


This function flushes the 2D graphics pipeline. It ensures all pending draw calls are executed and completed before any new ones can begin.




**Returns:**

void 





        

<hr>



### function GetLineWidth 

_This function returns the current line width._ 
```C++
static float AGE::Renderer2D::GetLineWidth () 
```





**Returns:**

A float representing the current line width.


This function returns the current line width.




**Returns:**

float The current line width as defined in the graphics pipeline data. 





        

<hr>



### function GetStats 

_Get the statistics of the 2D renderer._ 
```C++
static Statistics AGE::Renderer2D::GetStats () 
```



This function retrieves and returns the current statistics of the 2D renderer, including rendering time, draw calls, etc.




**Returns:**

A [**Statistics**](struct_a_g_e_1_1_statistics.md) object containing the current stats of the 2D renderer.


Get the statistics of the 2D renderer.


This function retrieves and returns the current statistics of the 2D renderer, including information about rendering performance such as draw calls, vertices, etc.




**Returns:**

A [**Statistics**](struct_a_g_e_1_1_statistics.md) object containing the current stats of the 2D renderer. 





        

<hr>



### function Init 

_Initializes the_ [_**Renderer2D**_](class_a_g_e_1_1_renderer2_d.md) _object._
```C++
static void AGE::Renderer2D::Init () 
```



This function is used to initialize the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) object, setting it up for rendering operations. It does not take any parameters and returns void.


Initializes the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) object.


This function is used to initialize the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) object, setting it up for rendering operations. It does not take any parameters and returns void. 


        

<hr>



### function SetLineWidth 

_Set the line width for rendering._ 
```C++
static void AGE::Renderer2D::SetLineWidth (
    float Width
) 
```



This function sets the line width used in rendering operations. The actual effect may vary depending on the specific renderer and its configuration.




**Parameters:**


* `Width` The new line width to be set. Must be a positive value.

Set the line width for rendering.


This function sets the line width used in rendering operations. The actual effect may vary depending on the specific renderer and its configuration.




**Parameters:**


* `Width` The new line width to be set. Must be a positive value. 




        

<hr>



### function Shutdown 

_Shuts down the_ [_**Renderer2D**_](class_a_g_e_1_1_renderer2_d.md) _instance._
```C++
static void AGE::Renderer2D::Shutdown () 
```



This function is used to clean up any resources that were allocated during initialization of the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) instance, such as freeing GPU memory or closing open graphics contexts. It also resets all internal state so a new call to Initialize() will start with an empty slate.




**Returns:**

void


Shuts down the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) instance.


This function is used to clean up any resources that were allocated during initialization of the [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md) object, such as freeing GPU memory or closing open graphics contexts. It also resets all internal state so a new call to Initialize() will start with a fresh slate.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Renderer2D.h`

