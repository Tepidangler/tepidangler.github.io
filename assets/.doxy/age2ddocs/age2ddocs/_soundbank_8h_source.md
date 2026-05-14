

# File Soundbank.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Audio**](dir_db6938f1ff25f5ebd4fcc50cd8804f79.md) **>** [**AudioEngine**](dir_bf6a2ae4f421b3e627c8671719c9dbdd.md) **>** [**Public**](dir_ea32d5a6b44ca038dc6c67f0bb71548f.md) **>** [**Soundbank.h**](_soundbank_8h.md)

[Go to the documentation of this file](_soundbank_8h.md)


```C++
//
// Created by De'Lano Wilcox on 11/22/2025.
//
#pragma once
#ifndef AGE_SOUNDBANK_H
#define AGE_SOUNDBANK_H

#endif //AGE_SOUNDBANK_H

#include "Core/Public/UUID.h"
#include <string>
#include <filesystem>

namespace AGE
{
    class SoundBank
    {
    public:
        SoundBank(const std::filesystem::path& FilePath, UUID ID);
SoundBank(const SoundBank&) = default;
~SoundBank() = default;

std::filesystem::path& GetFilePath() {return m_FilePath; }
std::string& GetBankName() {return m_Name;}
void SetBankName(const std::string& Name) {m_Name = Name;};
uint32_t GetBankID() {return m_ID;}
void SetBankID(uint32_t ID) {m_ID = ID;}

UUID& GetAssetID() {return m_AssetID;}

        std::filesystem::path m_FilePath;
        std::string m_Name;
        uint32_t m_ID;
        UUID m_AssetID;
    };


}
```


