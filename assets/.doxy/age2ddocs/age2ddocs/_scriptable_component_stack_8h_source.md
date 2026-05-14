

# File ScriptableComponentStack.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**ScriptableComponentStack.h**](_scriptable_component_stack_8h.md)

[Go to the documentation of this file](_scriptable_component_stack_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Scene/Public/ScriptableEntity.h"

namespace GameFramework
{
    class ScriptableCompStack
    {
    public:
        ScriptableCompStack();
        ~ScriptableCompStack();

        void PushComponent(AGE::ScriptableEntity* Entt);


        void PopComponent(AGE::ScriptableEntity* Entt);



std::vector<AGE::ScriptableEntity*>::iterator begin() { return m_Entitys.begin(); }

std::vector<AGE::ScriptableEntity*>::iterator end() { return m_Entitys.end(); }

std::vector<AGE::ScriptableEntity*>::const_iterator begin() const { return m_Entitys.cbegin(); }

std::vector<AGE::ScriptableEntity*>::const_iterator end() const { return m_Entitys.cend(); }

    private:
        std::vector<AGE::ScriptableEntity*> m_Entitys;
        unsigned int m_EntityInsertIndex = 0;
    };
}
```


