

# File RendererEvent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Events**](dir_a6a7e1bcefbf82083808690bf10dad71.md) **>** [**Public**](dir_4b8400f802eae9b048f7995495b525ca.md) **>** [**RendererEvent.h**](_renderer_event_8h.md)

[Go to the documentation of this file](_renderer_event_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Event.h"
#include "Core/Public/Window.h"
#include "Render/Public/RenderAPI.h"

namespace AGE
{
    class RendererChangeEvent : public Event
    {
    public:
        RendererChangeEvent(AGEWindow* Window)
            : m_Window(Window) {}


        inline AGEWindow* GetWindow() const { return m_Window; }

        std::string ToString() const override
        {
            std::stringstream ss;
            ss << "Renderer Changed: " << Utils::ConvertAPIToString();
            return ss.str();
        }

        EVENT_CLASS_TYPE(RendererChanged)
            EVENT_CLASS_CATEGORY(EventCategoryApplication)
    private:
        AGEWindow* m_Window;
    };

    class RenderUIEvent : public Event
    {
    public:
        RenderUIEvent(TimeStep DeltaTime)
            :m_DeltaTime(DeltaTime){}

        inline TimeStep GetDeltaTime() const { return m_DeltaTime; }
        TimeStep m_DeltaTime;
        EVENT_CLASS_TYPE(RenderUI)
        EVENT_CLASS_CATEGORY(EventCategoryApplication)
    };
}
```


