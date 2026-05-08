

# File Widget.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Public**](dir_22621ac137e3b40d7111b7a349592295.md) **>** [**Widget.h**](_widget_8h.md)

[Go to the documentation of this file](_widget_8h.md)


```C++
//
// Created by gdmgp on 12/3/2025.
//

#ifndef AGE2D_WIDGET_H
#define AGE2D_WIDGET_H
#include "Core/Public/Core.h"
#include "Serializers/Public/DataReader.h"
#include "Serializers/Public/DataWriter.h"
namespace AGE
{
    class ScriptableWidget;

    struct Widget
    {
        static void Serialize(DataWriter* Serializer, const Widget& Data)
        {

        }

        static void Deserialize(DataReader* Serializer, Widget& Data)
        {

        }

        ScriptableWidget* Instance = nullptr;
        ScriptableWidget* (*InstantiateScript)();
        void (*DestroyScript)(Widget*);

        template<typename T>
        void Bind()
        {
            InstantiateScript = []() {return static_cast<ScriptableWidget*>(new T()); };
            DestroyScript = [](Widget* WC) {delete WC->Instance; WC->Instance = nullptr; };
        }

    };
} // AGE

#endif //AGE2D_WIDGET_H
```


