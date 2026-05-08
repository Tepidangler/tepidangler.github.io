

# File LayerStack.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**LayerStack.h**](_layer_stack_8h.md)

[Go to the documentation of this file](_layer_stack_8h.md)


```C++
#pragma once
#include "Core.h"
#include "Layer.h"

#include <vector>

namespace AGE
{
    class AGE_API LayerStack
    {
    public:
        LayerStack();
        ~LayerStack();

        void PushLayer(Layer* Layer);

        void PushOverlay(Layer* Overlay);

        void PopLayer(Layer* Layer);

        void PopOverlay(Layer* Overlay);

        Layer* GetLayerByName(const std::string& LayerName);


        std::vector<Layer*>::iterator begin() { return m_Layers.begin(); }

        std::vector<Layer*>::iterator end() { return m_Layers.end(); }

        std::vector<Layer*>::const_iterator begin() const { return m_Layers.cbegin(); }

        std::vector<Layer*>::const_iterator end() const { return m_Layers.cend(); }

    private:
        std::vector<Layer*> m_Layers;
        unsigned int m_LayerInsertIndex  = 0;
    };
}
```


