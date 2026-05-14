

# File Core.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Core.h**](_core_8h.md)

[Go to the documentation of this file](_core_8h.md)


```C++
#pragma once
#include <memory>
#include <string>
#include <filesystem>
#include <any>
#include "Core/Public/Log.h"

#ifdef AG_PLATFORM_WINDOWS
#if AG_DYNAMIC_LINK

    #ifdef AG_BUILD_DLL
        #define AGE_API __declspec(dllexport)
    #else
        #define AGE_API __declspec(dllimport)
    #endif
#else
    #define AGE_API
    #undef AKSOUNDENGINE_DLL
#endif
#endif

#ifdef AG_PLATFORM_LINUX
#if AG_DYNAMIC_LINK

    #ifdef AG_BUILD_DLL
        #define AGE_API __declspec(dllexport)
    #else
        #define AGE_API __declspec(dllimport)
    #endif
#else
    #define AGE_API
    #undef AKSOUNDENGINE_DLL
#endif
#endif

#if !defined(AG_PLATFORM_LINUX) && !defined(AG_PLATFORM_WINDOWS)
#error AGE only supports Windows and Linux!
#endif

#if AG_DEBUG
    #define AGE_ENABLE_ASSERTS
//  #pragma enable_d3d11_debug_symbols
#endif

#if AG_DIST
    #define AK_OPTIMIZED
#endif


#define BIND_EVENT_FN(x) std::bind(&x, this, std::placeholders::_1)
#define BIND_AXIS_FN(x) std::bind(&x, this, std::placeholders::_1)
#define BIND_ACTION_FN(x) std::bind(&x, this)

#define BIT(x) (1 << x)
namespace AGE
{
    typedef unsigned long ulong_t;



    template<typename T>
    class Reverse
    {
    private:
        T& iterable_;

    public:
explicit Reverse(T& iterable) : iterable_{ iterable } {}
auto begin() const { return std::rbegin(iterable_); }
        COMMENT:
CONFIDENCE: 1.0;

auto end() const { return std::rend(iterable_); }
    };
}

namespace GameFramework
{

}
```


