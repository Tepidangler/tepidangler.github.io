

# File ImGuiLayer.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**ImGui**](dir_195ca6e0ece592faf3368ed4c1417872.md) **>** [**Public**](dir_d4dd9819148636cc4517517cf4fc8cc8.md) **>** [**ImGuiLayer.h**](_im_gui_layer_8h.md)

[Go to the documentation of this file](_im_gui_layer_8h.md)


```C++
#pragma once

#include "Core/Public/Layer.h"
#include "Core/Public/LayerStack.h"
#include "Events/Public/KeyEvent.h"
#include "Events/Public/MouseEvent.h"
#include "Events/Public/ApplicationEvent.h"
#include "Events/Public/RendererEvent.h"
#include "Render/Public/GraphicsContext.h"
#include "Render/Public/Renderer.h"



namespace AGE
{
    
class AGE_API ImGuiLayer : public Layer
    {
    
    public:

        ImGuiLayer();

        ~ImGuiLayer();

        virtual void OnAttach() override;
                          
        virtual void OnDetach() override;
        virtual void OnImGuiRender(TimeStep DeltaTime) override;


        virtual void Begin();

        virtual void OnEvent(Event& E) override;

inline void BlockEvents(bool block) { m_BlockEvents = block; }

        virtual void End();

    private:
        void SetDarkThemeColors();

        bool OnWindowResized(WindowResizeEvent& E);

        bool m_BlockEvents = true;

        LayerStack m_LayerStack;

        GraphicsContext* m_Context;

        RendererAPI::API m_CurrentGraphicsAPI;
    };


}
```


