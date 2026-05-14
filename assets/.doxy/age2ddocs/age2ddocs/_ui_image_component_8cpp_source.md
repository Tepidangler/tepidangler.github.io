

# File UiImageComponent.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Components**](dir_e8b8bc6c8f57f68d4cd177cc71b48fb4.md) **>** [**Private**](dir_9ab3bcaf0d7053ec28a49e38e0ade647.md) **>** [**UiImageComponent.cpp**](_ui_image_component_8cpp.md)

[Go to the documentation of this file](_ui_image_component_8cpp.md)


```C++
//
// Created by gdmgp on 12/30/2025.
//

#include "../Public/UiImageComponent.h"

#include "Render/Public/Renderer2D.h"

RTTR_REGISTRATION{
    rttr::registration::class_<AGE::UIImageComponent>("ImageComponent")
    .constructor<const std::string&>()
    .method("OnUpdate", &AGE::UIImageComponent::OnUpdate)
    .property("Image", &AGE::UIImageComponent::m_Image)(rttr::metadata("Description", "Properties related to box surrounding the text"));
}
namespace AGE
{
UIImageComponent::UIImageComponent(const std::string &Name)
    {
        m_Name = Name;
        m_Type = UIComponentType::ImageComponent;
        std::unordered_map<UUID, Ref<Texture2D>> TextureMap = AssetManager::Get().GetAssetRegistry()->GetTextures();

        std::for_each(TextureMap.begin(), TextureMap.end(),[&](const std::pair<UUID, Ref<Texture2D>>& pair)
        {
            m_TextureNames.push_back(pair.second->GetName());
        });

        m_Image = Texture2D::Create(TextureSpecification());
    }

void UIImageComponent::OnUpdate(TimeStep DeltaTime)
    {
        Renderer2D::DrawQuad(m_Image, m_Properties);
    }

void UIImageComponent::OnEvent(Event &Event)
    {
    }

    

void UIImageComponent::DrawContent()
    {
        //Combo Box

        //Button with drag and drop ability
        uint32_t TextureID = m_Image->GetTextureID();
        ImGui::ImageButton("##Image", (ImTextureID)&TextureID, ImVec2(32.f,32.f));
        if (ImGui::BeginDragDropTarget())
        {
            if (const ImGuiPayload* Payload = ImGui::AcceptDragDropPayload("CONTENT_BROWSER_ITEM"))
            {
                const wchar_t* Path = (const wchar_t*)Payload->Data;
                std::filesystem::path TexturePath = Path;
                std::string FileName = TexturePath.filename().replace_extension("").string();
                if (AssetManager::Get().IsTextureLoaded(TexturePath))
                {
                    m_Image = AssetManager::Get().GetTexture(FileName);
                }
                else
                {
                    m_Image = AssetManager::Get().LoadTexture(TexturePath);
                }

            }
            ImGui::EndDragDropTarget();
        }

    }
} // AGE
```


