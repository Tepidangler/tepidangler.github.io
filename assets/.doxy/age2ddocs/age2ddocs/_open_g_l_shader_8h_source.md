

# File OpenGLShader.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Public**](dir_910dbe77797081a1ec62d5e5934a1ea3.md) **>** [**OpenGLShader.h**](_open_g_l_shader_8h.md)

[Go to the documentation of this file](_open_g_l_shader_8h.md)


```C++
#pragma once
#include "Render/Public/Shader.h"
#include <glm/glm.hpp>

//REMOVE
typedef unsigned int GLenum;

namespace AGE
{
    class OpenGLShader : public Shader
    {
    public:
        OpenGLShader(const std::string& FilePath);
        OpenGLShader(const std::string& VertexSrcPath, const std::string& FragmentSrcPath);
        OpenGLShader(const std::string& Name, const std::string& VertexSrc, const std::string& FragmentSrc);

        virtual ~OpenGLShader();

        void Bind() const override;
        void Unbind() const override;

        void SetFloat(const char* Name, float Values, float* ValuePtr = nullptr, int Count = 2) const override;
        void SetFloat2(const char* Name, const Vector2& Values, const Vector2* ValuePtr= nullptr, int Count = 2) const override;
        void SetFloat3(const char* Name, const Vector3& Values, const Vector3* ValuePtr= nullptr, int Count = 2) const override;
        void SetFloat4(const char* Name, const Vector4& Value, const Vector4* ValuePtr = nullptr, int Count = 2) const override;
        void SetMat3(const char* Name, const Matrix3D& Matrix) const override;
        void SetMat4(const char* Name, const Matrix4D& Matrix) const override;
        void SetInt(const char* Name, const int Texture = 0, const int* TexturePtr = nullptr, const int Count = 2) const override;

        const std::string& GetShaderName() const override { return m_ShaderName; }

        void UploadFloat(const char* Name, float Values, float* ValuePtr = nullptr, int Count = 2) const;
        void UploadFloat2(const char* Name, const Vector2& Values, const Vector2* ValuePtr= nullptr, int Count = 2) const;
        void UploadFloat3(const char* Name, const Vector3& Values, const Vector3* ValuePtr= nullptr, int Count = 2) const;
        void UploadFloat4(const char* Name, const Vector4& Value, const Vector4* ValuePtr = nullptr, int Count = 2) const;
        void UploadMat3(const char* Name, const Matrix3D& Matrix) const;
        void UploadMat4(const char* Name, const Matrix4D& Matrix) const;
        void UploadInt(const char* Name, const int Texture = 0, const int* TexturePtr = nullptr, const int Count = 2) const;

        std::string ReadFile(const std::string FilePath);

        std::unordered_map < GLenum, std::string> PreProcess(const std::string& Source);

        void Compile(const std::unordered_map<GLenum, std::string>& ShaderSources);

        inline virtual uint32_t GetRendererID() const override { return m_RendererID; }

        
    private:
        uint32_t m_RendererID;
        std::string m_ShaderName;
    };
}
```


