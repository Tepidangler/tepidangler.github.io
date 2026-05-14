

# File ScriptableEntity.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Scene**](dir_2169a406ec11cf5f5db2240313483342.md) **>** [**Public**](dir_fb54e21640a292d6294e6bc8d6d36acc.md) **>** [**ScriptableEntity.h**](_scriptable_entity_8h.md)

[Go to the documentation of this file](_scriptable_entity_8h.md)


```C++

#pragma once
#include "Scene/Public/Entity.h"
#include "Structs/Public/Functions.h"
#include <rttr/type>
#ifdef __clang__
#pragma clang diagnostic push
#ifdef AG_PLATFORM_LINUX
#pragma clang diagnostic ignored "-Wunused-function"
#endif
#include "rttr/registration_friend.h"
#pragma clang diagnostic pop
#elif defined(__GNUC__)
#pragma GCC diagnostic push
#pragma clang diagnostic ignored "-Wunused-function"
#include "rttr/registration_friend.h"
#pragma GCC diagnostic pop
#elif defined(_MSC_VER)
#pragma warning(push, 0)
#include "rttr/registration_friend.h"
#pragma warning(pop)
#else
#error "Compiler is not supported with AGE yet"
#endif



namespace AGE
{
    enum class MetaDataType
    {
        Scriptable,
    };
    struct AGENode;

    class ScriptableEntity : public std::enable_shared_from_this<ScriptableEntity>
    {
    public:

        vi
rtual ~S
criptableEntity() {};

        vi
rtual bo
ol IsCharacter()
        {
            return GetScriptableEntityType() == "Character";
        }
        template<typename T>
        T&
 GetComponent()
        {
            return m_Entity.GetComponent<T>();
        }

        template<typename T, typename ... Args>
        T&
 AddComponent(Args&& ... args)
        {
            return m_Entity.AddComponent<T>();
        }

        vi
rtual st
d::string GetScriptableEntityType() { return ""; }
        virtual void OnEvent(Event& E) {};
        vi
rtual vo
id OnOverlapStart() {}
        vi
rtual vo
id OnOverlapStop() {}
        vi
rtual vo
id OnHit() {}

        virtual void AddBeginPlayFunctions(AGEFunction< AGENode, ScriptableEntity> Func) {};
        virtual void AddTickFunctions(AGEFunction< AGENode, ScriptableEntity> Func) {};

        virtual void ClearFunctions() {};
        vi
rtual st
d::string GetName() { return ""; };
        viCOMMENT:
CONFIDENCE: 1.0;

rt
ual Vector3 GetLocation() { return {}; }
        vi
rtual vo
id SetLocation(const AGE::Vector3& Location) {}

        vi
rtual UU
ID GetID() { return m_Entity.GetUUID(); }

    protected:
        virtual void OnCreate() {};
        virtual void OnBeginPlay() {};
        virtual void OnDestroy() {};
        virtual void OnUpdate(TimeStep DeltaTime) {};
        virtual void Reset() {};
        vi
rtual En
tity& GetEntityHandle() { return m_Entity; }
        virtual void PushComp();

    private:
        Entity m_Entity;
        friend class Scene;
        RTTR_ENABLE()
        RTTR_REGISTRATION_FRIEND
    };
}
```


