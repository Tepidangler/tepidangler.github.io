

# File VerticalBoxComponent.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Components**](dir_e8b8bc6c8f57f68d4cd177cc71b48fb4.md) **>** [**Private**](dir_9ab3bcaf0d7053ec28a49e38e0ade647.md) **>** [**VerticalBoxComponent.cpp**](_vertical_box_component_8cpp.md)

[Go to the documentation of this file](_vertical_box_component_8cpp.md)


```C++
//
// Created by gdmgp on 2/1/2026.
//

#include "../Public/VerticalBoxComponent.h"

RTTR_REGISTRATION{
    rttr::registration::class_<AGE::VerticalBoxComponent>("VerticalBoxComponent")
    .constructor<const std::string&>()
    .method("OnUpdate", &AGE::VerticalBoxComponent::OnUpdate);
    //.property("Children", &AGE::VerticalBoxComponent::m_Components)(rttr::metadata("Description", "Child components attached to this box"));
}

namespace AGE
{
    VerticalBoxComponent::VerticalBoxComponent(const std::string &Name) {
        m_Name = Name;
        m_Type = UIComponentType::VerticalBoxComponent;
    }

    void VerticalBoxComponent::OnUpdate(TimeStep DeltaTime)
    {
        UIComponent::OnUpdate(DeltaTime);
    }

    void VerticalBoxComponent::OnEvent(Event &Event) {
    }

    void VerticalBoxComponent::DrawContent() {
    }
} // AGE
```


