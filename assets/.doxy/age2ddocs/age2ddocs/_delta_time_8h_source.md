

# File DeltaTime.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**DeltaTime.h**](_delta_time_8h.md)

[Go to the documentation of this file](_delta_time_8h.md)


```C++
#pragma once

namespace AGE
{
    class TimeStep
    {
    public:
        TimeStep(float time = 0.f)
            :m_Time(time)
        {
        }

        float GetSeconds() const { return m_Time; }
        float GetMilliseconds() const { return m_Time * 1000.f; }

        operator float() const { return m_Time; }

    private:
        float m_Time;
    };
}
```


