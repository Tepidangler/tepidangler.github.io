

# File WindowsWindow.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**Windows**](dir_29cf55498d836108c28434a30f1caa57.md) **>** [**Public**](dir_791287e181c442a825a539b1df7902c0.md) **>** [**WindowsWindow.h**](_windows_window_8h.md)

[Go to the documentation of this file](_windows_window_8h.md)


```C++

#ifdef AG_PLATFORM_WINDOWS
#pragma once
#include "Core/Public/Window.h"
#include "Render/Public/GraphicsContext.h"
#include <GLFW/glfw3.h>
#define GLFW_EXPOSE_NATIVE_WIN32
#include <GLFW/glfw3native.h>

typedef uint16_t JoyStickID;
namespace AGE
{
    class WindowsWindow : public AGEWindow
    {
    public:

        WindowsWindow(const WindowProps& Props);
        virtual ~WindowsWindow();

        void OnUpdate() override;

        inline unsigned int GetWidth() const override { return m_Data.Width; }
        inline unsigned int GetHeight() const override { return m_Data.Height; }

        // Window Attributes

        inline void SetEventCallback(const EventCallbackFn& Callback) override 
        {
            m_Data.EventCallback = Callback; 
            m_RendererCallback = Callback;

            for (auto& D : m_JDatas)
            {
                D.EventCallback = Callback;
            }

        }
        void SetVSync(bool Enabled) override;
        bool IsVSync() const override;
        void ProcessJoystickInput();

        static WindowsWindow& Get() { return *s_Window; }
        void* GetNativeWindow() const override { return m_Window; }
        HWND GetPlatformWindow() override { return m_Win32Window; }
        Vector2 GetMousePos() override;

        GraphicsContext* GetGraphicsContext() override { return m_Context.get(); }

        static void JoystickCallback(int JID, int Event);

        void SwitchRenderer() override;

        void RebuildWindow() override;

        void SetWindowIcon(const std::filesystem::path& Path) override;

    private:
        virtual void Init(const WindowProps& Props);
        virtual void Shutdown();

    private:

        GLFWwindow* m_Window;
        HWND m_Win32Window;
        [[maybe_unused]] GLFWgamepadstate m_PadState;

        struct WindowData
        {
            std::string Title;
            unsigned int Width, Height;
            bool VSync;
            const char* String;

            EventCallbackFn EventCallback;
        };

        struct JoystickData
        {
            std::string Name;

            EventCallbackFn EventCallback;
        };

        EventCallbackFn m_RendererCallback;

        WindowData m_Data;

        std::array<JoystickData, 15> m_JDatas;

        static WindowsWindow* s_Window;

        Scope<GraphicsContext> m_Context;

        GLFWimage m_Images[1];
        
    };
}
#endif
```


