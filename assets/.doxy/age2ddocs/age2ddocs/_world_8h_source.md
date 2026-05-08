

# File World.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Physics**](dir_0200296fe7041373e4c6a62f3844ed95.md) **>** [**Public**](dir_384ddce68b480931e8586b1cf8a80838.md) **>** [**World.h**](_world_8h.md)

[Go to the documentation of this file](_world_8h.md)


```C++
#pragma once
#include "Core/Public/Core.h"
#include <box2d/box2d.h>
#include "Scene/Public/Scene.h"


namespace AGE
{
    class World
    {
    public:
        virtual void DestroyWorld() = 0;

        virtual void Step(TimeStep DeltaTime) = 0;

        virtual void MakeDefaultQueryFilter() = 0;
        virtual void QueryBoxOverlap(const QueryParams& Params) = 0;
        virtual void QueryCapsuleOverlap(const QueryParams& Params) = 0;
        virtual void QuerySegmentOverlap(const QueryParams& Params) = 0;
        virtual void QueryHit(const QueryParams& Params) = 0;
        template<typename T>
        T* As();

        static Ref<World> Create(Ref<Scene> scene);


    };
}
```


