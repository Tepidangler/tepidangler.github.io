

# File AGEVideo.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Video**](dir_578bc13a0cdd58dd59c0b94f1f46155f.md) **>** [**Private**](dir_e8b69b5737a5bdbffd9e44518451477a.md) **>** [**AGEVideo.cpp**](_a_g_e_video_8cpp.md)

[Go to the documentation of this file](_a_g_e_video_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Video/Public/AGEVideo.h"
#include "Video/Public/VideoSource.h"
#include "Render/Public/Renderer2D.h"
#include "Render/Public/RenderCommand.h"
#if 0

namespace AGE
{
    void AGEVideo::Init()
    {
        CoreLogger::Info("Starting AGE Video Player!");
    }
    void AGEVideo::Shutdown()
    {
    }
    VideoSource AGEVideo::LoadVideoSource(const std::string& FileName)
    {
        return VideoSource(FileName);
    }

    void AGEVideo::Play(const Ref<VideoSource>& Source, EditorCamera& Camera)
    {
        switch ((int)RendererAPI::GetAPI())
        {
        case 0:
        {
            AGE_CORE_ASSERT(false, "Headless is currently unsupported!");
            break;
        }
        case 1:
        {
            break;
        }
        case 2:
        case 3:
        {
            break;
        }
        default:
        {
        }
        }
    }
    void AGEVideo::Stop(const Ref<VideoSource>& Source)
    {
    }
    void AGEVideo::Stop(const std::vector<Ref<VideoSource>>& Sources)
    {
    }

    void AGEVideo::PlayVideo(const Ref<VideoSource>& Source)
    {

    }

    void AGEVideo::PlayVideoOpenGL(const Ref<VideoSource>& Source, EditorCamera& Camera)
    {
        AGE_CORE_ASSERT(false, "OpenGL Not Implemented!");
    }
    void AGEVideo::PlayVideoDX(const Ref<VideoSource>& Source)
    {
        AGE_CORE_ASSERT(false, "Direct X Not Implemented!");
    }
}
#endif
```


