

# File Texture.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Texture**](dir_3194396490e5a71e19ad7a016853cc4f.md) **>** [**Private**](dir_beb370da822bf0b51577351bd056b4ca.md) **>** [**Texture.cpp**](_texture_8cpp.md)

[Go to the documentation of this file](_texture_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Core/Public/Core.h"
#include "Texture/Public/Texture.h"
#include "Render/Public/Renderer.h"
#include "Platform/OpenGL/Public/OpenGLTexture.h"

namespace AGE
{

    Ref<Texture2D> Texture2D::Create(const std::string& Path)
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateRef<OpenGLTexture2D>(Path);
            break;
        default:
            AGE_CORE_ASSERT(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }

    Ref<Texture2D> Texture2D::Create(uint8_t* Image, const TextureSpecification& Spec)
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateRef<OpenGLTexture2D>(Image,Spec);
            break;
        default:
            AGE_CORE_ASSERT(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }

    Ref<Texture2D> Texture2D::Create(const std::vector<std::string>& Paths)
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateRef<OpenGLTexture2D>(Paths);
            break;
        default:
            AGE_CORE_ASSERT(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }

    Ref<Texture2D> Texture2D::Create(const TextureSpecification& Spec)
    {
        switch (Renderer::GetAPI())
        {
            case 0:
                AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
                return nullptr;
                break;
            case 1:
                return CreateRef<OpenGLTexture2D>(Spec);
                break;
            default:
                AGE_CORE_ASSERT(false, "Unknown Renderer API!");
                return nullptr;
                break;
            }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }
    Ref<Texture2D> Texture2D::Create(const Image* Img, uint32_t Width, uint32_t Height, int Channels, size_t Size)
    {
        switch (Renderer::GetAPI())
        {
        case 0:
            AGE_CORE_ASSERT(false, "RendererAPI::API::None is currently not supported!");
            return nullptr;
            break;
        case 1:
            return CreateRef<OpenGLTexture2D>(Img, Width, Height, Channels, Size);
            break;
        default:
            AGE_CORE_ASSERT(false, "Unknown Renderer API!");
            return nullptr;
            break;
        }
        AGE_CORE_ASSERT(false, "Unknown Renderer API!");
        return nullptr;
    }

    template<typename T>
    T* Texture2D::As()
    {
        AGE_CORE_ASSERT(false, "As() Failed!");
        return nullptr;
    }

    void TextureSpecification::Serialize(DataWriter* Serializer, const TextureSpecification& Instance)
    {
        Serializer->WriteRaw<uint32_t>(Instance.Width);
        Serializer->WriteRaw<uint32_t>(Instance.Height);
        Serializer->WriteRaw<uint8_t>((uint8_t)Instance.Format);
        Serializer->WriteRaw<bool>(Instance.GenerateMips);
    }

    void TextureSpecification::Deserialize(DataReader* Serializer, TextureSpecification& Instance)
    {
        Serializer->ReadRaw<uint32_t>(Instance.Width);
        Serializer->ReadRaw<uint32_t>(Instance.Height);
        uint8_t format;
        Serializer->ReadRaw<uint8_t>(format);
        Instance.Format = (ImageFormat)format;
        Serializer->ReadRaw<bool>(Instance.GenerateMips);
    }
}
```


