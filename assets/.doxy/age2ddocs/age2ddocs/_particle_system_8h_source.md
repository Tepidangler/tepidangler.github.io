

# File ParticleSystem.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Particles**](dir_d5e6827e04ca3e5dc26c1a2d53d43bf9.md) **>** [**Public**](dir_de24c6887d7bea99649d1ef2e929b7b9.md) **>** [**ParticleSystem.h**](_particle_system_8h.md)

[Go to the documentation of this file](_particle_system_8h.md)


```C++
#pragma once
#include <glm/glm.hpp>

#include "Core/Public/DeltaTime.h"
#include "Camera/Public/Camera.h"
#include "Math/Public/MathStructures.h"
#include "Math/Public/UtilityFunctions.h"

namespace AGE
{
    struct ParticleProps
    {
        Vector3 Position;
        Vector3 Velocity;
        Vector3 VelocityVariation;
        Vector4 ColorBegin;
        Vector4 ColorEnd;

        float SizeBegin;
        float SizeEnd;
        float SizeVariation;
        float LifeTime = 1.f;
    };

    class ParticleSystem
    {
    public:
        ParticleSystem(uint32_t MaxParticles = 100000);

        void OnUpdate(TimeStep DeltaTime);
        void OnRender(const Camera& Camera, const Matrix4D& Transform);

        void Emit(const ParticleProps& Properties);



    private:

        struct Particle : public QuadProperties
        {
            Vector3 Position;
            Vector3 Velocity;
            Vector4 ColorBegin;
            Vector4 ColorEnd;
            float Rotation = 0.f;
            float SizeBegin;
            float SizeEnd;

            float LifeTime = 1.f;
            float LifeRemaining = 0.f;

            bool Active = false;
            
        };

        std::vector<Particle> m_ParticlePool;

        uint32_t m_PoolIndex ;
    };
}
```


