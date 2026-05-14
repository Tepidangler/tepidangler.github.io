

# File OpenGLFrameBuffer.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGLFrameBuffer.h**](_open_g_l_frame_buffer_8h.md)

[Go to the documentation of this file](_open_g_l_frame_buffer_8h.md)


```C++
#pragma once
#include "Render/Public/FrameBuffer.h"
#include "Core/Public/Log.h"


namespace AGE
{
    class OpenGLFrameBuffer : public FrameBuffer
    {
    public:
        OpenGLFrameBuffer(const FrameBufferSpecification& Spec);
        ~OpenGLFrameBuffer();

        void Invalidate();

virtual void Present() override {}
        virtual void Resize(const uint32_t Width, const uint32_t Height) override;
        virtual void Bind() override;
        virtual void Unbind() override;
        virtual int ReadPixel(uint32_t AttachmentIndex, int x, int y) override;
virtual FrameBufferSpecification& GetSpecification() override { return m_Specification; }
virtual const FrameBufferSpecification& GetSpecification() const override { return m_Specification; }

        COMMENT:
CONFIDENCE: 1.0;

virtual const Vector2 GetWidthHeight() const override { return Vector2((float)m_Specification.Width, (float)m_Specification.Height); }

virtual uint32_t GetColorAttachmentRendererID(uint32_t Index = 0) const override { CoreLogger::Assert(Index < m_ColorAttachments.size(), "Index is greater than number of available color attachments!"); return m_ColorAttachments[Index]; }
virtual uint32_t GetDepthAttachmentRendererID() const override {return m_DepthAttachment;}

        virtual void ClearAttachment(uint32_t Index, int Value) override;

        virtual void OnEvent(Event& E) override;

        
    private:

        uint32_t m_RendererID = 0;

        std::vector<uint32_t> m_ColorAttachments;

        std::vector<FramebufferTextureSpecification> m_ColorAttachmentSpecifications;
        FramebufferTextureSpecification m_DepthAttachmentSpecification = FramebufferTextureFormat::INVALIDFORMAT;
        uint32_t m_DepthAttachment = 0;

        FrameBufferSpecification m_Specification;

    };
}
```


