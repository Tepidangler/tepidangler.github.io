

# Class AGE::SquirrelRNG



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  int | [**GetCurrentPosition**](#function-getcurrentposition) () <br> |
|  uint32\_t | [**GetSeed**](#function-getseed) () <br> |
|  void | [**Init**](#function-init) (uint32\_t Seed=0) <br> |
|  void | [**ResetSeed**](#function-resetseed) (uint32\_t Seed, int Position=0) <br> |
|  uint8\_t | [**RollRandomByte**](#function-rollrandombyte) () <br> |
|  bool | [**RollRandomChance**](#function-rollrandomchance) (float ProbabilityofReturnTrue) <br> |
|  void | [**RollRandomDirection2D**](#function-rollrandomdirection2d) (float & out\_x, float & out\_y) <br> |
|  float | [**RollRandomFloatInRange**](#function-rollrandomfloatinrange) (float MinValueInclusive, float MaxValueInclusive) <br> |
|  float | [**RollRandomFloatZeroToOne**](#function-rollrandomfloatzerotoone) () <br> |
|  int | [**RollRandomIntInRange**](#function-rollrandomintinrange) (int MinValueInclusive, int MaxValueInclusive) <br> |
|  uint32\_t | [**RollRandomIntLessThan**](#function-rollrandomintlessthan) (uint32\_t MaxValueNotInclusive) <br> |
|  float | [**RollRandomRotationFloat**](#function-rollrandomrotationfloat) () <br> |
|  uint16\_t | [**RollRandomUint16**](#function-rollrandomuint16) () <br> |
|  uint32\_t | [**RollRandomUint32**](#function-rollrandomuint32) () <br> |
|  void | [**SetCurrentPosition**](#function-setcurrentposition) (int Position) <br> |


























## Public Static Functions Documentation




### function GetCurrentPosition 

```C++
static inline int AGE::SquirrelRNG::GetCurrentPosition () 
```




<hr>



### function GetSeed 

```C++
static inline uint32_t AGE::SquirrelRNG::GetSeed () 
```




<hr>



### function Init 

```C++
static void AGE::SquirrelRNG::Init (
    uint32_t Seed=0
) 
```




<hr>



### function ResetSeed 

```C++
static inline void AGE::SquirrelRNG::ResetSeed (
    uint32_t Seed,
    int Position=0
) 
```




<hr>



### function RollRandomByte 

```C++
static uint8_t AGE::SquirrelRNG::RollRandomByte () 
```




<hr>



### function RollRandomChance 

```C++
static bool AGE::SquirrelRNG::RollRandomChance (
    float ProbabilityofReturnTrue
) 
```




<hr>



### function RollRandomDirection2D 

```C++
static void AGE::SquirrelRNG::RollRandomDirection2D (
    float & out_x,
    float & out_y
) 
```




<hr>



### function RollRandomFloatInRange 

```C++
static float AGE::SquirrelRNG::RollRandomFloatInRange (
    float MinValueInclusive,
    float MaxValueInclusive
) 
```




<hr>



### function RollRandomFloatZeroToOne 

```C++
static float AGE::SquirrelRNG::RollRandomFloatZeroToOne () 
```




<hr>



### function RollRandomIntInRange 

```C++
static int AGE::SquirrelRNG::RollRandomIntInRange (
    int MinValueInclusive,
    int MaxValueInclusive
) 
```




<hr>



### function RollRandomIntLessThan 

```C++
static uint32_t AGE::SquirrelRNG::RollRandomIntLessThan (
    uint32_t MaxValueNotInclusive
) 
```




<hr>



### function RollRandomRotationFloat 

```C++
static float AGE::SquirrelRNG::RollRandomRotationFloat () 
```




<hr>



### function RollRandomUint16 

```C++
static uint16_t AGE::SquirrelRNG::RollRandomUint16 () 
```




<hr>



### function RollRandomUint32 

```C++
static uint32_t AGE::SquirrelRNG::RollRandomUint32 () 
```




<hr>



### function SetCurrentPosition 

```C++
static inline void AGE::SquirrelRNG::SetCurrentPosition (
    int Position
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/RNG/Public/RNG.h`

