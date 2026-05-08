

# File UIStructs.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**UI**](dir_c71f946845db44b77b26d47f3af3494b.md) **>** [**Public**](dir_22621ac137e3b40d7111b7a349592295.md) **>** [**UIStructs.h**](_u_i_structs_8h.md)

[Go to the documentation of this file](_u_i_structs_8h.md)


```C++
//
// Created by gdmgp on 12/29/2025.
//

#ifndef AGE2D_UISTRUCTS_H
#define AGE2D_UISTRUCTS_H

#include <string>
#include "Core/Public/Core.h"
#include "Math/Public/Vector3.h"
#include "Math/Public/Vector4.h"
#include "Texture/Public/Texture.h"

namespace AGE
{
    template<typename ... Callable>
    struct UIVisitor : Callable...
    {
        using Callable::operator()...;
    };

    struct UIComponentType
    {
        enum Value : uint16_t
        {
            TextComponent,TextBoxComponent,
            HorizontalBoxComponent,VerticalBoxComponent,
            ButtonComponent,
            ImageComponent
        };

        UIComponentType() = default;
         UIComponentType(Value Val)
            : value(Val)
        {
            Name = ToString(value);

        }

        constexpr operator Value() const {return value;}

        explicit operator bool() const = delete;

        constexpr bool operator==(UIComponentType a) const
        {
            return value == a.value;
        }

        constexpr bool operator!=(UIComponentType a) const
        {
            return value != a.value;
        }

        operator std::string()  const
        {
            return Name;
        }
        std::string operator()(Value Val)  const
        {
            return ToString(Val);
        }

        Value ToValue()
        {
            return value;
        }
        Value ToValue() const
        {
            return value;
        }

        std::string& ToString()
        {
            return Name;
        }

        std::string ToString() const
        {
            return Name;
        }

        std::string ToString(Value Val)
        {
            switch(Val)
            {
                case TextComponent:
                {
                    return "TextComponent";
                    break;
                }
                case TextBoxComponent:
                {
                    return "TextBoxComponent";
                    break;
                }
                case HorizontalBoxComponent: {
                    return "HorizontalBoxComponent";
                    break;
                }
                case VerticalBoxComponent: {
                    return "VerticalBoxComponent";
                    break;
                }
                case ButtonComponent: {
                    return "ButtonComponent";
                    break;
                }
                case ImageComponent: {
                    return "ImageComponent";
                    break;
                }
                default:
                {
                    break;
                }
            }

            return std::string();
        }

        std::string ToString(Value Val) const
        {
            switch(Val)
            {
                case TextComponent:
                {
                    return "TextComponent";
                    break;
                }
                case TextBoxComponent:
                {
                    return "TextBoxComponent";
                    break;
                }
                case HorizontalBoxComponent: {
                    return "HorizontalBoxComponent";
                    break;
                }
                case VerticalBoxComponent: {
                    return "VerticalBoxComponent";
                    break;
                }
                case ButtonComponent: {
                    return "ButtonComponent";
                    break;
                }
                case ImageComponent: {
                    return "ImageComponent";
                    break;
                }
                default:
                {
                    break;
                }
            }
            return std::string();

        }

        static void Serialize(DataWriter* Serializer, const UIComponentType& Instance)
        {
            Serializer->WriteString(Instance.Name);
            Serializer->WriteRaw<uint16_t>(Instance.value);
        }

        static void Deserialize(DataReader* Serializer, UIComponentType& Instance)
        {
            Serializer->ReadString(Instance.Name);
            Serializer->ReadRaw<Value>(Instance.value);
        }


    private:
        Value value;
        std::string Name = "";
    };

    struct UIProperties
    {
        UIProperties() = default;
        Vector3 Position = Vector3(0.f);
        Vector3 Rotation = Vector3(0.f);
        Vector3 Scale = Vector3(1.f);
        bool Visible = true;
        bool Focused = false;
    };

    struct BoxProperties
    {
        BoxProperties() = default;
        Vector3 Position = Vector3(0.f);
        Vector3 Rotation = Vector3(0.f);
        Vector3 Scale = Vector3(1.f);
        Vector4 TintColor = {1.f};
        Ref<Texture> BoxTexture = nullptr;
    };
}
#endif //AGE2D_UISTRUCTS_H
```


