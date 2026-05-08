

# File Soundbank.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Audio**](dir_db6938f1ff25f5ebd4fcc50cd8804f79.md) **>** [**AudioEngine**](dir_bf6a2ae4f421b3e627c8671719c9dbdd.md) **>** [**Private**](dir_933cf9cfa8f6f567c0c937ed7947c49a.md) **>** [**Soundbank.cpp**](_soundbank_8cpp.md)

[Go to the documentation of this file](_soundbank_8cpp.md)


```C++
//
// Created by De'Lano Wilcox on 11/22/2025.
//

#include "Audio/AudioEngine/Public/Soundbank.h"

namespace AGE
{
    SoundBank::SoundBank(const std::filesystem::path& FilePath, UUID ID)
        :m_FilePath(FilePath), m_AssetID(ID)
    {
        m_Name = m_FilePath.filename().string();
    }
}
```


