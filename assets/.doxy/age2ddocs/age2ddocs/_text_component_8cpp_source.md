

# File TextComponent.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Components**](dir_e8b8bc6c8f57f68d4cd177cc71b48fb4.md) **>** [**Private**](dir_9ab3bcaf0d7053ec28a49e38e0ade647.md) **>** [**TextComponent.cpp**](_text_component_8cpp.md)

[Go to the documentation of this file](_text_component_8cpp.md)


```C++
//
// Created by gdmgp on 12/5/2025.
//

#include "AGEpch.hpp"
#include "UI/Components/Public/TextComponent.h"
#include "Render/Public/Renderer2D.h"
#include "Core/Public/Log.h"
#include <rttr/registration>
#include <misc/cpp/imgui_stdlib.h>


namespace AGE
{
    TextComponent::TextComponent(const std::string& Name)
    {
        m_Name = Name;
        m_Type = UIComponentType::TextComponent;
        m_StringProperties.TextFont = AGEFont::GetDefault();
    }
    void TextComponent::OnUpdate(TimeStep DeltaTime)
    {
        if (m_CompProperties.Visible)
        {
            Renderer2D::DrawString(m_StringProperties);
        }
    }

    void TextComponent::OnEvent(Event &Event)
    {
    }

    void TextComponent::DrawFontSelectionComboBox()
    {
        std::unordered_map<UUID,Ref<AGEFont>> Fonts = AssetManager::Get().GetAssetRegistry()->GetFonts();
        std::vector<std::string> FontNames = AssetManager::Get().GetAssetRegistry()->GetFontNames();

        if (m_StringProperties.FontName.empty())
        {
            m_StringProperties.FontName = AGEFont::GetDefault()->GetFontName();
        }
        ImGui::Text("Fonts"); ImGui::SameLine();
        if (ImGui::BeginCombo("##Fonts",m_StringProperties.FontName.c_str()))
        {
            for (auto& F : FontNames)
            {
                bool IsSelected = F == m_StringProperties.FontName;
                if (ImGui::Selectable(F.c_str(), IsSelected))
                {
                    m_StringProperties.FontName = F;
                }

                if (IsSelected)
                {
                    ImGui::SetItemDefaultFocus();
                }

            }
            ImGui::EndCombo();
        }

    }

    void TextComponent::DrawContent()
    {
        ImGui::Text("String Properties");
        ImGui::Text("Text");ImGui::SameLine();
        ImGui::InputText("##Text", &m_StringProperties.Text);
        DrawFontSelectionComboBox();
        if (m_StringProperties.TextFont->GetAtlasTexture()->GetName() != m_StringProperties.FontName)
        {
            m_StringProperties.TextFont = AssetManager::Get().GetFont(m_StringProperties.FontName);
        }
        ImGui::InputDouble("Font Size", &m_StringProperties.FontSize, 1.0, 4.0);
        ImGui::ColorEdit4("Text Color", &m_StringProperties.Color.x);
        DrawVec3Control("Position", m_StringProperties.Position);
        DrawVec3Control("Rotation", m_StringProperties.Rotation);
    }

    template<>
    TextComponent* UIComponent::As()
    {
        return (TextComponent*)this;
    }
} // AGE

RTTR_REGISTRATION
{
    rttr::registration::class_<AGE::TextComponent>("TextComponent")
    .constructor<const std::string&>()
    .method("OnUpdate", &AGE::TextComponent::OnUpdate)
    .property("Name", &AGE::TextComponent::m_Name);
}
```


