

# File WindowsUtils.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Utils**](dir_2ea46939f511f6144e40e8e7d32aa78e.md) **>** [**Public**](dir_6a98f83a49b4a8e48cceea88fbb59588.md) **>** [**WindowsUtils.h**](_windows_utils_8h.md)

[Go to the documentation of this file](_windows_utils_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include <ranges>
#include <string>

namespace AGE
{
    class FileDialogs
    {
    public:
        //Return "" if cancelled
        static std::string OpenFile(const std::string& Title, const std::filesystem::path& DefaultPath, std::vector<std::string> Filter);
        static std::string SaveFile(const std::string& Title, const std::filesystem::path& DefaultPath, std::vector<std::string> Filter);
    };
}
```


