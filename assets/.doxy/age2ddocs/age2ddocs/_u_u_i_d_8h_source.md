

# File UUID.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**UUID.h**](_u_u_i_d_8h.md)

[Go to the documentation of this file](_u_u_i_d_8h.md)


```C++
#pragma once
#ifdef AG_PLATFORM_WINDOWS
#include <xhash>
#else
#include <functional>
#endif
#include <cinttypes>
namespace AGE
{
    class UUID
    {
    public:
        UUID();
        UUID(uint64_t uuid);
        UUID(const UUID&) = default;


        operator uint64_t() const { return m_UUID; }

    private:

        uint64_t m_UUID;
    };

}

namespace std
{
    template<>
    struct hash<AGE::UUID>
    {
        std::size_t operator()(const AGE::UUID& uuid) const noexcept
        {
            return hash<uint64_t>()((uint64_t)uuid);
        }
    };
}
```


