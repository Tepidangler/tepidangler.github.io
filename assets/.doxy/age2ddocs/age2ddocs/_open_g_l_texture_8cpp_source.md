

# File OpenGLTexture.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Platform**](dir_016fed4b0a3cb950c530bbf3738fb926.md) **>** [**OpenGL**](dir_ebb7378fee88e7e575044fff67f59924.md) **>** [**Private**](dir_70227f149653e1f1d3b9a02604511f36.md) **>** [**OpenGLTexture.cpp**](_open_g_l_texture_8cpp.md)

[Go to the documentation of this file](_open_g_l_texture_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Core/Public/Core.h"
#include "Render/Public/Renderer.h"
#include "Platform/OpenGL/Public/OpenGLTexture.h"
#include "Statics/Public/Statics.h"


#include <glad/glad.h>
#include <stb_image.h>

namespace AGE
{
    namespace Utils
    {
        static GLenum AGEImageFormatToGLDataFormat(ImageFormat Format)
        {
            switch (Format)
            {
            case ImageFormat::R8:
            {
                return GL_RED;
            }
            case ImageFormat::RG16F:
            case ImageFormat::RG8:
            {
                return GL_RG;
            }
            case ImageFormat::RGB8:
            {
                return GL_RGB;
            }
            case ImageFormat::RGBA32F:
            case ImageFormat::RGBA8:
            {
                return GL_RGBA;
            }
            default:
            {
                break;
            }
            }

            AGE_CORE_ASSERT(false, "Data Format not supported by AGE!");
            return 0;
        }

        static GLenum AGEImageFormatToGLInternalFormat(ImageFormat Format)
        {
            switch (Format)
            {
            case ImageFormat::R8:
            {
                return GL_R8;
            }
            case ImageFormat::RG8:
            {
                return GL_RG8;
            }
            case ImageFormat::RGB8:
            {
                return GL_RGB8;
            }
            case ImageFormat::RGBA8:
            {
                return GL_RGBA8;
            }
            case ImageFormat::RG16F:
            {
                return GL_RG16F;
            }
            case ImageFormat::RGBA32F:
            {
                return GL_RGBA32F;
            }

            default:
            {
                break;
            }
            }

            AGE_CORE_ASSERT(false, "Internal Format not supported by AGE!");
            return 0;
        }

    }

    OpenGLTexture2D::OpenGLTexture2D(const TextureSpecification& Spec)
        :m_Specification(Spec), m_Width((int)Spec.Width), m_Height((int)Spec.Height)
    {
        AGE_PROFILE_FUNCTION();
        m_InternalFormat = Utils::AGEImageFormatToGLInternalFormat(Spec.Format);
        m_DataFormat = Utils::AGEImageFormatToGLDataFormat(Spec.Format);

        if (Spec.IsArray)
        {
            glCreateTextures(GL_TEXTURE_2D_ARRAY, 1, &m_TextureID);
            glTextureStorage2D(m_TextureID, 1, m_InternalFormat, m_Width, m_Height);

            //Set Texture wrapping params
            glTexParameteri(GL_TEXTURE_2D_ARRAY, GL_TEXTURE_WRAP_S, GL_REPEAT);

            glTexParameteri(GL_TEXTURE_2D_ARRAY, GL_TEXTURE_WRAP_T, GL_REPEAT);


            //Set Texture filtering params
            glTexParameteri(GL_TEXTURE_2D_ARRAY, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

            glTexParameteri(GL_TEXTURE_2D_ARRAY, GL_TEXTURE_MAG_FILTER, GL_NEAREST);

            //glGenerateMipmap(m_TextureID);
        }
        else
        {
            glCreateTextures(GL_TEXTURE_2D, 1, &m_TextureID);
            glTextureStorage2D(m_TextureID, 1, m_InternalFormat, m_Width, m_Height);

            //Set Texture wrapping params
            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_REPEAT);

            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_REPEAT);


            //Set Texture filtering params
            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);

            //glGenerateMipmap(m_TextureID);
        }

    }

    OpenGLTexture2D::OpenGLTexture2D(const Image* Img, uint32_t Width, uint32_t Height, int Channels, size_t Size)
        :m_Width((int)Width), m_Height((int)Height), m_nrChannels(Channels)
    {
        AGE_PROFILE_FUNCTION();

        GLenum InternalFormat = 0, DataFormat = 0;
        if (m_nrChannels == 4)
        {
            InternalFormat = GL_RGBA8;
            DataFormat = GL_RGBA;
        }
        else if (m_nrChannels == 3)
        {
            InternalFormat = GL_RGB8;
            DataFormat = GL_RGB;
        }

        m_InternalFormat = InternalFormat;
        m_DataFormat = DataFormat;

        AGE_CORE_ASSERT(InternalFormat & DataFormat, "Format not supported!");
        glCreateTextures(GL_TEXTURE_2D,1, &m_TextureID);

        glTextureStorage2D(m_TextureID, 1, InternalFormat, m_Width, m_Height);

        //glPixelStorei(GL_UNPACK_ALIGNMENT, 1);

        //Set Texture wrapping params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_REPEAT);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_REPEAT);

        //Set Texture filtering params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);

        CoreLogger::Error("OpenGL Error: {}",glGetError());
        glTextureSubImage2D(m_TextureID, 0, 0, 0, m_Width, m_Height, DataFormat, GL_UNSIGNED_BYTE, Img->GetImageBuffer());
        CoreLogger::Error("OpenGL Error: {}",glGetError());


    }
    
    OpenGLTexture2D::OpenGLTexture2D(const std::string& Path)
        : m_Path(Path), m_AssetID(UUID())
    {
        AGE_PROFILE_FUNCTION();

        unsigned char *Data = nullptr;
        {
            stbi_set_flip_vertically_on_load(true);
            AGE_PROFILE_SCOPE("stbi_load -> OpenGLTexture2D::OpenGLTexture2D(const std::string& Path)");
            Data = stbi_load(Path.c_str(), &m_Width, &m_Height, &m_nrChannels, 0);
        }
        AGE_CORE_ASSERT(Data != nullptr, "Unable to Load Image");


        GLenum InternalFormat = 0, DataFormat = 0;
        if (m_nrChannels == 4)
        {
            InternalFormat = GL_RGBA8;
            DataFormat = GL_RGBA;
        } else if (m_nrChannels == 3)
        {
            InternalFormat = GL_RGB8;
            DataFormat = GL_RGB;
        } else if (m_nrChannels == 2)
        {
            InternalFormat = GL_RG8;
            DataFormat = GL_RG;
        } else
        {
            InternalFormat = GL_R8;
            DataFormat = GL_RED;
        }
        m_InternalFormat = InternalFormat;
        m_DataFormat = DataFormat;

        AGE_CORE_ASSERT(InternalFormat & DataFormat, "Format not supported!");
        glCreateTextures(GL_TEXTURE_2D, 1, &m_TextureID);

        glTextureStorage2D(m_TextureID, 1, InternalFormat, m_Width, m_Height);

        //Set Texture wrapping params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_REPEAT);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_REPEAT);

        //Set Texture filtering params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);

        OpenGLTexture2D::SetData(Data, m_Width * m_Height * m_nrChannels);

        CoreLogger::Error("OpenGLTexture2D(const std::string& Path) OpenGl Error: {}", glGetError());
        stbi_image_free(Data);
        std::filesystem::path FilePath = m_Path;
        m_Name = Utils::EngineStatics::GetFilename(FilePath);
    }

    OpenGLTexture2D::OpenGLTexture2D(uint8_t* Image, const TextureSpecification& Spec)
        :m_Width(Spec.Width), m_Height(Spec.Height), m_nrChannels(4)
    {
        m_InternalFormat = Utils::AGEImageFormatToGLInternalFormat(Spec.Format);
        m_DataFormat = Utils::AGEImageFormatToGLDataFormat(Spec.Format);
        AGE_CORE_ASSERT(Image != nullptr, "Unable to Load Image");

        AGE_CORE_ASSERT(m_InternalFormat & m_DataFormat, "Format not supported!");
        glCreateTextures(GL_TEXTURE_2D, 1, &m_TextureID);
        glTextureStorage2D(m_TextureID, 1, m_InternalFormat, m_Width, m_Height);
        //Set Texture wrapping params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_REPEAT);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_REPEAT);

        //Set Texture filtering params
        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

        glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);

        OpenGLTexture2D::SetData(Image, Spec.Width * Spec.Height * m_nrChannels);
    }

    OpenGLTexture2D::OpenGLTexture2D(const std::vector<std::string>& Paths)
    {
        AGE_PROFILE_FUNCTION();
        //stbi_set_flip_vertically_on_load(true);
        for (size_t i = 0; i < Paths.size(); i++)
        {


            unsigned char* Data = nullptr;
            {
                AGE_PROFILE_SCOPE("stbi_load -> OpenGLTexture2D::OpenGLTexture2D(const std::string& Path)");
                Data = stbi_load(Paths[i].c_str(), &m_Width, &m_Height, &m_nrChannels, 0);

            }
            AGE_CORE_ASSERT(Data, "Unable to Load Image");

            GLenum InternalFormat = 0, DataFormat = 0;
            if (m_nrChannels == 4)
            {
                InternalFormat = GL_RGBA8;
                DataFormat = GL_RGBA;
            }
            else if (m_nrChannels == 3)
            {
                InternalFormat = GL_RGB8;
                DataFormat = GL_RGB;
            }

            m_InternalFormat = InternalFormat;
            m_DataFormat = DataFormat;

            AGE_CORE_ASSERT(InternalFormat & DataFormat, "Format not supported!");
                glCreateTextures(GL_TEXTURE_2D, 1, &m_TextureID);

            glTextureStorage2D(m_TextureID, 1, InternalFormat, m_Width, m_Height);

            //Set Texture wrapping params
            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_REPEAT);

            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_REPEAT);

            //Set Texture filtering params
            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MIN_FILTER, GL_NEAREST);

            glTexParameteri(GL_TEXTURE_2D, GL_TEXTURE_MAG_FILTER, GL_NEAREST);


            glTextureSubImage2D(m_TextureID, 0, 0, 0, m_Width, m_Height, DataFormat, GL_UNSIGNED_BYTE, Data);

            //glGenerateMipmap(m_TextureID);

            stbi_image_free(Data);
        }
    }


    OpenGLTexture2D::~OpenGLTexture2D()
    {
        AGE_PROFILE_FUNCTION();
        glDeleteTextures(1, &m_TextureID);
    }
    void OpenGLTexture2D::Bind(uint32_t Slot) const
    {
        AGE_PROFILE_FUNCTION();
        glBindTextureUnit(Slot, m_TextureID);

    }
    void OpenGLTexture2D::Unbind() const
    {
        glBindTextureUnit(0, 0);
    }

    void OpenGLTexture2D::SetData(void* Data, uint32_t Size)
    {
        AGE_PROFILE_FUNCTION();
        uint32_t bpc; //bytes per channel
        switch (m_DataFormat)
        {
            case GL_RGBA: bpc = 4; break;
            case GL_RGB: bpc = 3; break;
            case GL_RG: bpc = 2; break;
            default: bpc = 1; break;
        }
        AGE_CORE_ASSERT(Size == ((uint32_t)(m_Width * m_Height) * bpc), "Size Data must be entire texture!");

        switch (m_InternalFormat)
        {
            case GL_RG16F:
            {
                glTextureSubImage2D(m_TextureID, 0, 0, 0, m_Width, m_Height, m_DataFormat, GL_HALF_FLOAT, Data);
                break;
            }
            case GL_RGBA32F:
            case GL_RG32F:
            {
                glTextureSubImage2D(m_TextureID, 0, 0, 0, m_Width, m_Height, m_DataFormat, GL_FLOAT, Data);
                break;
            }
            default:
            {
                glTextureSubImage2D(m_TextureID, 0, 0, 0, m_Width, m_Height, m_DataFormat, GL_UNSIGNED_BYTE, Data);
                break;
            }
        }
        if (!m_ImageData.first)
        {
            m_ImageData.first = new uint8_t[Size];
#ifdef AG_PLATFORM_WINDOWS
            memcpy_s(m_ImageData.first,Size, Data, Size);
#else
            memcpy(m_ImageData.first, Data, Size);
#endif
            m_ImageData.second = Size;
        }
    }

}
```


