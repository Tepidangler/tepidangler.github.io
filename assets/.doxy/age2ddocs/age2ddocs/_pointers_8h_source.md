

# File Pointers.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Pointers.h**](_pointers_8h.md)

[Go to the documentation of this file](_pointers_8h.md)


```C++
//
// Created by gdmgp on 2/8/2026.
//
#pragma once
#include <memory>
#ifndef AGE2D_POINTERS_H
#define AGE2D_POINTERS_H
namespace AGE {

    template<typename T>
    using Scope = std::unique_ptr<T>;

    template<typename T, typename ... Args>
constexpr Scope<T> CreateScope(Args&& ... args)
    {
        return std::make_unique<T>(std::forward<Args>(args)...);
    }
    template<typename T>
    using Ref = std::shared_ptr<T>;

    template<typename T, typename ... Args>
constexpr Ref<T> CreateRef(Args&& ... args)
    {
        return std::make_shared<T>(std::forward<Args>(args)...);
    };

    template<typename To, typename From, typename Deleter>
std::unique_ptr<To, Deleter> dynamic_unique_cast(std::unique_ptr<From, Deleter>&& p)
    {
        if (To* cast = dynamic_cast<To*>(p.get()))
        {
            std::unique_ptr<To, Deleter> result(cast, std::move(p.get_deleter()));
            p.release();
            return result;
        }
        //CoreLogger::Error("Cast Failed!");
        return std::unique_ptr<To, Deleter>(nullptr);
    }

    template<typename T>
inline void SafeRelease(T& ptr)
    {
        if (ptr != NULL)
        {
            ptr->Release();
            ptr = nullptr;
        }
    }

    //TODO: Implement Intruisive Ptr
}
#endif //AGE2D_POINTERS_H
```


