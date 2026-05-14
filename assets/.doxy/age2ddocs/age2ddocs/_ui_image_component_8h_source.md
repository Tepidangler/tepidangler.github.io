

# File UiImageComponent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Components**](dir_e8b8bc6c8f57f68d4cd177cc71b48fb4.md) **>** [**Public**](dir_5c113c7ed6e7034142773ced1bfb6a62.md) **>** [**UiImageComponent.h**](_ui_image_component_8h.md)

[Go to the documentation of this file](_ui_image_component_8h.md)


```C++
//
// Created by gdmgp on 12/30/2025.
//

#ifndef AGE2D_UIIMAGECOMPONENT_H
#define AGE2D_UIIMAGECOMPONENT_H
#pragma once
#include "UI/Public/UiComponent.h"
#include "Texture/Public/Texture.h"

namespace AGE
{
    class UIImageComponent : public UIComponent
    {
    public:

        UIImageComponent(const std::string& Name);

virtual ~UIImageComponent() = default;

void CallSerialize(DataWriter* Serializer) override
        {
        }
void CallDeserialize(DataReader* Serializer) override
        {
        }

        void OnUpdate(TimeStep DeltaTime) override;
        void OnEvent(Event& Event) override;
        void DrawContent() override;

        Ref<Texture2D> m_Image;
        std::string m_CurrentTexture;
        std::vector<std::string> m_TextureNames;
        QuadProperties m_Properties{};

        RTTR_ENABLE(UIComponent)
        RTTR_REGISTRATION_FRIEND
    };
} // AGE

#endif //AGE2D_UIIMAGECOMPONENT_H
```


