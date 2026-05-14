

# File IniWriter.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Serializers**](dir_0e7d7552020383c89e3ca069b8b7352b.md) **>** [**Public**](dir_35bb773506be3ac06655ba85521041b9.md) **>** [**IniWriter.h**](_ini_writer_8h.md)

[Go to the documentation of this file](_ini_writer_8h.md)


```C++
//
// Created by gdmgp on 12/5/2025.
//

#ifndef AGE2D_INIWRITER_H
#define AGE2D_INIWRITER_H
#include "Core/Public/Core.h"
#ifdef __clang__
#pragma clang diagnostic push
#pragma clang diagnostic ignored "-Wconversion"
#pragma clang diagnostic ignored "-Wmicrosoft-unqualified-friend"
#include "SimpleIni.h"
#pragma clang diagnostic pop
#elif defined(__GNUC__)
#pragma GCC diagnostic push
#pragma GCC diagnostic ignored "-Wconversion"
#include "SimpleIni.h"
#pragma GCC diagnostic pop
#elif defined(_MSC_VER)
#pragma warning(push, 0)
#include "SimpleIni.h"
#pragma warning(pop)
#else
#error "Compiler is not supported with AGE yet"
#endif

namespace AGE
{
    class IniWriter
    {
    public:
        IniWriter(const std::filesystem::path &Path);
~IniWriter() = default;

        bool Write(const std::string &Section, const std::string &Key, const std::string &Value);

        bool SaveFile();



    private:
        std::filesystem::path m_IniPath;
        CSimpleIniA m_Ini;
    };


} // AGE

#endif //AGE2D_INIWRITER_H
```


