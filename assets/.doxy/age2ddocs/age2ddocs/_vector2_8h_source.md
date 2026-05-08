

# File Vector2.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Math**](dir_5b9993be36110f29e6abf37e5784a4f8.md) **>** [**Public**](dir_6835e5d20dff99344f151a9056e5ca16.md) **>** [**Vector2.h**](_vector2_8h.md)

[Go to the documentation of this file](_vector2_8h.md)


```C++
#ifndef VECTOR2_H
#define VECTOR2_H
#endif // !VECTOR2_H

#include <cmath>
#include <glm/glm.hpp>
#include <sstream>
#pragma once

namespace AGE {
    struct Vector2
    {
    public:
        
        float x, y;
        

        Vector2();
        explicit Vector2(float a);
        Vector2(float a, float b);
        Vector2(const Vector2& Other)
        {
            x = Other.x;
            y = Other.y;
        }

        Vector2& operator=(const Vector2& Other)
        {
            x = Other.x;
            y = Other.y;
            return *this;
        }

        float dot(const Vector2& vec) const {
            float product = (x * vec.x) + (y * vec.y);
            return product;
        }

        float norm(const Vector2& vec) const {
            float magnitude = sqrtf(powf((x - vec.x), 2.f) + powf((y - vec.y), 2.f));

            return magnitude;
        }

        float magnitude() const {
            return norm(Vector2());
        }

        Vector2 normalize() const;

        float& operator [](int i)
        {
            return ((&x)[i]);
        }

        const float& operator [](int i) const
        {
            return ((&x)[i]);
        }

        Vector2 operator+(const Vector2& vec) const {
            return Vector2(x + vec.x, y + vec.y);
        }

        void operator+=(const Vector2& vec) {
            x += vec.x;
            y += vec.y;
        }

        Vector2 operator-(const Vector2& vec) const {
            return Vector2(x - vec.x, y - vec.y);
        }
        Vector2 operator-(const float val) const {
            return Vector2(x - val, y - val);
        }


        void operator-=(const Vector2& vec) {
            x -= vec.x;
            y -= vec.y;
        }

        Vector2 operator*(float scalar) const {
            return Vector2(x * scalar, y * scalar);
        }

        void operator*=(float scalar) {
            x *= scalar;
            y *= scalar;
        }

        Vector2 operator/(float scalar) const {
            return Vector2(x / scalar, y / scalar);
        }

        Vector2 operator/(const Vector2& vec) const {
            return Vector2(x / vec.x, y / vec.y);
        }

        void operator/=(float scalar) {
            x /= scalar;
            y /= scalar;
        }

        bool operator==(const Vector2& vec) const {
            return x == vec.x && y == vec.y;
        }

        bool operator!=(const Vector2& vec) const {
            return x != vec.x || y != vec.y;
        }

        operator std::string()
        {
            std::stringstream SS;

            SS << "X: " << x << " Y: " << y << '\n';

            return SS.str();
        }

        operator glm::vec2() const
        {
            return {x,y};
        }
    };


}


```


