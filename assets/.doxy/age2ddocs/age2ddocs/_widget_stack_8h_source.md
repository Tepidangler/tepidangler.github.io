

# File WidgetStack.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Public**](dir_22621ac137e3b40d7111b7a349592295.md) **>** [**WidgetStack.h**](_widget_stack_8h.md)

[Go to the documentation of this file](_widget_stack_8h.md)


```C++
//
// Created by gdmgp on 12/3/2025.
//

#pragma once
#ifndef AGE2D_WIDGETSTACK_H
#define AGE2D_WIDGETSTACK_H
#include "UI/Public/ScriptableWidget.h"
#include "Core/Public/Core.h"
#include "Core/Public/DeltaTime.h"

namespace AGE
{
    class WidgetStack
    {
    public:
WidgetStack() = default;
~WidgetStack() = default;

        void PushWidgetToStack(Ref<ScriptableWidget> Widget);
        void PopWidgetFromStack();

Ref<ScriptableWidget> GetActiveWidget() {return m_Widgets.front();}

        void OnTopUpdate(TimeStep DeltaTime);

        void ActivateWidget();
        void DeactivateWidget();

std::deque<Ref<ScriptableWidget>>::iterator begin() {return m_Widgets.begin();}
std::deque<Ref<ScriptableWidget>>::iterator end() {return m_Widgets.end();}
std::deque<Ref<ScriptableWidget>>::const_iterator begin() const {return m_Widgets.cbegin();}
std::deque<Ref<ScriptableWidget>>::const_iterator end() const {return m_Widgets.cend();}


    private:
        std::deque<Ref<ScriptableWidget>> m_Widgets;
        Entity m_Entity;
    };
} // AGE

#endif //AGE2D_WIDGETSTACK_H
```


