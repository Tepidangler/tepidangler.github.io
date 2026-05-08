

# File Log.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**Log.cpp**](_log_8cpp.md)

[Go to the documentation of this file](_log_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Log.h"

#include "fmt/chrono.h"

namespace AGE
{
    Ref<spdlog::logger> Log::s_AGECoreLogger;
    Ref<spdlog::logger> Log::s_AGEGameLogger;
    std::vector<char> Log::s_Logs;
    std::vector<size_t> Log::s_Offsets;
    std::vector<LogType> Log::s_Type;

    void Log::Init()
    {
        spdlog::set_pattern("%^[%T] %n: %v%$");

        s_AGECoreLogger = spdlog::stdout_color_mt("AGECORE");
        s_AGECoreLogger->set_level(spdlog::level::trace);
        s_AGEGameLogger = spdlog::stdout_color_mt("AGEGAME");
        s_AGEGameLogger->set_level(spdlog::level::trace);
        s_Offsets.push_back(0);

    }
}
```


