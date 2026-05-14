

# File WidgetStack.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Private**](dir_1203d8b56ae061d1573ea9addf7cd415.md) **>** [**WidgetStack.cpp**](_widget_stack_8cpp.md)

[Go to the documentation of this file](_widget_stack_8cpp.md)


```C++
//
// Created by gdmgp on 12/3/2025.
//

//#include "AGEpch.hpp"
#include "../Public/WidgetStack.h"


namespace AGE
{
void WidgetStack::PushWidgetToStack(Ref<ScriptableWidget> Widget)
    {
        m_Widgets.emplace_front(Widget);
    }

void WidgetStack::PopWidgetFromStack()
    {
        m_Widgets.pop_front();
    }

void WidgetStack::OnTopUpdate(TimeStep DeltaTime)
    {
        if (m_Widgets.size() > 0)
        {
            m_Widgets.front()->OnUpdate(DeltaTime);
        }
    }

void WidgetStack::ActivateWidget() {
        m_Widgets.front()->SetVisibility(true);
    }

void WidgetStack::DeactivateWidget() {
        m_Widgets.front()->SetVisibility(false);
    }
} // AGE
```


