

# File JsonParser.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Parser**](dir_81d36680c9a9035d38dcc36084da83fe.md) **>** [**Public**](dir_b9d50061ecaa34aafe5e7c2ebce34886.md) **>** [**JsonParser.h**](_json_parser_8h.md)

[Go to the documentation of this file](_json_parser_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include "nlohmann/json.hpp"

namespace AGE
{


    class JsonParser
    {
    public:

JsonParser() = default;
        JsonParser(const std::string& FilePath);

        template<typename T>
        bool SaveJsonFile(const std::filesystem::path& Filepath, std::vector<T>& Data);

        static nlohmann::json LoadJsonFile(const std::filesystem::path& Filepath);

        static std::string Parse(const std::string& FilePath);

        static std::string ParseString(const std::string& String);

    };



}
```


