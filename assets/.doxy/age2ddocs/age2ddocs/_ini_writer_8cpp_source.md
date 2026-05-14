

# File IniWriter.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Serializers**](dir_0e7d7552020383c89e3ca069b8b7352b.md) **>** [**Private**](dir_ec26f5e2e3b4d07fbb894a640522da88.md) **>** [**IniWriter.cpp**](_ini_writer_8cpp.md)

[Go to the documentation of this file](_ini_writer_8cpp.md)


```C++
//
// Created by gdmgp on 12/5/2025.
//

#include "Core/Public/AGEpch.hpp"
#include "../Public/IniWriter.h"
#include "Core/Public/Log.h"


namespace AGE
{
IniWriter::IniWriter(const std::filesystem::path &Path)
        :m_IniPath(Path)
    {
        m_Ini.SetUnicode();

        SI_Error rc = m_Ini.LoadFile(Path.string().c_str());

        if (rc < 0)
        {
            CoreLogger::Error("Unable To Load {}", Path.string());
        }
    }

bool IniWriter::Write(const std::string &Section, const std::string &Key, const std::string &Value)
    {
        SI_Error rc = m_Ini.SetValue(Section.c_str(), Key.c_str(), Value.c_str());

        return rc == SI_INSERTED || rc == SI_UPDATED;
    }

bool IniWriter::SaveFile()
    {
        SI_Error rc = m_Ini.SaveFile(m_IniPath.c_str());

        return rc == SI_OK;

    }
} // AGE
```


