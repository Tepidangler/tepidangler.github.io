

# Class AGE::SquirrelNoise



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**Get1dNoiseForRotation**](#function-get1dnoiseforrotation) (int Rotation, uint32\_t Seed=0) <br>_Same Functions, mapped to floats in [-180,180]._  |
|  float | [**Get1dNoiseNegOneToOne**](#function-get1dnoisenegonetoone) (int Position, uint32\_t Seed=0) <br>_Same Functions, mapped to floats in [-1,1]._  |
|  uint32\_t | [**Get1dNoiseUint**](#function-get1dnoiseuint) (int Position, uint32\_t Seed=0) <br> |
|  float | [**Get1dNoiseZeroToOne**](#function-get1dnoisezerotoone) (int Position, uint32\_t Seed=0) <br> |
|  float | [**Get2dNoiseNegOneToOne**](#function-get2dnoisenegonetoone) (int PositionX, int PositionY, uint32\_t Seed=0) <br> |
|  uint32\_t | [**Get2dNoiseUint**](#function-get2dnoiseuint) (int PositionX, int PositionY, uint32\_t Seed=0) <br> |
|  float | [**Get2dNoiseZeroToOne**](#function-get2dnoisezerotoone) (int PositionX, int PositionY, uint32\_t Seed=0) <br> |
|  float | [**Get3dNoiseNegOneToOne**](#function-get3dnoisenegonetoone) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br> |
|  uint32\_t | [**Get3dNoiseUint**](#function-get3dnoiseuint) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br> |
|  float | [**Get3dNoiseZeroToOne**](#function-get3dnoisezerotoone) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br> |
|  float | [**Get4dNoiseNegOneToOne**](#function-get4dnoisenegonetoone) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br> |
|  uint32\_t | [**Get4dNoiseUint**](#function-get4dnoiseuint) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br> |
|  float | [**Get4dNoiseZeroToOne**](#function-get4dnoisezerotoone) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br> |
|  uint32\_t | [**Rand**](#function-rand) () <br> |
|   | [**SquirrelNoise**](#function-squirrelnoise) () <br> |




























## Public Functions Documentation




### function Get1dNoiseForRotation 

_Same Functions, mapped to floats in [-180,180]._ 
```C++
float AGE::SquirrelNoise::Get1dNoiseForRotation (
    int Rotation,
    uint32_t Seed=0
) 
```




<hr>



### function Get1dNoiseNegOneToOne 

_Same Functions, mapped to floats in [-1,1]._ 
```C++
float AGE::SquirrelNoise::Get1dNoiseNegOneToOne (
    int Position,
    uint32_t Seed=0
) 
```




<hr>



### function Get1dNoiseUint 

```C++
uint32_t AGE::SquirrelNoise::Get1dNoiseUint (
    int Position,
    uint32_t Seed=0
) 
```




<hr>



### function Get1dNoiseZeroToOne 

```C++
float AGE::SquirrelNoise::Get1dNoiseZeroToOne (
    int Position,
    uint32_t Seed=0
) 
```




<hr>



### function Get2dNoiseNegOneToOne 

```C++
float AGE::SquirrelNoise::Get2dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```




<hr>



### function Get2dNoiseUint 

```C++
uint32_t AGE::SquirrelNoise::Get2dNoiseUint (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```




<hr>



### function Get2dNoiseZeroToOne 

```C++
float AGE::SquirrelNoise::Get2dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```




<hr>



### function Get3dNoiseNegOneToOne 

```C++
float AGE::SquirrelNoise::Get3dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```




<hr>



### function Get3dNoiseUint 

```C++
uint32_t AGE::SquirrelNoise::Get3dNoiseUint (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```




<hr>



### function Get3dNoiseZeroToOne 

```C++
float AGE::SquirrelNoise::Get3dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```




<hr>



### function Get4dNoiseNegOneToOne 

```C++
float AGE::SquirrelNoise::Get4dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```




<hr>



### function Get4dNoiseUint 

```C++
uint32_t AGE::SquirrelNoise::Get4dNoiseUint (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```




<hr>



### function Get4dNoiseZeroToOne 

```C++
float AGE::SquirrelNoise::Get4dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```




<hr>



### function Rand 

```C++
uint32_t AGE::SquirrelNoise::Rand () 
```




<hr>



### function SquirrelNoise 

```C++
AGE::SquirrelNoise::SquirrelNoise () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/RNG/Public/RNG.h`

