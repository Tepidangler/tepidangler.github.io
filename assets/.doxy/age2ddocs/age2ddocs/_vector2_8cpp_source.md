

# File Vector2.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Math**](dir_5b9993be36110f29e6abf37e5784a4f8.md) **>** [**Private**](dir_4591091c161a59a7c245ad7688ad7744.md) **>** [**Vector2.cpp**](_vector2_8cpp.md)

[Go to the documentation of this file](_vector2_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Math/Public/Vector2.h"

namespace AGE {
    Vector2::Vector2() {
        x = 0;
        y = 0;
    }
    Vector2::Vector2(float a, float b) {
        x = a;
        y = b;
    }
    Vector2::Vector2(float a) {
        x = a;
        y = a;
    }

    Vector2 Vector2::normalize() const {
        float magnitude = this->magnitude();
        if (magnitude == 0) {
            return Vector2(0, 0);
        }

        return Vector2(x, y) / magnitude;
    }

}
```


