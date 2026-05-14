

# File AudioEngine.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Audio**](dir_db6938f1ff25f5ebd4fcc50cd8804f79.md) **>** [**AudioEngine**](dir_bf6a2ae4f421b3e627c8671719c9dbdd.md) **>** [**Private**](dir_933cf9cfa8f6f567c0c937ed7947c49a.md) **>** [**AudioEngine.cpp**](_audio_engine_8cpp.md)

[Go to the documentation of this file](_audio_engine_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Audio/AudioEngine/Public/AudioEngine.h"
#include "Audio/AGESound/Public/AGEAudio.h"
#include "Audio/Fmod/Public/FmodEngine.h"
#include "Audio/Wwise/Public/WWiseEngine.h"
#include "Core/Public/Log.h"

namespace AGE
{
    

Ref<AudioEngine> AudioEngine::Create(AudioEngineType Type)
    {

        switch (Type)
        {
        case 0:
        {
            return CreateRef<AGESound>();
        }

        case 1:
        {
#if WITH_WWISE
            return CreateRef<Wwise>();
#else
            CoreLogger::Assert(false, "AGE was not built with WWise! Check the value of your CMake variables and make sure BUILD_WITH_WWISE is ON and you have set a path for the SDK in WWISE_INSTALL_PATH");
            return nullptr;
#endif
        }

        case 2:
        {
#if WITH_FMOD
            return CreateRef<FmodEngine>();
#else
            CoreLogger::Assert(false, "AGE was not built with FMod! Check the value of your CMake variables and make sure BUILD_WITH_FMOD is ON and you have set a path for the SDK in FMOD_INSTALL_PATH");
            return nullptr;
#endif
        }

        }

        return CreateRef<AGESound>();

    }

    template<typename T>
T* AudioEngine::As()
    {
        CoreLogger::Assert(false, "As() Failed");
    }




}

```


