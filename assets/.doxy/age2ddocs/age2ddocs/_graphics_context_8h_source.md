

# File GraphicsContext.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Render**](dir_bf2ed8d341b54e9ac186cdc667978d77.md) **>** [**Public**](dir_68ba7e1260de504efb39109a85960357.md) **>** [**GraphicsContext.h**](_graphics_context_8h.md)

[Go to the documentation of this file](_graphics_context_8h.md)


```C++
#pragma once
#ifdef AG_PLATFORM_WINDOWS
#include "d3d11_4.h"
#endif
#include "Structs/Public/DataStructures.h"

namespace AGE
{
    class GraphicsContext
    {
    public:
        
virtual ~GraphicsContext() {}
        virtual void Init() = 0;

        virtual void SwapBuffers() = 0;

        static Scope<GraphicsContext> Create(void* Window);

        template<typename T>
        T* As();
    };

}
```


