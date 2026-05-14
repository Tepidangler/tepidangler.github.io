

# File Vector4.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Math**](dir_5b9993be36110f29e6abf37e5784a4f8.md) **>** [**Private**](dir_4591091c161a59a7c245ad7688ad7744.md) **>** [**Vector4.cpp**](_vector4_8cpp.md)

[Go to the documentation of this file](_vector4_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Math/Public/Vector4.h"
#ifdef AG_PLATFORM_WINDOWS
#include <shtypes.h>
#endif

namespace AGE {
Vector4::Vector4() {
        x = 0;
        y = 0;
        z = 0;
        w = 0;
    }

Vector4::Vector4(float a) {
        x = a;
        y = a;
        z = a;
        w = a;
    }

Vector4::Vector4(glm::vec4 vec) {
        x = vec.x;
        y = vec.y;
        z = vec.z;
        w = vec.w;
    }

Vector4::Vector4(float a, float b, float c, float d) {
        x = a;
        y = b;
        z = c;
        w = d;
    }

    COMMENT:
CONFIDENCE: 1.0;

Vector4::Vector4(uint8_t a, uint8_t b, uint8_t c, uint8_t d)
    {
        std::byte tmpbyte = std::byte(a);
        int tmpint = std::to_integer<int>(tmpbyte);
        x = ((100.f * (float)tmpint) / 255.f) * .01f;

        tmpbyte = std::byte(b);
        tmpint = std::to_integer<int>(tmpbyte);
        y = ((100.f * (float)tmpint) / 255.f) * .01f;

        tmpbyte = std::byte(c);
        tmpint = std::to_integer<int>(tmpbyte);
        z = ((100.f * (float)tmpint) / 255.f) * .01f;

        tmpbyte = std::byte(d);
        tmpint = std::to_integer<int>(tmpbyte);

        w = ((100.f * (float)tmpint) / 255.f) * .01f;
    }

Vector4::Vector4(const float* color) {
        x = color[0];
        y = color[1];
        z = color[2];
        w = color[3];
    }

    //void Vector4::Serialize(DataWriter *Serializer, const Vector4 &Instance)
    //{
    //  Serializer->WriteRaw<float>(Instance.x);
    //  Serializer->WriteRaw<float>(Instance.y);
    //  Serializer->WriteRaw<float>(Instance.z);
    //  Serializer->WriteRaw<float>(Instance.w);
    //}
//
    //void Vector4::Deserialize(DataReader *Serializer, Vector4 &Instance)
    //{
    //  Serializer->ReadRaw<float>(Instance.x);
    //  Serializer->ReadRaw<float>(Instance.y);
    //  Serializer->ReadRaw<float>(Instance.z);
    //  Serializer->ReadRaw<float>(Instance.w);
    //}

Vector4 Vector4::normalize() const
    {
        return Vector4();
    }
}
```


