

# File InputBinding.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Private**](dir_d65e1b3fe96e0227a21781a1e5bc67b7.md) **>** [**InputBinding.cpp**](_input_binding_8cpp.md)

[Go to the documentation of this file](_input_binding_8cpp.md)


```C++
//
// Created by gdmgp on 3/13/2026.
//
#include "AGEpch.hpp"
#include "Core/Public/InputBinding.h"

namespace AGE
{
    Ref<InputBinding> InputBinding::CreateGamepadBinding(const std::string_view& Name, GamePad::Buttons button, Binding::Type bindingtype)
    {
        if (button != GamePad::Buttons::INVALID)
        {
            return CreateRef<GamepadInputBinding>(Name,button, bindingtype);
        }
            return CreateRef<GamepadInputBinding>(Name, bindingtype);
    }

    Ref<InputBinding> InputBinding::CreateGamepadBinding(const std::string_view &Name, GamePad::Axes axes,
        Binding::Type bindingtype)
    {
        if (axes != GamePad::Axes::INVALIDAXES)
        {
            return CreateRef<GamepadInputBinding>(Name,axes, bindingtype);
        }
        return CreateRef<GamepadInputBinding>(Name, bindingtype);
    }

    Ref<InputBinding> InputBinding::CreateKBMBinding(const std::string_view& Name, Key::Keys keycode, Binding::Type bindingtype)
    {
        if (keycode != Key::INVALID)
        {
            return CreateRef<KBMInputBinding>(Name, keycode, bindingtype);
        }
            return CreateRef<KBMInputBinding>(Name, bindingtype);
    }

    Ref<InputBinding> InputBinding::CreateInvalid()
    {
        return CreateRef<InvalidInputBinding_t>();
    }
} // AGE
```


