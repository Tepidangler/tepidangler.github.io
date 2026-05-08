

# File Texture.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Texture**](dir_3194396490e5a71e19ad7a016853cc4f.md) **>** [**Public**](dir_f02d8c73f2f37e5e80bb760b434406e3.md) **>** [**Texture.h**](_texture_8h.md)

[Go to the documentation of this file](_texture_8h.md)


```C++
#pragma once
#include <tmx.h>
#include "Sprite/Public/Image.h"


namespace AGE
{
    class DataReader;
    class DataWriter;

    enum class ImageFormat : uint8_t
    {
        INVALIDIMAGEFORMAT = 0,
        R8,
        RG8,
        RGB8,
        RGBA8,
        RG16F,
        RGBA32F
    };

    struct TextureSpecification
    {
    public:
        TextureSpecification() = default;
        virtual ~TextureSpecification() = default;

        uint32_t Width = 1;
        uint32_t Height = 1;
        ImageFormat Format = ImageFormat::RGBA8;
        bool GenerateMips = true;
        bool IsArray = false;
        static void Serialize(DataWriter* Serializer, const TextureSpecification& Instance);
        static void Deserialize(DataReader* Serializer, TextureSpecification& Instance);
    };

    class Texture
    {
    public:
        virtual ~Texture() {}

        virtual void Bind(uint32_t Slot = 0) const = 0;

        virtual const TextureSpecification& GetSpecification() const = 0;

        virtual void Unbind() const = 0;
        virtual uint32_t GetWidth() const = 0;
        virtual uint32_t GetHeight() const = 0;

        virtual uint32_t GetTextureID() const = 0;
        virtual uint64_t GetAssetID() const = 0;
        virtual void SetAssetID(uint64_t ID) = 0;
        virtual std::string GetName() const = 0;
        virtual void SetName(const std::string& Name) = 0;
        virtual std::string GetTextureFilePath() const = 0;
        virtual void SetTextureFilePath(const std::string& Path) = 0;
        virtual std::pair<uint8_t*, size_t> GetTextureData() = 0;
        virtual void SetData(void* Data, uint32_t Size) = 0;


        virtual bool operator==(const Texture& Other) const = 0;


    };

    class Texture2D : public Texture
    {
    public:

        static Ref<Texture2D> Create(const std::string& Path);
        static Ref<Texture2D> Create(uint8_t* Image, const TextureSpecification& Spec);
        static Ref<Texture2D> Create(const std::vector<std::string>& Path);
        static Ref<Texture2D> Create(const TextureSpecification& Spec);
        static Ref<Texture2D> Create(const Image* Img, uint32_t Width, uint32_t Height, int Channels, size_t Size);

        template<typename T>
        T* As();

    };


}
```


