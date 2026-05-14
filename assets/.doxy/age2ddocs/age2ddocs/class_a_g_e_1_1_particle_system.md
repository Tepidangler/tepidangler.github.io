

# Class AGE::ParticleSystem



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ParticleSystem**](class_a_g_e_1_1_particle_system.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Emit**](#function-emit) (const [**ParticleProps**](struct_a_g_e_1_1_particle_props.md) & Properties) <br>_Emit a new particle with the given properties._  |
|  void | [**OnRender**](#function-onrender) (const [**Camera**](class_a_g_e_1_1_camera.md) & Camera, const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform) <br> |
|  void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function updates the state of each particle in the system over a given time step._  |
|   | [**ParticleSystem**](#function-particlesystem) (uint32\_t MaxParticles=100000) <br>_Constructs a_ [_**ParticleSystem**_](class_a_g_e_1_1_particle_system.md) _object with the specified maximum number of particles._ |




























## Public Functions Documentation




### function Emit 

_Emit a new particle with the given properties._ 
```C++
void AGE::ParticleSystem::Emit (
    const ParticleProps & Properties
) 
```



This function creates a new particle and initializes its properties based on the provided [**ParticleProps**](struct_a_g_e_1_1_particle_props.md) object. The position, rotation, velocity, color, lifetime, size of the particle are set according to the values in the [**ParticleProps**](struct_a_g_e_1_1_particle_props.md) object.




**Parameters:**


* `particleProps` Properties for the new particle.

Emits a new particle with given properties.


This function creates a new particle and initializes its properties based on the provided [**ParticleProps**](struct_a_g_e_1_1_particle_props.md) object. The position, rotation, velocity, color, lifetime, size of the particle are set according to the values in the [**ParticleProps**](struct_a_g_e_1_1_particle_props.md) object. The particle is then added to the pool of particles.




**Parameters:**


* `particleProps` Properties for the new particle. 




        

<hr>



### function OnRender 

```C++
void AGE::ParticleSystem::OnRender (
    const Camera & Camera,
    const Matrix4D & Transform
) 
```




<hr>



### function OnUpdate 

_This function updates the state of each particle in the system over a given time step._ 
```C++
void AGE::ParticleSystem::OnUpdate (
    TimeStep DeltaTime
) 
```



The function iterates through all particles in the system and performs several operations on them based on their current state. If a particle is not active, it will be skipped. For active particles, if their life remaining is less than or equal to zero, they are deactivated. Otherwise, their lifespan is reduced by the time step and their position is updated by adding their velocity times the time step. The rotation of the particle remains unaffected in this case.




**Parameters:**


* `ts` The time step over which to update the particles.

This function updates the state of each particle in the system over a given time step.


The function iterates through all particles in the pool and performs several operations on them based on their current status. If a particle is not active, it is skipped. For active particles, if their life remaining is less than or equal to zero, they are deactivated. Otherwise, their lifespan is reduced by the time step size, and their position is updated by adding their velocity times the time step size. The rotation of each particle also increases over time.




**Parameters:**


* `ts` The duration of the time step for which the particles should be updated. 




        

<hr>



### function ParticleSystem 

_Constructs a_ [_**ParticleSystem**_](class_a_g_e_1_1_particle_system.md) _object with the specified maximum number of particles._
```C++
AGE::ParticleSystem::ParticleSystem (
    uint32_t MaxParticles=100000
) 
```



This constructor initializes the particle pool to the given size and sets up the random number generator for the indices. The m\_PoolIndex is initialized as MaxParticles - 1, ensuring that the first call to GetNextFreeParticle() will return 0. 

**Parameters:**


* `MaxParticles` The maximum number of particles that can be stored in the particle pool.

Constructs a [**ParticleSystem**](class_a_g_e_1_1_particle_system.md) object with the specified maximum number of particles.


Initializes the particle pool to the given size and sets up the random number generator for the indices.




**Parameters:**


* `MaxParticles` The maximum number of particles that can be in the system at any one time. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Particles/Public/ParticleSystem.h`

