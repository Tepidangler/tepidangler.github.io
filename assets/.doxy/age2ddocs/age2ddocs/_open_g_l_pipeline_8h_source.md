

# File OpenGLPipeline.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGLPipeline.h**](_open_g_l_pipeline_8h.md)

[Go to the documentation of this file](_open_g_l_pipeline_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Render/Public/Pipeline.h"

namespace AGE
{
    class OpenGLPipeline : public Pipeline
    {
    public:

        OpenGLPipeline();
        ~OpenGLPipeline() override;

        void Init() override;
        void StartBatch2D() override;
        void NextBatch2D() override;
        void Flush2D() override;

        Renderer2DData& GetData() override;
        void ResetStats() override;
        Statistics& GetStats() override;
        void GenerateDefaultTextures();

    private:
        Renderer2DData m_Data;
    };
}
```


