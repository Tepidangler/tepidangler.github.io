

# File AudioEngine.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Audio**](dir_db6938f1ff25f5ebd4fcc50cd8804f79.md) **>** [**AudioEngine**](dir_bf6a2ae4f421b3e627c8671719c9dbdd.md) **>** [**Public**](dir_ea32d5a6b44ca038dc6c67f0bb71548f.md) **>** [**AudioEngine.h**](_audio_engine_8h.md)

[Go to the documentation of this file](_audio_engine_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Audio/AudioEngine/Public/Soundbank.h"
#include <memory>

namespace AGE
{
    enum AudioEngineType : uint16_t
    {
        AGESoundEngine = 0,
        WWiseEngine,
        FModEngine
    };

    class AudioEngine
    {
    public:

        template<typename T>
        T* As();

        virtual ~AudioEngine() = default;
        static Ref<AudioEngine> Create(AudioEngineType Type);

        virtual void Init() = 0;
        virtual void Start() = 0;
        virtual void Update() = 0;
        virtual void Stop() = 0;
        virtual void Shutdown() = 0;

        virtual void LoadBanks(const std::vector<Ref<SoundBank>>& Banks) = 0;
        virtual void LoadBank(Ref<SoundBank> Bank) = 0;

        virtual std::string& GetCurrentEventName() = 0;
        virtual void SetCurrentEventName(const std::string& Name) = 0;

        virtual bool IsEventValid(const std::string& EventName) = 0;

        virtual void SetParameterByName(const std::string& Name, float Value) = 0;
        virtual void Set3DAttributes(void* Attributes) =0;


        virtual void LoadEvents() = 0;


    private:

    };
}
```


