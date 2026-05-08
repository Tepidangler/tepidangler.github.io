

# File Timer.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Timer.h**](_timer_8h.md)

[Go to the documentation of this file](_timer_8h.md)


```C++
#pragma once
#include <chrono>

namespace AGE
{
    class Timer
    {
    public:

        Timer()
        {
            Reset();
        }

        void Reset()
        {
            m_Start = std::chrono::high_resolution_clock::now();
        }

        float Elapsed()
        {
            //return std::chrono::duration_cast<std::chrono::nanoseconds>(
            //         std::chrono::high_resolution_clock::now() - m_Start).count() * .001f * .001f * .001f;

            return std::chrono::duration<float, std::nano>(std::chrono::high_resolution_clock::now() - m_Start).count() * .001f * .001f * .001f;
        }

        float ElapsedMillis()
        {
            return Elapsed() * 1000.f;
        }

    private:

        std::chrono::time_point<std::chrono::high_resolution_clock> m_Start;
    };
}
```


