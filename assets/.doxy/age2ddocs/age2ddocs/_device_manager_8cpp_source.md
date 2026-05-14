

# File DeviceManager.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**DeviceManager.cpp**](_device_manager_8cpp.md)

[Go to the documentation of this file](_device_manager_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "DeviceManager.h"
#include "Render/Public/Renderer.h"

namespace AGE
{
DeviceManager::DeviceManager(AudioEngineType AudioEngine, bool UseXInput)
    {
        m_Window = Scope<AGEWindow>(AGEWindow::Create());
        m_AudioManager = CreateScope<AudioManager>(AudioEngine);
#ifdef AG_PLATFORM_WINDOWS
        if (UseXInput)
        {
            m_XInput = CreateScope<XInput>();
        }
        m_XInput = nullptr;
#endif
        CoreLogger::Info("Device Manager Initialized!");
    }
    //AUDIO MANAGER

AudioManager::AudioManager(AudioEngineType Type)
        :m_Type(Type)
    {
        m_AudioEngine = Ref<AudioEngine>(AudioEngine::Create(Type));
        CoreLogger::Info("Audio Manager Initialized!");
    }

void AudioManager::SwitchAudioEngine(AudioEngineType Type)
    {
        m_AudioEngine.reset();
        m_AudioEngine = Ref<AudioEngine>(AudioEngine::Create(Type));
        m_Type = Type;
    }
}

```


