

# File KeyEvent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Events**](dir_a6a7e1bcefbf82083808690bf10dad71.md) **>** [**Public**](dir_4b8400f802eae9b048f7995495b525ca.md) **>** [**KeyEvent.h**](_key_event_8h.md)

[Go to the documentation of this file](_key_event_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Event.h"


namespace AGE
{
    class AGE_API KeyEvent : public Event
    {
    public:
        
        inline int GetKeyCode() const { return m_KeyCode; }

        EVENT_CLASS_CATEGORY(EventCategoryKeyboard | EventCategoryInput)
        
    protected:
        
        KeyEvent(int KeyCode)
            : m_KeyCode(KeyCode) {}

        int m_KeyCode;
    };

    class AGE_API KeyPressedEvent : public KeyEvent
    {
    public:
        KeyPressedEvent(int KeyCode, int RepeatCount)
            : KeyEvent(KeyCode), m_RepeatCount(RepeatCount) {}

        inline int GetRepeatCount() const { return m_RepeatCount; }

        std::string ToString() const override
        {
            std::stringstream ss;
            ss << "KeyPressedEvent: " << m_KeyCode << " (" << m_RepeatCount << " repeats)";
            return ss.str();
        }

        EVENT_CLASS_TYPE(KeyPressed)
            
    private:
        int m_RepeatCount;
    };

    class AGE_API KeyReleasedEvent : public KeyEvent
    {
    public:
        KeyReleasedEvent(int KeyCode)
            : KeyEvent(KeyCode) {}

        std::string ToString() const override
        {
            std::stringstream ss;
            ss << "KeyReleasedEvent: " << m_KeyCode;
            return ss.str();
        }

            EVENT_CLASS_TYPE(KeyReleased)
    };

    class AGE_API KeyTypedEvent : public KeyEvent
    {
    public:
        KeyTypedEvent(int KeyCode)
            : KeyEvent(KeyCode) {}

        std::string ToString() const override
        {
            std::stringstream ss;
            ss << "KeyTypedEvent: " << m_KeyCode;
            return ss.str();
        }

        EVENT_CLASS_TYPE(KeyTyped)
    };
}
```


