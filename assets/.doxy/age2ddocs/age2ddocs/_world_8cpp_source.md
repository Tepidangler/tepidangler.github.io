

# File World.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Physics**](dir_0200296fe7041373e4c6a62f3844ed95.md) **>** [**Private**](dir_aa1a9f4b85cc4e4a5149e0c99c6c45ae.md) **>** [**World.cpp**](_world_8cpp.md)

[Go to the documentation of this file](_world_8cpp.md)


```C++


#include "AGEpch.hpp"
#include "Physics/Public/World.h"
#include "Physics/Public/World2D.h"

namespace AGE
{
    Re
f<World> World::Create(Ref<Scene> scene)
    {
        return CreateRef<World2D>(scene);
    }

    template<typename T>
    T*
 World::As()
    {
        CoreLogger::Assert(false, "As() Failed!");
        return nullptr;
    }
}
```


