

# File Font.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Public**](dir_68ba7e1260de504efb39109a85960357.md) **>** [**Font.h**](_font_8h.md)

[Go to the documentation of this file](_font_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "Texture/Public/Texture.h"

namespace AGE
{
    struct MSDFData;

    class AGEFont : public std::enable_shared_from_this<AGEFont>
    {
    public:
        AGEFont(const std::filesystem::path& Font, bool LoadingDefault = false);
        ~AGEFont();

        const MSDFData* GetMSDFData() const { return m_Data; }
        Ref<Texture2D> GetAtlasTexture() const { return m_AtlasTexture; }

        void SaveFont();
        void LoadFont(const std::string& FontName);

        static Ref<AGEFont> GetDefault();

        const std::string& GetFontName() const { return m_FontName; }
        uint64_t GetAssetID() const { return m_AssetID; }

    private:
        void SaveDefaultFont();
        void LoadDefaultFont(const std::string& FontName);
        MSDFData* m_Data;
        Ref<Texture2D> m_AtlasTexture;
        std::string m_FontName;
        uint64_t m_AssetID;
    };
}
```


