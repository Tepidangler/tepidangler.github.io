

# File Types.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Types.h**](_types_8h.md)

[Go to the documentation of this file](_types_8h.md)


```C++
//
// Created by gdmgp on 3/24/2026.
//

#ifndef AGE_TYPES_H
#define AGE_TYPES_H
#include <cstdint>
#include <cstring>

namespace AGE
{
    struct float16
    {
         uint16_t bits;

    float16() = default;

    // Construct from float32
    float16(float value)
    {
        bits = float32_to_float16(value);
    }

    // Convert back to float32
    operator float() const
    {
        return float16_to_float32(bits);
    }

private:
    static uint16_t float32_to_float16(float value)
    {
        uint32_t f;
        std::memcpy(&f, &value, sizeof(f));

        uint32_t sign = (f >> 16) & 0x8000;
        uint32_t mantissa = f & 0x007FFFFF;
        int32_t exp = ((f >> 23) & 0xFF) - 127 + 15;

        if (exp <= 0)
        {
            if (exp < -10)
                return (uint16_t)sign;

            mantissa |= 0x00800000;
            int shift = 14 - exp;

            uint16_t m = (uint16_t)(mantissa >> shift);

            // round
            if ((mantissa >> (shift - 1)) & 1)
                m++;

            return sign | m;
        }
        else if (exp >= 31)
        {
            if (mantissa == 0)
                return (uint16_t)(sign | 0x7C00); // Inf

            return (uint16_t)(sign | 0x7C00 | (mantissa >> 13)); // NaN
        }

        uint16_t h_exp = (uint16_t)(exp << 10);
        uint16_t h_man = (uint16_t)(mantissa >> 13);

        // round
        if (mantissa & 0x00001000)
        {
            h_man++;
            if (h_man == 0x0400)
            {
                h_man = 0;
                h_exp += 0x0400;
            }
        }

        return (uint16_t)(sign | h_exp | h_man);
    }

    static float float16_to_float32(uint16_t h)
    {
        uint32_t sign = (h & 0x8000) << 16;
        uint32_t exp  = (h >> 10) & 0x1F;
        uint32_t mant = h & 0x03FF;

        uint32_t f;

        if (exp == 0)
        {
            if (mant == 0)
            {
                // Zero
                f = sign;
            }
            else
            {
                // Subnormal → normalize
                exp = 1;
                while ((mant & 0x0400) == 0)
                {
                    mant <<= 1;
                    exp--;
                }
                mant &= 0x03FF;

                exp = exp + (127 - 15);
                mant <<= 13;

                f = sign | (exp << 23) | mant;
            }
        }
        else if (exp == 31)
        {
            // Inf or NaN
            f = sign | 0x7F800000 | (mant << 13);
        }
        else
        {
            // Normalized
            exp = exp + (127 - 15);
            mant <<= 13;

            f = sign | (exp << 23) | mant;
        }

        float result;
        std::memcpy(&result, &f, sizeof(result));
        return result;
    }
    };
} // AGE

typedef AGE::float16 half_t;

#endif //AGE_TYPES_H
```


