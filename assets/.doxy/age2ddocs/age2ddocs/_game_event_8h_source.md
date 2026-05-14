

# File GameEvent.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Events**](dir_a6a7e1bcefbf82083808690bf10dad71.md) **>** [**Public**](dir_4b8400f802eae9b048f7995495b525ca.md) **>** [**GameEvent.h**](_game_event_8h.md)

[Go to the documentation of this file](_game_event_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Event.h"

#include "Scene/Public/Scene.h"

namespace AGE
{

    class InputEvent : public Event
    {
inline int GetGamepadButton() { return m_Button; }

        EVENT_CLASS_CATEGORY(EventCategoryInput | EventCategoryGame)

    protected:
        InputEvent();
InputEvent(int Axis, float Position)
            :m_Axis(Axis), m_Position(Position) {}
InputEvent(int Button)
            : m_Button(Button) {}

    protected:
        int m_Axis;
        float m_Position;
        int m_Button;
    };

    class AxisEvent : public InputEvent
    {
    public:
AxisEvent(int Axis, float Position)
            : InputEvent(Axis, Position) {}

inline int GetAxis() { return m_Axis; }
inline float GetPosition() { return m_Position; }
        EVENT_CLASS_TYPE(AxisMoved)
    };

    class GamepadButtonPressedEvent : public InputEvent
    {
    public:
GamepadButtonPressedEvent(int Button)
            :InputEvent(Button) {}

inline int GetButton() { return m_Button; }
        EVENT_CLASS_TYPE(GamepadButtonPressed)
    };

    class GamepadButtonReleasedEvent : public InputEvent
    {
    public:
GamepadButtonReleasedEvent(int Button)
            :InputEvent(Button) {}

inline int GetButton() { return m_Button; }
        EVENT_CLASS_TYPE(GamepadButtonReleased)
    };

    class SceneEvent : public Event
    {
        EVENT_CLASS_CATEGORY(EventCategoryGame)
        protected:
SceneEvent(Ref<Scene> Scene)
            :m_Scene(Scene) {}

    protected:
        Ref<Scene> m_Scene;
    };

    class SceneChangedEvent : public SceneEvent
    {
        public:
SceneChangedEvent(Ref<Scene> Scene)
            :SceneEvent(Scene){}

inline Ref<Scene> GetScene() {return m_Scene;}
        EVENT_CLASS_TYPE(SceneChanged)
    };
}
```


