

# File Entity.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Scene**](dir_2169a406ec11cf5f5db2240313483342.md) **>** [**Private**](dir_3322a6c7c8fa5303912ba19015d19cce.md) **>** [**Entity.cpp**](_entity_8cpp.md)

[Go to the documentation of this file](_entity_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Scene/Public/Entity.h"


namespace AGE
{
    Entity::Entity(entt::entity Handle, Scene* ScenePtr)
        :m_EntityHandle(Handle), m_Scene(ScenePtr)
    {
    }
}
```


