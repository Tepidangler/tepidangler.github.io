

# File WindowsUtils.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Utils**](dir_2ea46939f511f6144e40e8e7d32aa78e.md) **>** [**Private**](dir_1cbb136cab301e6e794b9ffbc12fda9b.md) **>** [**WindowsUtils.cpp**](_windows_utils_8cpp.md)

[Go to the documentation of this file](_windows_utils_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Utils/Public/WindowsUtils.h"

#ifdef __clang__
#pragma clang diagnostic push
#pragma clang diagnostic ignored "-Wsign-conversion"
#include "portable-file-dialogs.h"
#pragma clang diagnostic pop
#elif defined(__GNUC__)
#pragma GCC diagnostic push
#pragma clang diagnostic ignored "-Wsign-conversion"
#include "portable-file-dialogs.h"
#pragma GCC diagnostic pop
#elif defined(_MSC_VER)
#pragma warning(push, 0)
#include "portable-file-dialogs.h"
#pragma warning(pop)
#else
#error "Compiler is not supported with AGE yet"
#endif

namespace AGE
{
    std::string FileDialogs::OpenFile(const std::string& Title, const std::filesystem::path& DefaultPath, std::vector<std::string> Filter)
    {
        auto f = pfd::open_file(Title.c_str(), DefaultPath.generic_string(),
            Filter);

        if (f.result().empty())
        {
            return {};
        }

        return f.result()[0];
    }

    std::string FileDialogs::SaveFile(const std::string& Title, const std::filesystem::path& DefaultPath, std::vector<std::string> Filter)
    {
        auto f = pfd::save_file(Title.c_str(), DefaultPath.generic_string(),
            Filter
            ,pfd::opt::force_overwrite);

        if (f.result().empty())
        {
            return {};
        }

        return f.result();
    }
}
```


