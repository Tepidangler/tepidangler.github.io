

# File OpenGLVertexArray.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGLVertexArray.h**](_open_g_l_vertex_array_8h.md)

[Go to the documentation of this file](_open_g_l_vertex_array_8h.md)


```C++
#pragma once
#include "Render/Public/VertexArray.h"
#include <memory>

namespace AGE
{
    class OpenGLVertexArray : public VertexArray
    {
    public:

        OpenGLVertexArray();

        ~OpenGLVertexArray() override;

        void Bind() const override;

        void Unbind() const override;

        void AddVertexBuffer(Ref<VertexBuffer>& VertexBuffer) override;

        void SetIndexBuffer(Ref<IndexBuffer>& IndexBuffer) override;

        const std::vector<Ref<VertexBuffer>>& GetVertexBuffers() const override { return m_VertexBuffers; }

        const Ref<IndexBuffer>& GetIndexBuffer() const override { return m_IndexBuffer; }
        
        void EnableVertexAttribArray(uint32_t ArrayID) const override;

        void MakeVertexAttribPtr(uint32_t index, int size, uint32_t type, uint8_t normalized, int stride, const void* pointer) const override;

        std::vector<Ref<VertexBuffer>>::iterator begin() override { return m_VertexBuffers.begin(); }

        std::vector<Ref<VertexBuffer>>::iterator end() override { return m_VertexBuffers.end(); }

        std::vector<Ref<VertexBuffer>>::const_iterator begin() const override { return m_VertexBuffers.begin(); }

        std::vector<Ref<VertexBuffer>>::const_iterator end() const override { return m_VertexBuffers.end(); }


    private:

        std::vector<Ref<VertexBuffer>> m_VertexBuffers;
        Ref<IndexBuffer> m_IndexBuffer;
        uint32_t m_ArrayID;
    };
}
```


