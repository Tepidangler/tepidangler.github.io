

# File DataStructures.h



[**FileList**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Structs**](dir_f59ccc9a72ae3438d04a374096905b1a.md) **>** [**Public**](dir_45de20072fa93eb64e7a3a710a6dbdd5.md) **>** [**DataStructures.h**](_data_structures_8h.md)

[Go to the source code of this file](_data_structures_8h_source.md)



* `#include "Core/Public/AGEpch.hpp"`
* `#include "Core/Public/Core.h"`
* `#include "Math/Public/MathStructures.h"`
* `#include "Events/Public/Event.h"`
* `#include <box2d/id.h>`
* `#include <box2d/types.h>`
* `#include <box2d/box2d.h>`
* `#include <glm/glm.hpp>`
* `#include <zlib.h>`
* `#include <xmmintrin.h>`
* `#include <smmintrin.h>`
* `#include <immintrin.h>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**AGE**](namespace_a_g_e.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**AGEPixel**](struct_a_g_e_1_1_a_g_e_pixel.md) <br> |
| struct | [**AGEPoint**](struct_a_g_e_1_1_a_g_e_point.md) <br> |
| struct | [**AGERect**](struct_a_g_e_1_1_a_g_e_rect.md) <br> |
| struct | [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) <br> |
| struct | [**AsepriteCelChunk**](struct_a_g_e_1_1_aseprite_cel_chunk.md) <br> |
| struct | [**AsepriteChunk**](struct_a_g_e_1_1_aseprite_chunk.md) <br> |
| struct | [**AsepriteColorProfileChunk**](struct_a_g_e_1_1_aseprite_color_profile_chunk.md) <br> |
| struct | [**AsepriteExternalFileEntry**](struct_a_g_e_1_1_aseprite_external_file_entry.md) <br> |
| struct | [**AsepriteExternalFilesChunk**](struct_a_g_e_1_1_aseprite_external_files_chunk.md) <br> |
| struct | [**AsepriteFileData**](struct_a_g_e_1_1_aseprite_file_data.md) <br> |
| struct | [**AsepriteFrameData**](struct_a_g_e_1_1_aseprite_frame_data.md) <br> |
| struct | [**AsepriteHeader**](struct_a_g_e_1_1_aseprite_header.md) <br> |
| struct | [**AsepriteLayer**](struct_a_g_e_1_1_aseprite_layer.md) <br> |
| struct | [**AsepriteMaskChunk**](struct_a_g_e_1_1_aseprite_mask_chunk.md) <br> |
| struct | [**AsepriteOldPaletteChunk**](struct_a_g_e_1_1_aseprite_old_palette_chunk.md) <br> |
| struct | [**AsepritePaletteChunk**](struct_a_g_e_1_1_aseprite_palette_chunk.md) <br> |
| struct | [**AsepritePixelData**](struct_a_g_e_1_1_aseprite_pixel_data.md) <br> |
| struct | [**AsepritePropertyData**](struct_a_g_e_1_1_aseprite_property_data.md) <br> |
| struct | [**AsepriteSliceChunk**](struct_a_g_e_1_1_aseprite_slice_chunk.md) <br> |
| struct | [**AsepriteSliceKey**](struct_a_g_e_1_1_aseprite_slice_key.md) <br> |
| struct | [**AsepriteTag**](struct_a_g_e_1_1_aseprite_tag.md) <br> |
| struct | [**AsepriteTagsChunk**](struct_a_g_e_1_1_aseprite_tags_chunk.md) <br> |
| struct | [**AsepriteUserData**](struct_a_g_e_1_1_aseprite_user_data.md) <br> |
| struct | [**AsepriteUserProps**](struct_a_g_e_1_1_aseprite_user_props.md) <br> |
| struct | [**AsepriteVariant**](struct_a_g_e_1_1_aseprite_variant.md) <br> |
| struct | [**Box2DQueryContext**](struct_a_g_e_1_1_box2_d_query_context.md) <br> |
| struct | [**CircleProperties**](struct_a_g_e_1_1_circle_properties.md) <br> |
| struct | [**CircleVertex**](struct_a_g_e_1_1_circle_vertex.md) <br> |
| struct | [**LineProperties**](struct_a_g_e_1_1_line_properties.md) <br> |
| struct | [**LineVertex**](struct_a_g_e_1_1_line_vertex.md) <br> |
| struct | [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) <br> |
| struct | [**QueryParams**](struct_a_g_e_1_1_query_params.md) <br> |
| struct | [**ScreenResolution**](struct_a_g_e_1_1_screen_resolution.md) <br> |
| struct | [**StringProperties**](struct_a_g_e_1_1_string_properties.md) <br> |
| struct | [**TextVertex**](struct_a_g_e_1_1_text_vertex.md) <br> |
| struct | [**TilemapProperties**](struct_a_g_e_1_1_tilemap_properties.md) <br> |
| struct | [**TilemapVertex**](struct_a_g_e_1_1_tilemap_vertex.md) <br> |
| struct | [**UniformBufferObj**](struct_a_g_e_1_1_uniform_buffer_obj.md) <br> |
| struct | [**Vertex**](struct_a_g_e_1_1_vertex.md) <br> |
| struct | [**\_constantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) <br> |
| struct | [**\_constantBufferStruct2D**](struct_a_g_e_1_1__constant_buffer_struct2_d.md) <br> |
| struct | [**\_vertexPositionColor**](struct_a_g_e_1_1__vertex_position_color.md) <br> |
| struct | [**\_vertexPositionColorTangent**](struct_a_g_e_1_1__vertex_position_color_tangent.md) <br> |



















































------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

