

# File MouseEvent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Events**](dir_a6a7e1bcefbf82083808690bf10dad71.md) **>** [**Public**](dir_4b8400f802eae9b048f7995495b525ca.md) **>** [**MouseEvent.h**](_mouse_event_8h.md)

[Go to the documentation of this file](_mouse_event_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Event.h"


namespace AGE
{
    
class AGE_API MouseEvent : public Event
    {
    public:
        inline int GetMouseButton() const { return m_Button; }
        
        EVENT_CLASS_CATEGORY(EventCategoryMouse | EventCategoryInput)

    protected:
        MouseEvent(int Button)
            : m_Button(Button) {}

MouseEvent(float x, float y)
            : m_MouseX(x), m_MouseY(y) {}

MouseEvent(float xOffset, float yOffset, bool Scrolled) // I can probably figure out a better way to do this, but it'll work for now since I won't ever actually be using the boolean
            : m_XOffset(xOffset), m_YOffset(yOffset) {}

    protected:

        int m_Button;

        float m_MouseX;
        float m_MouseY;

        float m_XOffset;
        float m_YOffset;
    };

    class AGE_API MouseMovedEvent : public MouseEvent
    {
    public:
        
        MouseMovedEvent(float x, float y)
            : MouseEvent(x,y) {}

inline float GetX() const { return m_MouseX; }
inline float GetY() const { return m_MouseY; }

std::string ToString() const override
        {
            std::stringstream ss;
            ss << "MouseMovedEvent: " << m_MouseX << ", " << m_MouseY;
            return ss.str();
        }

        EVENT_CLASS_TYPE(MouseMoved)
    };

    class AGE_API MouseScrolledEvent : public MouseEvent
    {
    public:
        
        MouseScrolledEvent(float xOffset, float yOffset)
            : MouseEvent(xOffset, yOffset, true) {}

inline float GetXOffset() const { return m_XOffset; }
inline float GetYOffset() const { return m_YOffset; }

std::string ToString() const override
        {
            std::stringstream ss;
            ss << "MouseScrolledEvent: " << GetXOffset() << ", " << GetYOffset();
            return ss.str();
        }

        EVENT_CLASS_TYPE(MouseScrolled)
    };

    class AGE_API MouseButtonPressedEvent : public MouseEvent
    {
    public:

        MouseButtonPressedEvent(int Button)
            : MouseEvent(Button) {}

std::string ToString() const override
        {
            std::stringstream ss;
            ss << "MouseButtonPressedEvent: " << m_Button;
            return ss.str();
        }

        EVENT_CLASS_TYPE(MouseButtonPressed)
    };

class AGE_API MouseButtonReleasedEvent : public MouseEvent
    {
    public:

        MouseButtonReleasedEvent(int Button)
            : MouseEvent(Button) {}

std::string ToString() const override
        {
            std::stringstream ss;
            ss << "MouseButtonReleasedEvent: " << m_Button;
            return ss.str();
        }

        EVENT_CLASS_TYPE(MouseButtonReleased)
    };
}
```


