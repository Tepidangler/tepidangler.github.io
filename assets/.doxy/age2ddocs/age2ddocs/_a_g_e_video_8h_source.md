

# File AGEVideo.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Video**](dir_578bc13a0cdd58dd59c0b94f1f46155f.md) **>** [**Public**](dir_b2379784e2c191aed75bb712ef5fa396.md) **>** [**AGEVideo.h**](_a_g_e_video_8h.md)

[Go to the documentation of this file](_a_g_e_video_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Render/Public/FrameBuffer.h"
#include "Core/Public/DeltaTime.h"
#include "Camera/Public/EditorCamera.h"
#if 0

namespace AGE
{
    typedef void IGRenderCallback(TimeStep DeltaTime);

    class VideoSource;

    class AGEVideo
    {
    public:
        static void Init();
        static void Shutdown();

        static VideoSource LoadVideoSource(const std::string& FileName);
        static void Play(const Ref<VideoSource>& Source, EditorCamera& Camera);
        static void Stop(const Ref<VideoSource>& Source);
        static void Stop(const std::vector<Ref<VideoSource>>& Sources);

    private:
        static void PlayVideo(const Ref<VideoSource>& Source);
        static void PlayVideoOpenGL(const Ref<VideoSource>& Source, EditorCamera& Camera);
        static void PlayVideoDX(const Ref<VideoSource>& Source);



    };



}
#endif
```


