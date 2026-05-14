

# Class AGE::Utils::EngineStatics



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Utils**](namespace_a_g_e_1_1_utils.md) **>** [**EngineStatics**](class_a_g_e_1_1_utils_1_1_engine_statics.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  std::string | [**GetFilename**](#function-getfilename) (std::filesystem::path & Name) <br>_This function returns the filename from a given filesystem path._  |
|  bool | [**IsBigEndian**](#function-isbigendian) (void) <br>_This function checks if the system is big endian or not._  |
|  bool | [**IsBitSet**](#function-isbitset) (T Num, T Pos) <br>_This function checks if a specific bit is set in the given number._  |


























## Public Static Functions Documentation




### function GetFilename 

_This function returns the filename from a given filesystem path._ 
```C++
static inline std::string AGE::Utils::EngineStatics::GetFilename (
    std::filesystem::path & Name
) 
```



The function takes in a std::filesystem::path object and uses it to extract the filename by replacing any extension with an empty string, then returning the resultant filename as a std::string.




**Parameters:**


* `Name` A reference to a std::filesystem::path object representing the path from which we want to extract the filename. 



**Returns:**

The function returns a std::string containing the name of the file represented by the input path, without any extension. If the provided path does not represent a valid file, an empty string is returned.


This function returns the filename from a given filesystem path.


The function takes in a std::filesystem::path object and uses it to extract the filename by replacing any extension with an empty string, then returning the resultant filename as a std::string.




**Parameters:**


* `Name` A reference to a std::filesystem::path object representing the path from which we want to extract the filename. 



**Returns:**

The function returns a std::string containing the filename extracted from the provided filesystem path. 





        

<hr>



### function IsBigEndian 

_This function checks if the system is big endian or not._ 
```C++
static inline bool AGE::Utils::EngineStatics::IsBigEndian (
    void
) 
```



It does this by creating a union that contains an unsigned integer and four characters. The integer is initialized with a value of 0x01020304. If the first character in the union (c[0]) equals to 1, then it means that the system is little endian. Otherwise, it's big endian.




**Returns:**

Returns true if the system is big endian and false otherwise.


This function checks if the system is big endian or not.


The function uses a union to create an instance of a uint32\_t and a char array. It then assigns the value 0x01020304 to the uint32\_t member, which represents the bytes in memory as 01 02 03 04. The function returns true if the first byte of this union (representing the most significant byte) is equal to 1, indicating a big endian system. Otherwise, it returns false.




**Returns:**

bool - Returns true if the system is big endian, false otherwise. 





        

<hr>



### function IsBitSet 

_This function checks if a specific bit is set in the given number._ 
```C++
template<typename T>
static inline bool AGE::Utils::EngineStatics::IsBitSet (
    T Num,
    T Pos
) 
```





**Parameters:**


* `Num` The number to check for the bit being set. 
* `Pos` The position of the bit to be checked, starting from 0 at the least significant bit. 



**Returns:**

True if the specified bit is set (i.e., equals 1), false otherwise.


Checks if a specific bit is set in the given number.


This function takes two parameters, Num and Pos. It creates a mask by shifting the value 1 to the left by 'Pos' places. Then it checks if any of the bits in the result are set in the binary representation of 'Num'. If so, it returns true; otherwise, false.




**Parameters:**


* `Num` The number whose bit is being checked. 
* `Pos` The position of the bit to check from least significant bit (LSB) onwards.



**Returns:**

True if the specified bit in 'Num' is set, false otherwise. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Statics/Public/Statics.h`

