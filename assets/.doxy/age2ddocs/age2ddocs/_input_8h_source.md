

# File Input.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Input.h**](_input_8h.md)

[Go to the documentation of this file](_input_8h.md)


```C++
#pragma once
#include "Core.h"
#include "Keycodes.h"
#include "MouseButtonCodes.h"

namespace AGE
{
class AGE_API Input
     {
        public:
            static bool IsKeyPressed(int Keycode);

            static bool IsMouseButtonPressed(int Button); 

            static bool IsGamepadButtonPressed(uint16_t ID, uint8_t Button);

            static float GetMouseX();

            static float GetMouseY();

            static std::pair<float,float> GetMouseXY();

            static bool IsJoyStickConnected(uint16_t ID);

            static float GetJoyStickLeftX(uint16_t ID);
            static float GetJoyStickLeftY(uint16_t ID);

            static std::pair<float,float> GetJoyStickLeftXY(uint16_t ID);

            static float GetJoyStickRightX(uint16_t ID);
            static float GetJoyStickRightY(uint16_t ID);
            static std::pair<float, float> GetJoyStickRightXY(uint16_t ID);

            static float GetJoyStickLeftTrigger(uint16_t ID);
            static float GetJoyStickRightTrigger(uint16_t ID);


     private:
         static bool IsJoyStickPresent(uint16_t ID);
    
     };
}
```


