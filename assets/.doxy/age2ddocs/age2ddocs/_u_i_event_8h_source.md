

# File UIEvent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Events**](dir_a6a7e1bcefbf82083808690bf10dad71.md) **>** [**Public**](dir_4b8400f802eae9b048f7995495b525ca.md) **>** [**UIEvent.h**](_u_i_event_8h.md)

[Go to the documentation of this file](_u_i_event_8h.md)


```C++
//
// Created by gdmgp on 12/30/2025.
//

#ifndef AGE2D_UIEVENT_H
#define AGE2D_UIEVENT_H
#include "Events/Public/Event.h"

namespace AGE
{
    class WidgetConstructedEvent : public Event
    {
    public:
        WidgetConstructedEvent(const Ref<ScriptableWidget> UIWidget, uint8_t Stack)
            :m_Stack(Stack), m_ScriptableWidget(UIWidget) {}

        uint8_t GetStack() const { return m_Stack; }
        Ref<ScriptableWidget> GetWidget() const { return m_ScriptableWidget; }

        EVENT_CLASS_TYPE(WidgetConstructed)
        EVENT_CLASS_CATEGORY(EventCategoryUI)
    private:
        uint8_t m_Stack;
        Ref<ScriptableWidget> m_ScriptableWidget;
    };

    class WidgetActivatedEvent : public Event
    {
    public:
        WidgetActivatedEvent(const Ref<ScriptableWidget> UIWidget, uint8_t Stack)
            :m_Stack(Stack), m_ScriptableWidget(UIWidget) {}

        uint8_t GetStack() const { return m_Stack; }
        Ref<ScriptableWidget> GetWidget() const { return m_ScriptableWidget; }

        EVENT_CLASS_TYPE(WidgetActivated)
        EVENT_CLASS_CATEGORY(EventCategoryUI)
    private:
        uint8_t m_Stack;
        Ref<ScriptableWidget> m_ScriptableWidget;
    };

    class WidgetDeactivatedEvent : public Event
    {
    public:
        WidgetDeactivatedEvent(const Ref<ScriptableWidget> UIWidget, uint8_t Stack)
            :m_Stack(Stack), m_ScriptableWidget(UIWidget) {}

        uint8_t GetStack() const { return m_Stack; }
        Ref<ScriptableWidget> GetWidget() const { return m_ScriptableWidget; }

        EVENT_CLASS_TYPE(WidgetDeactivated)
        EVENT_CLASS_CATEGORY(EventCategoryUI)
    private:
        uint8_t m_Stack;
        Ref<ScriptableWidget> m_ScriptableWidget;
    };

}
#endif //AGE2D_UIEVENT_H
```


