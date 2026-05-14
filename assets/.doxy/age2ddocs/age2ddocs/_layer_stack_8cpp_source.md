

# File LayerStack.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**LayerStack.cpp**](_layer_stack_8cpp.md)

[Go to the documentation of this file](_layer_stack_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "LayerStack.h"

namespace AGE
{
LayerStack::LayerStack()
    {
    }

LayerStack::~LayerStack()
    {
        for (Layer* L : m_Layers)
        {
            delete L;
        }
    
    }


void LayerStack::PushLayer(Layer* Layer)
    {
        m_Layers.emplace(m_Layers.begin() + m_LayerInsertIndex, Layer);
        m_LayerInsertIndex++;
    }
void LayerStack::PushOverlay(Layer* Overlay)
    {
        m_Layers.emplace_back(Overlay);
    }
void LayerStack::PopLayer(Layer* Layer)
    {
        Layer->OnDetach();
        auto it = std::find(m_Layers.begin(), m_Layers.end(), Layer);

        if (it != m_Layers.end())
        {

            m_Layers.erase(it);
            m_LayerInsertIndex--;
        }
    }
void LayerStack::PopOverlay(Layer* Overlay)
    {
        auto it = std::find(m_Layers.begin(), m_Layers.end(), Overlay);
        
        if (it != m_Layers.end())
        {
            m_Layers.erase(it);
        }
    }

Layer * LayerStack::GetLayerByName(const std::string &LayerName)
    {
        auto it = std::find_if(m_Layers.begin(), m_Layers.end(), [LayerName](const Layer* Layer)
        {
            return Layer->GetName() == LayerName;
        });

        if (it != m_Layers.end())
        {
            return *it;
        }

        // TODO: Add something to let users know what happened
        return nullptr;
    }
}

```


