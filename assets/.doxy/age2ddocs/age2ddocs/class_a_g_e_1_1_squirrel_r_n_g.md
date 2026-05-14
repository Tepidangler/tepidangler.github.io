

# Class AGE::SquirrelRNG



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  int | [**GetCurrentPosition**](#function-getcurrentposition) () <br>_This function returns the current position value stored in 's\_Position'._  |
|  uint32\_t | [**GetSeed**](#function-getseed) () <br>_This function returns the current seed value used for random number generation._  |
|  void | [**Init**](#function-init) (uint32\_t Seed=0) <br>_Initializes the_ [_**SquirrelRNG**_](class_a_g_e_1_1_squirrel_r_n_g.md) _with a given seed._ |
|  void | [**ResetSeed**](#function-resetseed) (uint32\_t Seed, int Position=0) <br>_Resets the seed and position for a pseudo-random number generator._  |
|  uint8\_t | [**RollRandomByte**](#function-rollrandombyte) () <br>_Generates a random byte using the Squirrel RNG algorithm._  |
|  bool | [**RollRandomChance**](#function-rollrandomchance) (float ProbabilityofReturnTrue) <br>_This function rolls a random chance based on the given probability._  |
|  void | [**RollRandomDirection2D**](#function-rollrandomdirection2d) (float & out\_x, float & out\_y) <br>_RollRandomDirection2D generates a random direction in two dimensions._  |
|  float | [**RollRandomFloatInRange**](#function-rollrandomfloatinrange) (float MinValueInclusive, float MaxValueInclusive) <br>_RollRandomFloatInRange generates a random float within the specified range._  |
|  float | [**RollRandomFloatZeroToOne**](#function-rollrandomfloatzerotoone) () <br>_This function generates a random float between 0 and 1._  |
|  int | [**RollRandomIntInRange**](#function-rollrandomintinrange) (int MinValueInclusive, int MaxValueInclusive) <br>_Generates a random integer within the specified range._  |
|  uint32\_t | [**RollRandomIntLessThan**](#function-rollrandomintlessthan) (uint32\_t MaxValueNotInclusive) <br>_Generates a random integer less than the provided maximum value._  |
|  float | [**RollRandomRotationFloat**](#function-rollrandomrotationfloat) () <br>_RollRandomRotationFloat generates a random float value for rotation. The function uses Perlin noise to generate a pseudo-random number and cast it to float. This is used as a means of generating a random float value that can be used for rotation purposes._  |
|  uint16\_t | [**RollRandomUint16**](#function-rollrandomuint16) () <br>_Generates a random uint16\_t value._  |
|  uint32\_t | [**RollRandomUint32**](#function-rollrandomuint32) () <br>_Generates a random uint32 number._  |
|  void | [**SetCurrentPosition**](#function-setcurrentposition) (int Position) <br>_Sets the current position value._  |


























## Public Static Functions Documentation




### function GetCurrentPosition 

_This function returns the current position value stored in 's\_Position'._ 
```C++
static inline int AGE::SquirrelRNG::GetCurrentPosition () 
```





**Returns:**

The integer value of the current position. If no such variable exists, it will return a default value of 0.


This function returns the current position.




**Returns:**

The integer value of the current position. If there is no such position, it will return -1. 





        

<hr>



### function GetSeed 

_This function returns the current seed value used for random number generation._ 
```C++
static inline uint32_t AGE::SquirrelRNG::GetSeed () 
```





**Returns:**

The current seed value as a uint32\_t.


This function returns the current seed value used for random number generation. 

**Returns:**

The current seed value as a uint32\_t. 





        

<hr>



### function Init 

_Initializes the_ [_**SquirrelRNG**_](class_a_g_e_1_1_squirrel_r_n_g.md) _with a given seed._
```C++
static void AGE::SquirrelRNG::Init (
    uint32_t Seed=0
) 
```



This function sets the initial seed for the random number generator and resets all other variables to their default state. The generated noise object is also created here.




**Parameters:**


* `Seed` The initial seed value for the RNG.

Initializes the [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) with a given seed.


This function sets the initial seed value for the random number generator, resets the position and rotation values to 0, creates a new instance of [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md), and assigns it to s\_NoiseObj.




**Parameters:**


* `Seed` The initial seed value for the RNG. 




        

<hr>



### function ResetSeed 

_Resets the seed and position for a pseudo-random number generator._ 
```C++
static inline void AGE::SquirrelRNG::ResetSeed (
    uint32_t Seed,
    int Position=0
) 
```



This function sets the global variables `s_Seed` and `s_Position` to the provided values. The new seed is used as the starting point for generating pseudo-random numbers, while the position indicates the current position in the sequence of generated numbers.




**Parameters:**


* `Seed` A 32-bit unsigned integer that will be used as the new seed value. 
* `Position` An optional parameter indicating the start position for generating pseudo-random numbers. Defaults to 0 if not provided. 



**Returns:**

void


Resets the seed value and position for a pseudo-random number generator.


This function sets the global variables `s_Seed` and `s_Position` to the provided values, which are used by other functions in this class for generating pseudo-random numbers.




**Parameters:**


* `Seed` The new seed value to use. 
* `Position` The new position value to use (default is 0). 




        

<hr>



### function RollRandomByte 

_Generates a random byte using the Squirrel RNG algorithm._ 
```C++
static uint8_t AGE::SquirrelRNG::RollRandomByte () 
```



This function uses the Squirrel RNG algorithm to generate a random byte. The output is deterministic and can be used for cryptographic purposes if necessary.




**Returns:**

A randomly generated uint8\_t value.


Generates a random byte using the Squirrel RNG algorithm.


This function uses the Squirrel RNG algorithm to generate a random byte. It returns a constant value of 0, as per the implementation.




**Returns:**

A randomly generated byte (uint8\_t). In this case, it always returns 0. 





        

<hr>



### function RollRandomChance 

_This function rolls a random chance based on the given probability._ 
```C++
static bool AGE::SquirrelRNG::RollRandomChance (
    float ProbabilityofReturnTrue
) 
```





**Parameters:**


* `ProbabilityofReturnTrue` The probability of returning true, should be between 0 and 1. 



**Returns:**

bool Returns true with the provided probability, false otherwise. If the input is not within [0,1], it returns false.


This function is used to roll a random chance based on the provided probability.




**Parameters:**


* `ProbabilityofReturnTrue` The probability of returning true, should be between 0 and 1.



**Returns:**

bool Returns true with the given probability, false otherwise. If the input probability is not within the range [0, 1], it will return false. 





        

<hr>



### function RollRandomDirection2D 

_RollRandomDirection2D generates a random direction in two dimensions._ 
```C++
static void AGE::SquirrelRNG::RollRandomDirection2D (
    float & out_x,
    float & out_y
) 
```



This function uses the noise object to generate two values between 0 and 1 for x and y coordinates respectively. The generated values are stored in out\_x and out\_y.




**Parameters:**


* `out_x` Reference to a float where the x coordinate will be stored. 
* `out_y` Reference to a float where the y coordinate will be stored.



**Returns:**

void


Generates a random direction in 2D space.


This function generates two random numbers using the noise object `s_NoiseObj` and assigns them to the output parameters `out_x` and `out_y`, respectively. The generated values are between 0 and 1.




**Parameters:**


* `out_x` A reference to a float that will receive the x-coordinate of the random direction. 
* `out_y` A reference to a float that will receive the y-coordinate of the random direction. 




        

<hr>



### function RollRandomFloatInRange 

_RollRandomFloatInRange generates a random float within the specified range._ 
```C++
static float AGE::SquirrelRNG::RollRandomFloatInRange (
    float MinValueInclusive,
    float MaxValueInclusive
) 
```



This function uses a [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) to generate a random float between two given values (MinValueInclusive and MaxValueInclusive). The generated number will be inclusive of both end points, meaning it could return either MinValueInclusive or MaxValueInclusive with equal probability.




**Parameters:**


* `MinValueInclusive` the lower limit of the range from which to generate a random float. 
* `MaxValueInclusive` the upper limit of the range from which to generate a random float.



**Returns:**

A random float within the specified range (MinValueInclusive, MaxValueInclusive]. The return value will be greater than or equal to MinValueInclusive and less than or equal to MaxValueInclusive with equal probability. If MinValueInclusive is greater than MaxValueInclusive, "Unknown" is returned.


Generates a random float within the specified range.


This function generates a pseudo-random floating point number between two given values (inclusive). The generated value is determined by applying noise to the current position and seed, then scaling it to fit within the provided range.




**Parameters:**


* `MinValueInclusive` The lower limit of the range from which to generate the random float. 
* `MaxValueInclusive` The upper limit of the range from which to generate the random float.



**Returns:**

A pseudo-random floating point number within the specified range. 





        

<hr>



### function RollRandomFloatZeroToOne 

_This function generates a random float between 0 and 1._ 
```C++
static float AGE::SquirrelRNG::RollRandomFloatZeroToOne () 
```



The generated number is obtained from the noise object associated with [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) class. It uses Get1dNoiseZeroToOne method of the noise object to generate the number, which takes in two parameters: current position (s\_Position) and a seed value (s\_Seed). The s\_Position is incremented after each call to this function to ensure uniqueness of the generated numbers.




**Returns:**

A float between 0 and 1 representing the random number.


This function generates a random float between 0 and 1. 

**Returns:**

A floating-point number in the range [0, 1). 





        

<hr>



### function RollRandomIntInRange 

_Generates a random integer within the specified range._ 
```C++
static int AGE::SquirrelRNG::RollRandomIntInRange (
    int MinValueInclusive,
    int MaxValueInclusive
) 
```



This function generates and returns a pseudo-random number between two given integers (inclusive). The generated number will be in the range [MinValueInclusive, MaxValueInclusive]. If MinValueInclusive &gt; MaxValueInclusive, an empty range is assumed which always returns MinValueInclusive.




**Parameters:**


* `MinValueInclusive` Lower bound of the range (inclusive). 
* `MaxValueInclusive` Upper bound of the range (inclusive).



**Returns:**

A pseudo-random integer within the specified range.


Generates a random integer within the specified range.


This function generates and returns a random integer between two given values (inclusive). The minimum value is inclusive, while the maximum value is also inclusive. If the provided min and max are equal, it will return that number as the result.




**Parameters:**


* `MinValueInclusive` The lower limit of the range from which to generate a random integer. Must be less than or equal to MaxValueInclusive. 
* `MaxValueInclusive` The upper limit of the range from which to generate a random integer. Must be greater than or equal to MinValueInclusive.



**Returns:**

A random integer within the specified range. If both min and max are equal, returns that number. 





        

<hr>



### function RollRandomIntLessThan 

_Generates a random integer less than the provided maximum value._ 
```C++
static uint32_t AGE::SquirrelRNG::RollRandomIntLessThan (
    uint32_t MaxValueNotInclusive
) 
```



This function generates a pseudo-random number using [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) algorithm, which is then returned as an unsigned 32-bit integer. The generated number will be less than the provided MaxValueNotInclusive parameter. If this value is zero or negative, the behavior of this function is undefined.




**Parameters:**


* `MaxValueNotInclusive` An unsigned 32-bit integer specifying the upper limit for the random number to be generated (exclusive). Must be greater than zero. 



**Returns:**

A pseudo-randomly generated unsigned 32-bit integer less than MaxValueNotInclusive.


Generates a random integer less than the provided maximum value.


This function generates a pseudo-random number using [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) algorithm and returns it. The returned number is guaranteed to be less than the provided MaxValueNotInclusive parameter. If MaxValueNotInclusive is zero, the function will return zero as well.




**Parameters:**


* `MaxValueNotInclusive` The upper limit of the random integer (exclusive). Must be greater than or equal to zero. 



**Returns:**

A pseudo-random number less than MaxValueNotInclusive. If MaxValueNotInclusive is zero, returns zero. 





        

<hr>



### function RollRandomRotationFloat 

_RollRandomRotationFloat generates a random float value for rotation. The function uses Perlin noise to generate a pseudo-random number and cast it to float. This is used as a means of generating a random float value that can be used for rotation purposes._ 
```C++
static float AGE::SquirrelRNG::RollRandomRotationFloat () 
```





**Returns:**

A floating point number between 0 and 1 representing the generated random rotation.


This function returns a random float value.


The function uses the Perlin noise algorithm to generate a pseudo-random number between 0 and 1. It increments the seed for each call, providing different values on subsequent calls.




**Returns:**

A floating point number in the range [0, 1]. 





        

<hr>



### function RollRandomUint16 

_Generates a random uint16\_t value._ 
```C++
static uint16_t AGE::SquirrelRNG::RollRandomUint16 () 
```



This function generates and returns a pseudo-random uint16\_t number using the [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) algorithm. The returned value is uniformly distributed over its entire range of possible values, from 0 to 65535 (inclusive).




**Returns:**

A random uint16\_t value.


Generates a random uint16 number between 0 and UINT16\_MAX.


This function uses the [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) algorithm to generate a pseudorandom number in the range of uint16. The generated value is then returned as an unsigned 16-bit integer.




**Returns:**

An unsigned 16-bit integer representing the random number. 





        

<hr>



### function RollRandomUint32 

_Generates a random uint32 number._ 
```C++
static uint32_t AGE::SquirrelRNG::RollRandomUint32 () 
```



This function generates and returns a pseudo-random unsigned integer of type uint32\_t. The actual values returned are not truly random, but rather determined by the internal state of the [**SquirrelRNG**](class_a_g_e_1_1_squirrel_r_n_g.md) object.




**Returns:**

A randomly generated uint32\_t number. In this case, it always returns 0 as per the current implementation.


Generates a random uint32 number.


This function uses the internal state of the Squirrel RNG to generate a random uint32 number. The generated value is deterministic and depends on the initial seed of the RNG.




**Returns:**

A pseudo-random 32-bit unsigned integer. 





        

<hr>



### function SetCurrentPosition 

_Sets the current position value._ 
```C++
static inline void AGE::SquirrelRNG::SetCurrentPosition (
    int Position
) 
```



This function sets the 's\_Position' variable to a new integer value provided as an argument. It does not return anything, so it is void.




**Parameters:**


* `Position` The new integer value that will be set for 's\_Position'.

Sets the current position to a given integer value.


This function sets the static variable 's\_Position' to the input parameter 'Position'. It does not return anything, so it is void type.




**Parameters:**


* `Position` The new position to be set for s\_Position. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/RNG/Public/RNG.h`

