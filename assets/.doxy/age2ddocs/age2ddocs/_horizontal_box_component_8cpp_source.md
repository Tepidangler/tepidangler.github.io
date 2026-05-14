

# File HorizontalBoxComponent.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Components**](dir_e8b8bc6c8f57f68d4cd177cc71b48fb4.md) **>** [**Private**](dir_9ab3bcaf0d7053ec28a49e38e0ade647.md) **>** [**HorizontalBoxComponent.cpp**](_horizontal_box_component_8cpp.md)

[Go to the documentation of this file](_horizontal_box_component_8cpp.md)


```C++
//
// Created by gdmgp on 2/1/2026.
//

#include "../Public/HorizontalBoxComponent.h"
RTTR_REGISTRATION{
    rttr::registration::class_<AGE::HorizontalBoxComponent>("HorizontalBoxComponent")
    .constructor<const std::string&>()
    .method("OnUpdate", &AGE::HorizontalBoxComponent::OnUpdate);
    //.property("Children", &AGE::HorizontalBoxComponent::m_Components)(rttr::metadata("Description", "Child components attached to this box"));
}
namespace AGE
{
HorizontalBoxComponent::HorizontalBoxComponent(const std::string &Name)
    {
        m_Name = Name;
        m_Type = UIComponentType::HorizontalBoxComponent;
    }

void HorizontalBoxComponent::OnUpdate(TimeStep DeltaTime)
    {
        UIComponent::OnUpdate(DeltaTime);
    }

void HorizontalBoxComponent::OnEvent(Event &Event) {
    }

void HorizontalBoxComponent::DrawContent() {
    }
} // AGE
```


