

# File Serializers.cpp



[**FileList**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Utils**](dir_2ea46939f511f6144e40e8e7d32aa78e.md) **>** [**Private**](dir_1cbb136cab301e6e794b9ffbc12fda9b.md) **>** [**Serializers.cpp**](_serializers_8cpp.md)

[Go to the source code of this file](_serializers_8cpp_source.md)



* `#include "AGEpch.hpp"`
* `#include "Core/Public/App.h"`
* `#include "Utils/Public/Serializers.h"`
* `#include "Scene/Public/Entity.h"`
* `#include "Scene/Public/Components.h"`
* `#include "Controllers/Public/CameraController.h"`
* `#include "Controllers/Public/PlayerController.h"`
* `#include "Controllers/Public/AudioController.h"`
* `#include "Characters/Public/Character.h"`
* `#include "Quests/Public/QuestComponent.h"`
* `#include "Serializers/Public/DataWriter.h"`
* `#include "Serializers/Public/DataReader.h"`
* `#include "Sprite/Public/SpriteAPI.h"`
* `#include "Animation/Public/Animation.h"`
* `#include "Assets/Public/AssetManager.h"`
* `#include <yaml-cpp/yaml.h>`
* `#include "TileMap/Public/TileMapManager.h"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**AGE**](namespace_a_g_e.md) <br> |
| namespace | [**YAML**](namespace_y_a_m_l.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**convert&lt; AGE::AnimationSpecification &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_animation_specification_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; AGE::Ref&lt; AGE::AudioSource &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_ref_3_01_a_g_e_1_1_audio_source_01_4_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; AGE::Ref&lt; AGE::Texture2D &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_ref_3_01_a_g_e_1_1_texture2_d_01_4_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; AGE::Vector2 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector2_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; AGE::Vector3 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector3_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; AGE::Vector4 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector4_01_4.md) &lt;&gt;<br> |
| struct | [**convert&lt; std::vector&lt; std::pair&lt; std::string, std::vector&lt; uint8\_t &gt; &gt; &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01std_1_1vector_3_01std_1_1pair_3_01std_1_1string_00_01std_1_1vector45b2d12052d054c4e49c457374d38f08.md) &lt;&gt;<br> |
| struct | [**convert&lt; std::vector&lt; uint8\_t &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01std_1_1vector_3_01uint8__t_01_4_01_4.md) &lt;&gt;<br> |



















































------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

