

# File Vector3.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Math**](dir_5b9993be36110f29e6abf37e5784a4f8.md) **>** [**Private**](dir_4591091c161a59a7c245ad7688ad7744.md) **>** [**Vector3.cpp**](_vector3_8cpp.md)

[Go to the documentation of this file](_vector3_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Math/Public/Vector3.h"
#include "Math/Public/Vector2.h"
#include "Math/Public/Vector4.h"

namespace AGE {
Vector3::Vector3() {
        x = 0;
        y = 0;
        z = 0;
    }
Vector3::Vector3(float a, float b, float c) {
        x = a;
        y = b;
        z = c;
    }
Vector3::Vector3(Vector2 a, float c)
    {
        x = a.x;
        y = a.x;
        z = c;
    }
Vector3::Vector3(glm::vec3 v)
    {
        x = v.x;
        y = v.y;
        z = v.z;
    }

    //Including Vector4.h will cause compiler issues because of recursion, so....
    //Convoluted, but, it'll work.
    COMMENT:
CONFIDENCE: 1.0;

Vector3::Vector3(Vector4 v)
    {
        x = v.x;
        y = v.y;
        z = v.z;
    }

    //void Vector3::Serialize(DataWriter *Serializer, const Vector3 &Instance)
    //{
    //  Serializer->WriteRaw<float>(Instance.x);
    //  Serializer->WriteRaw<float>(Instance.y);
    //  Serializer->WriteRaw<float>(Instance.z);
    //}
//
    //void Vector3::Deserialize(DataReader *Serializer, Vector3 &Instance)
    //{
    //  Serializer->ReadRaw<float>(Instance.x);
    //  Serializer->ReadRaw<float>(Instance.y);
    //  Serializer->ReadRaw<float>(Instance.z);
    //}

Vector3::Vector3(float a) {
        x = a;
        y = a;
        z = a;
    }

Vector3 Vector3::normalize() const {
        float magnitude = this->magnitude();
        if (magnitude == 0) {
            return Vector3(0, 0, 0);
        }

        return Vector3(x, y, z) / magnitude;
    }

}
```


