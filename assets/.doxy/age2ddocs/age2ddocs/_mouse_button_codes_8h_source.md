

# File MouseButtonCodes.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**MouseButtonCodes.h**](_mouse_button_codes_8h.md)

[Go to the documentation of this file](_mouse_button_codes_8h.md)


```C++
#pragma once

//Stolen form glfw3.h

typedef unsigned short uint16_t;

namespace AGE
{
    using MouseCode = uint16_t;

    namespace Mouse
    {
        enum Buttons: MouseCode
        {
            D1 = 0,
            D2 = 1,
            D3 = 2,
            D4 = 3,
            D5 = 4,
            D6 = 5,
            D7 = 6,
            D8 = 7,
            Last = D8,
            Left = D1,
            Right = D2,
            Middle = D3
        };
    }
}
```


