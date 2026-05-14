

# File ScriptableComponentStack.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**ScriptableComponentStack.cpp**](_scriptable_component_stack_8cpp.md)

[Go to the documentation of this file](_scriptable_component_stack_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Core/Public/ScriptableComponentStack.h"


namespace GameFramework
{
ScriptableCompStack::ScriptableCompStack()
    {
    }
ScriptableCompStack::~ScriptableCompStack()
    {
        for (AGE::ScriptableEntity* E : m_Entitys)
        {
            E->~ScriptableEntity();
        }
    }
void ScriptableCompStack::PushComponent(AGE::ScriptableEntity* Entt)
    {
        m_Entitys.emplace(m_Entitys.begin() + m_EntityInsertIndex, Entt);
        m_EntityInsertIndex++;
    }
void ScriptableCompStack::PopComponent(AGE::ScriptableEntity* Entt)
    {
        auto it = std::find(m_Entitys.begin(), m_Entitys.end(), Entt);

        if (it != m_Entitys.end())
        {
            m_Entitys.erase(it);
            m_EntityInsertIndex--;
        }
    }
}
```


