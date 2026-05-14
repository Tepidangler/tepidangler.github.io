

# File Layer.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Layer.h**](_layer_8h.md)

[Go to the documentation of this file](_layer_8h.md)


```C++
#pragma once

#include "Core.h"
#include "Events/Public/Event.h"
#include "Core/Public/DeltaTime.h"



namespace AGE
{
    

class AGE_API Layer
    {
    public:

        Layer(const std::string& name = "Layer");

        virtual ~Layer();

        virtual void Init() {};

virtual void OnAttach() {}
        
virtual void OnDetach() {}
        
virtual void OnUpdate(TimeStep DeltaTime) {} 

virtual void OnImGuiRender(TimeStep DeltaTime) {}
        
virtual void OnEvent(Event& Event) {}

        float GetTime();

inline const std::string& GetName() const { return m_DebugName; }

    protected:
        std::string m_DebugName;
    };
}
```


