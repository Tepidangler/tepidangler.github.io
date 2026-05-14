

# Class AGE::SquirrelNoise



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**Get1dNoiseForRotation**](#function-get1dnoiseforrotation) (int Rotation, uint32\_t Seed=0) <br>_Same Functions, mapped to floats in [-180,180]._  |
|  float | [**Get1dNoiseNegOneToOne**](#function-get1dnoisenegonetoone) (int Position, uint32\_t Seed=0) <br>_Same Functions, mapped to floats in [-1,1]._  |
|  uint32\_t | [**Get1dNoiseUint**](#function-get1dnoiseuint) (int Position, uint32\_t Seed=0) <br>_Generates a one-dimensional noise value._  |
|  float | [**Get1dNoiseZeroToOne**](#function-get1dnoisezerotoone) (int Position, uint32\_t Seed=0) <br>_Computes a one-dimensional noise value in the range [0, 1] for a given position and seed._  |
|  float | [**Get2dNoiseNegOneToOne**](#function-get2dnoisenegonetoone) (int PositionX, int PositionY, uint32\_t Seed=0) <br>_This function generates a 2D noise value between -1 and 1._  |
|  uint32\_t | [**Get2dNoiseUint**](#function-get2dnoiseuint) (int PositionX, int PositionY, uint32\_t Seed=0) <br>_Computes a two-dimensional noise value._  |
|  float | [**Get2dNoiseZeroToOne**](#function-get2dnoisezerotoone) (int PositionX, int PositionY, uint32\_t Seed=0) <br>_This function returns a two-dimensional noise value between 0 and 1._  |
|  float | [**Get3dNoiseNegOneToOne**](#function-get3dnoisenegonetoone) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br>_This function generates a 3D noise value between -1 and 1._  |
|  uint32\_t | [**Get3dNoiseUint**](#function-get3dnoiseuint) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br>_This function generates a 3D noise value using the_ [_**SquirrelNoise**_](class_a_g_e_1_1_squirrel_noise.md) _algorithm._ |
|  float | [**Get3dNoiseZeroToOne**](#function-get3dnoisezerotoone) (int PositionX, int PositionY, int PositionZ, uint32\_t Seed=0) <br>_This function generates a 3D noise value between 0 and 1._  |
|  float | [**Get4dNoiseNegOneToOne**](#function-get4dnoisenegonetoone) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br>_This function generates a four-dimensional noise value between -1 and 1._  |
|  uint32\_t | [**Get4dNoiseUint**](#function-get4dnoiseuint) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br>_Computes a four-dimensional noise value._  |
|  float | [**Get4dNoiseZeroToOne**](#function-get4dnoisezerotoone) (int PositionX, int PositionY, int PositionZ, int PositionW, uint32\_t Seed=0) <br>_This function generates a four-dimensional noise value between 0 and 1._  |
|  uint32\_t | [**Rand**](#function-rand) () <br>_Generates a pseudorandom 32-bit unsigned integer._  |
|   | [**SquirrelNoise**](#function-squirrelnoise) () <br>_Constructor for_ [_**SquirrelNoise**_](class_a_g_e_1_1_squirrel_noise.md) _class. Initializes the position member variable to 0._ |




























## Public Functions Documentation




### function Get1dNoiseForRotation 

_Same Functions, mapped to floats in [-180,180]._ 
```C++
float AGE::SquirrelNoise::Get1dNoiseForRotation (
    int Rotation,
    uint32_t Seed=0
) 
```



Computes a one-dimensional noise value for a given rotation and seed.


This function uses a combination of bitwise operations to generate a pseudorandom number based on the input parameters. The result is then clamped between 1 and ONE\_OVER\_MAX\_UINT, which are constants defined in the [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) class.




**Parameters:**


* `Rotation` The rotation value used as an input for the noise generation. 
* `Seed` A seed value to initialize the random number generator. 



**Returns:**

A float value representing a one-dimensional noise value. 





        

<hr>



### function Get1dNoiseNegOneToOne 

_Same Functions, mapped to floats in [-1,1]._ 
```C++
float AGE::SquirrelNoise::Get1dNoiseNegOneToOne (
    int Position,
    uint32_t Seed=0
) 
```



This function generates a one-dimensional noise value between -1 and 1.


The function takes an integer position and a seed as input parameters. It uses the provided position and seed to generate a pseudo-random number using bitwise operations, which is then scaled to fall within the range of -1 to 1.




**Parameters:**


* `Position` An integer representing the position for which to generate noise. 
* `Seed` A 32-bit unsigned integer used as a seed for the random number generation.



**Returns:**

A floating-point value between -1 and 1, representing the generated noise value.


Computes a noise value in the range -1 to 1.


This function generates a pseudo-random float value using a hash function on an input position and seed. The output is then scaled to fall within the range of -1 to 1.




**Parameters:**


* `Position` The integer position for which to generate noise. 
* `Seed` A unique identifier used to initialize the random number generator. 



**Returns:**

A float value in the range -1 to 1 representing the computed noise. 





        

<hr>



### function Get1dNoiseUint 

_Generates a one-dimensional noise value._ 
```C++
uint32_t AGE::SquirrelNoise::Get1dNoiseUint (
    int Position,
    uint32_t Seed=0
) 
```



This function generates a pseudorandom number for the given position and seed using a combination of bitwise operations. The result is then returned as an unsigned 32-bit integer.




**Parameters:**


* `Position` The input position for which to generate the noise. 
* `Seed` A random value used to initialize the noise generation. 



**Returns:**

An unsigned 32-bit integer representing the one-dimensional noise at the given position and seed.


Generates a one-dimensional noise value.


This function generates a pseudorandom number based on the input position and seed using various bitwise operations. The result is then returned as an unsigned 32-bit integer.




**Parameters:**


* `Position` The input position for generating the noise. 
* `Seed` A seed value to initialize the random generator. 



**Returns:**

An unsigned 32-bit integer representing the generated noise value. 





        

<hr>



### function Get1dNoiseZeroToOne 

_Computes a one-dimensional noise value in the range [0, 1] for a given position and seed._ 
```C++
float AGE::SquirrelNoise::Get1dNoiseZeroToOne (
    int Position,
    uint32_t Seed=0
) 
```



This function uses a hash function to generate a pseudorandom number based on the input parameters. The result is then scaled to the range [0, 1]. 

**Parameters:**


* `Position` The integer position for which to compute the noise value. 
* `Seed` A unique identifier used to seed the random number generator. 



**Returns:**

A floating-point value representing the computed noise in the range [0, 1].


Computes a one-dimensional noise value in the range [0, 1] for a given position and seed.


This function uses a hashing algorithm to generate a pseudorandom number based on the input parameters. The result is then scaled to fall within the range [0, 1].




**Parameters:**


* `Position` The integer position in the noise field. 
* `Seed` A seed value for the random number generation. 



**Returns:**

A floating-point value representing the one-dimensional noise at the given position and with the given seed. 





        

<hr>



### function Get2dNoiseNegOneToOne 

_This function generates a 2D noise value between -1 and 1._ 
```C++
float AGE::SquirrelNoise::Get2dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```



The function takes in two positions (x and y) and a seed for the random number generation. It uses the [**Get2dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get2dnoiseuint) function to generate an integer noise value, which is then scaled to be between -1 and 1 by multiplying with ONE\_OVER\_MAX\_INT.




**Parameters:**


* `PositionX` The x position in the noise field. 
* `PositionY` The y position in the noise field. 
* `Seed` A seed for the random number generation.



**Returns:**

A float value representing the 2D noise at the given positions and with the provided seed, between -1 and 1.


This function generates a 2D noise value between -1 and 1.


The function takes in two positions (x and y) and a seed for the random number generation. It uses the [**Get2dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get2dnoiseuint) function to generate an integer noise value, then scales it by ONE\_OVER\_MAX\_INT to get a float between -1 and 1.




**Parameters:**


* `PositionX` The x position in the noise field. 
* `PositionY` The y position in the noise field. 
* `Seed` A seed for the random number generation.



**Returns:**

A floating-point value representing the 2D noise at the given positions and with the provided seed, between -1 and 1. 





        

<hr>



### function Get2dNoiseUint 

_Computes a two-dimensional noise value._ 
```C++
uint32_t AGE::SquirrelNoise::Get2dNoiseUint (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```



This function generates a pseudo-random number based on the input parameters using a prime number (198491317) to create an offset for the x position in combination with the y position. The result is then passed through [**Get1dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get1dnoiseuint) to generate the noise value.




**Parameters:**


* `PositionX` The x-coordinate of the point for which to compute the noise. 
* `PositionY` The y-coordinate of the point for which to compute the noise. 
* `Seed` A seed value used to initialize the pseudo-random number generator.



**Returns:**

A pseudo-random integer between 0 and UINT32\_MAX, representing a two-dimensional noise value.


Computes a two-dimensional noise value.


This function generates a pseudo-random number based on the input coordinates and seed, using a prime number (198491317) to scramble the position data. The scrambled xy-coordinate is then passed into the [**Get1dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get1dnoiseuint) function for further processing.




**Parameters:**


* `PositionX` The x-coordinate in the noise field. 
* `PositionY` The y-coordinate in the noise field. 
* `Seed` A seed value to initialize the random number generator.



**Returns:**

A pseudo-random uint32\_t value based on the input coordinates and seed. 





        

<hr>



### function Get2dNoiseZeroToOne 

_This function returns a two-dimensional noise value between 0 and 1._ 
```C++
float AGE::SquirrelNoise::Get2dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    uint32_t Seed=0
) 
```



The function takes three parameters - the x and y positions for which to generate the noise, and a seed used in the random number generation. It uses the [**Get2dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get2dnoiseuint) function internally to get an unsigned integer noise value, then scales this by ONE\_OVER\_MAX\_UINT to return a float between 0 and 1.




**Parameters:**


* `PositionX` The x position for which to generate the noise. 
* `PositionY` The y position for which to generate the noise. 
* `Seed` A seed used in the random number generation.



**Returns:**

A floating-point value between 0 and 1 representing the two-dimensional noise at the given positions with the provided seed.


This function generates a two-dimensional noise value between 0 and 1.


The function takes in three parameters - the x and y positions for which to generate the noise, as well as a seed for random number generation. It uses the [**Get2dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get2dnoiseuint) function internally to get an unsigned integer noise value, then converts this to a float between 0 and 1 by multiplying with ONE\_OVER\_MAX\_UINT (a constant defined in [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) class).




**Parameters:**


* `PositionX` The x position for which to generate the noise. 
* `PositionY` The y position for which to generate the noise. 
* `Seed` A seed value for random number generation.



**Returns:**

Returns a float between 0 and 1 representing the two-dimensional noise at the given positions with the provided seed. 





        

<hr>



### function Get3dNoiseNegOneToOne 

_This function generates a 3D noise value between -1 and 1._ 
```C++
float AGE::SquirrelNoise::Get3dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```



The function takes in the x, y, z coordinates of the position for which we want to generate noise, as well as a seed for the random number generator. It uses this information along with some pre-defined constants (like ONE\_OVER\_MAX\_INT) to calculate and return a 3D noise value between -1 and 1.




**Parameters:**


* `PositionX` The x coordinate of the position for which we want to generate noise. 
* `PositionY` The y coordinate of the position for which we want to generate noise. 
* `PositionZ` The z coordinate of the position for which we want to generate noise. 
* `Seed` A seed for the random number generator used in generating the noise value.



**Returns:**

Returns a float between -1 and 1 representing the calculated 3D noise value.


This function generates a 3D noise value between -1 and 1.


The function takes in the x, y, z coordinates of the position to generate the noise for, as well as a seed for the random number generation. It uses the [**Get3dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get3dnoiseuint) function internally to get an unsigned integer noise value, which it then scales down by ONE\_OVER\_MAX\_INT and converts to float before returning.




**Parameters:**


* `PositionX` The x coordinate of the position to generate the noise for. 
* `PositionY` The y coordinate of the position to generate the noise for. 
* `PositionZ` The z coordinate of the position to generate the noise for. 
* `Seed` A seed for the random number generation.



**Returns:**

A float representing a 3D noise value between -1 and 1. 





        

<hr>



### function Get3dNoiseUint 

_This function generates a 3D noise value using the_ [_**SquirrelNoise**_](class_a_g_e_1_1_squirrel_noise.md) _algorithm._
```C++
uint32_t AGE::SquirrelNoise::Get3dNoiseUint (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```



The function takes in three positions (PositionX, PositionY, and PositionZ) and a seed for randomness. It uses these inputs to generate a unique hash which is then passed into the [**Get1dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get1dnoiseuint) function. This function returns a uint32\_t value representing the noise at the given position.




**Parameters:**


* `PositionX` The x-coordinate of the position in the noise field. 
* `PositionY` The y-coordinate of the position in the noise field. 
* `PositionZ` The z-coordinate of the position in the noise field. 
* `Seed` A seed for randomness, used to generate a unique hash.



**Returns:**

Returns a uint32\_t value representing the noise at the given position.


This function generates a 3D noise value using the [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) algorithm.


The function takes in three positions (PositionX, PositionY, and PositionZ) and a seed to generate a unique noise value. It uses two prime numbers (PRIME\_NUMBER1 and PRIME\_NUMBER2) to create an offset for the position values which enhances the randomness of the noise generation.




**Parameters:**


* `PositionX` The x-coordinate of the position in the 3D space. 
* `PositionY` The y-coordinate of the position in the 3D space. 
* `PositionZ` The z-coordinate of the position in the 3D space. 
* `Seed` A seed value to generate a unique noise value.



**Returns:**

Returns a uint32\_t noise value generated using [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) algorithm. 





        

<hr>



### function Get3dNoiseZeroToOne 

_This function generates a 3D noise value between 0 and 1._ 
```C++
float AGE::SquirrelNoise::Get3dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    uint32_t Seed=0
) 
```



The function takes in the x, y, z coordinates of the position for which to generate the noise, as well as a seed for random number generation. It uses this information along with some pre-defined constants (like ONE\_OVER\_MAX\_UINT) to calculate and return a noise value between 0 and 1.




**Parameters:**


* `PositionX` The x coordinate of the position for which to generate the noise. 
* `PositionY` The y coordinate of the position for which to generate the noise. 
* `PositionZ` The z coordinate of the position for which to generate the noise. 
* `Seed` A seed value used in random number generation.



**Returns:**

A float representing a 3D noise value between 0 and 1.


This function generates a 3D noise value between 0 and 1.


The function takes in the x, y, z coordinates of the position for which to generate the noise, as well as a seed for random number generation. It uses this information along with some predefined constants (like ONE\_OVER\_MAX\_UINT) to calculate and return a float value between 0 and 1 representing the noise at that location.




**Parameters:**


* `PositionX` The x-coordinate of the position for which to generate noise. 
* `PositionY` The y-coordinate of the position for which to generate noise. 
* `PositionZ` The z-coordinate of the position for which to generate noise. 
* `Seed` A seed value used in random number generation.



**Returns:**

A float value between 0 and 1 representing the noise at the given position. 





        

<hr>



### function Get4dNoiseNegOneToOne 

_This function generates a four-dimensional noise value between -1 and 1._ 
```C++
float AGE::SquirrelNoise::Get4dNoiseNegOneToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```



The function uses the [**Get4dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get4dnoiseuint) method to generate an integer noise value, then scales it by ONE\_OVER\_MAX\_INT to get a float value in the range [0, 1]. This is then scaled by 2 and subtracted from 3 to get a value in the range [-1, 1].




**Parameters:**


* `PositionX` The x-coordinate of the position for which to generate noise. 
* `PositionY` The y-coordinate of the position for which to generate noise. 
* `PositionZ` The z-coordinate of the position for which to generate noise. 
* `PositionW` The w-coordinate of the position for which to generate noise. 
* `Seed` A seed value used to initialize the random number generator.



**Returns:**

A float value representing the four-dimensional noise at the given position and with the given seed. This will be in the range [-1, 1].


This function generates a four-dimensional noise value between -1 and 1.


The function takes in the positions (x, y, z, w) and a seed to generate a pseudorandom number. It then scales this number by one over the maximum integer value to get a floating point number between 0 and 1. This is then multiplied by -1 and 1 to get a noise value between -1 and 1.




**Parameters:**


* `PositionX` The x position in the noise space. 
* `PositionY` The y position in the noise space. 
* `PositionZ` The z position in the noise space. 
* `PositionW` The w position in the noise space. 
* `Seed` A seed for the pseudorandom number generator.



**Returns:**

A floating point value between -1 and 1 representing a four-dimensional noise value. 





        

<hr>



### function Get4dNoiseUint 

_Computes a four-dimensional noise value._ 
```C++
uint32_t AGE::SquirrelNoise::Get4dNoiseUint (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```



This function computes the noise value for a given position in space (x, y, z, w) and with a specific seed. The computation is based on the [**Get1dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get1dnoiseuint) function, which internally uses a prime number to generate pseudo-random values.




**Parameters:**


* `PositionX` The x coordinate of the position for which to compute the noise value. 
* `PositionY` The y coordinate of the position for which to compute the noise value. 
* `PositionZ` The z coordinate of the position for which to compute the noise value. 
* `PositionW` The w coordinate of the position for which to compute the noise value. 
* `Seed` A seed used to initialize the pseudo-random number generator.



**Returns:**

A 32-bit unsigned integer representing the computed noise value.


Computes a four-dimensional noise value.


This function calculates a noise value based on the input parameters and a provided seed. The calculation involves a prime number multiplication, which is used to disperse the values evenly across the noise space.




**Parameters:**


* `PositionX` The x position for the noise calculation. 
* `PositionY` The y position for the noise calculation. 
* `PositionZ` The z position for the noise calculation. 
* `PositionW` The w position for the noise calculation. 
* `Seed` A seed value used to initialize the random number generator.



**Returns:**

Returns a uint32\_t representing the calculated noise value. 





        

<hr>



### function Get4dNoiseZeroToOne 

_This function generates a four-dimensional noise value between 0 and 1._ 
```C++
float AGE::SquirrelNoise::Get4dNoiseZeroToOne (
    int PositionX,
    int PositionY,
    int PositionZ,
    int PositionW,
    uint32_t Seed=0
) 
```



The function uses the [**Get4dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get4dnoiseuint) method to generate an unsigned integer noise value. It then converts this value into a float between 0 and 1 by multiplying it with ONE\_OVER\_MAX\_UINT (a constant defined in [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) class).




**Parameters:**


* `PositionX` The x-coordinate of the position for which to generate noise. 
* `PositionY` The y-coordinate of the position for which to generate noise. 
* `PositionZ` The z-coordinate of the position for which to generate noise. 
* `PositionW` The w-coordinate of the position for which to generate noise. 
* `Seed` A seed value used to initialize the random number generator.



**Returns:**

A float representing a four-dimensional noise value between 0 and 1.


This function generates a four-dimensional noise value between 0 and 1.


The function uses the [**Get4dNoiseUint()**](class_a_g_e_1_1_squirrel_noise.md#function-get4dnoiseuint) method to generate an unsigned integer noise value. It then converts this value into a float between 0 and 1 by multiplying it with ONE\_OVER\_MAX\_UINT (a constant defined as 1.0/UINT32\_MAX).




**Parameters:**


* `PositionX` The x-coordinate of the position for which to generate noise. 
* `PositionY` The y-coordinate of the position for which to generate noise. 
* `PositionZ` The z-coordinate of the position for which to generate noise. 
* `PositionW` The w-coordinate of the position for which to generate noise. 
* `Seed` A seed value used to initialize the random number generator.



**Returns:**

A float between 0 and 1 representing the four-dimensional noise at the specified position. 





        

<hr>



### function Rand 

_Generates a pseudorandom 32-bit unsigned integer._ 
```C++
uint32_t AGE::SquirrelNoise::Rand () 
```



This function uses the [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) algorithm to generate a pseudorandom number. The generated value is based on the current position in the noise field, which is then incremented for the next call.




**Returns:**

A pseudorandom 32-bit unsigned integer.


Generates a pseudorandom number using the squirrel noise algorithm.


This function generates a pseudorandom number based on the current position in the noise field, and then increments that position by one for subsequent calls. The returned value is an unsigned 32-bit integer.




**Returns:**

A pseudorandom number generated using squirrel noise algorithm. 





        

<hr>



### function SquirrelNoise 

_Constructor for_ [_**SquirrelNoise**_](class_a_g_e_1_1_squirrel_noise.md) _class. Initializes the position member variable to 0._
```C++
AGE::SquirrelNoise::SquirrelNoise () 
```



Constructor for [**SquirrelNoise**](class_a_g_e_1_1_squirrel_noise.md) class. Initializes the position to 0. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/RNG/Public/RNG.h`

