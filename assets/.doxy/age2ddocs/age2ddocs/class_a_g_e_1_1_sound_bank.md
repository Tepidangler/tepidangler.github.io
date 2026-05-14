

# Class AGE::SoundBank



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SoundBank**](class_a_g_e_1_1_sound_bank.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**m\_AssetID**](#variable-m_assetid)  <br> |
|  std::filesystem::path | [**m\_FilePath**](#variable-m_filepath)  <br> |
|  uint32\_t | [**m\_ID**](#variable-m_id)  <br> |
|  std::string | [**m\_Name**](#variable-m_name)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br>_Gets the Asset ID of the object._  |
|  uint32\_t | [**GetBankID**](#function-getbankid) () <br>_This function returns the bank ID of the current object._  |
|  std::string & | [**GetBankName**](#function-getbankname) () <br>_Returns the name of the bank._  |
|  std::filesystem::path & | [**GetFilePath**](#function-getfilepath) () <br>_Returns the file path of the object._  |
|  void | [**SetBankID**](#function-setbankid) (uint32\_t ID) <br>_This function sets the bank ID to a given value._  |
|  void | [**SetBankName**](#function-setbankname) (const std::string & Name) <br>_This function sets the bank name._  |
|   | [**SoundBank**](#function-soundbank-12) (const std::filesystem::path & FilePath, [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br>_Constructs a_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _object with the given file path and_[_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._ |
|   | [**SoundBank**](#function-soundbank-22) (const [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &) = default<br>_Default copy constructor for the_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _class._ |
|   | [**~SoundBank**](#function-soundbank) () = default<br>_Default destructor for the_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _class._ |




























## Public Attributes Documentation




### variable m\_AssetID 

```C++
UUID AGE::SoundBank::m_AssetID;
```




<hr>



### variable m\_FilePath 

```C++
std::filesystem::path AGE::SoundBank::m_FilePath;
```




<hr>



### variable m\_ID 

```C++
uint32_t AGE::SoundBank::m_ID;
```




<hr>



### variable m\_Name 

```C++
std::string AGE::SoundBank::m_Name;
```




<hr>
## Public Functions Documentation




### function GetAssetID 

_Gets the Asset ID of the object._ 
```C++
inline UUID & AGE::SoundBank::GetAssetID () 
```



This function returns a reference to the private member variable 'm\_AssetID'. It is used to access and possibly modify it if necessary. The returned value should not be altered as it may affect other parts of the program that rely on this unique identifier for their operations.




**Returns:**

A reference to [**UUID**](class_a_g_e_1_1_u_u_i_d.md)& representing the Asset ID.


Gets the Asset ID of the object.


This function returns a reference to the private member variable 'm\_AssetID'. It is used to access and possibly modify this value if necessary.




**Returns:**

A reference to [**UUID**](class_a_g_e_1_1_u_u_i_d.md)& representing the Asset ID. 





        

<hr>



### function GetBankID 

_This function returns the bank ID of the current object._ 
```C++
inline uint32_t AGE::SoundBank::GetBankID () 
```





**Returns:**

uint32\_t The bank ID as a 32-bit unsigned integer.


Retrieves the bank ID of the object. 

**Returns:**

The bank ID as a uint32\_t value. 





        

<hr>



### function GetBankName 

_Returns the name of the bank._ 
```C++
inline std::string & AGE::SoundBank::GetBankName () 
```





**Returns:**

A reference to a string containing the name of the bank.


Gets the name of a bank.


This function returns a reference to the private member variable `m_Name`, which holds the name of the bank. The returned value is non-const and can be modified by the caller. However, it's important to note that any changes made to this string will affect the internal state of the object.




**Returns:**

A reference to a string containing the name of the bank. 





        

<hr>



### function GetFilePath 

_Returns the file path of the object._ 
```C++
inline std::filesystem::path & AGE::SoundBank::GetFilePath () 
```





**Returns:**

A reference to the file path member variable.


Returns the file path of the object. 

**Returns:**

A reference to a std::filesystem::path object representing the file path. 





        

<hr>



### function SetBankID 

_This function sets the bank ID to a given value._ 
```C++
inline void AGE::SoundBank::SetBankID (
    uint32_t ID
) 
```





**Parameters:**


* `ID` The new uint32\_t type ID that will be set for the bank.

This function sets the bank identifier with a given uint32 value. 

**Parameters:**


* `ID` The unique identifier of the bank to be set. 




        

<hr>



### function SetBankName 

_This function sets the bank name._ 
```C++
inline void AGE::SoundBank::SetBankName (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The new name of the bank.

Sets the bank name.


This function sets the bank name by assigning it to the member variable m\_Name. The parameter 'Name' is a const reference to std::string, which represents the new bank name.




**Parameters:**


* `Name` A const reference to std::string representing the new bank name. 




        

<hr>



### function SoundBank [1/2]

_Constructs a_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _object with the given file path and_[_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _._
```C++
AGE::SoundBank::SoundBank (
    const std::filesystem::path & FilePath,
    UUID ID
) 
```





**Parameters:**


* `FilePath` The path to the sound bank file. 
* `ID` The unique identifier for this sound bank.

This function initializes a new [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object by setting its file path and [**UUID**](class_a_g_e_1_1_u_u_i_d.md), and also sets the name of the sound bank as the filename from the given path.


Constructs a [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object from the given file path and [**UUID**](class_a_g_e_1_1_u_u_i_d.md). 

**Parameters:**


* `FilePath` The path to the sound bank file. 
* `ID` The unique identifier for this sound bank. 




        

<hr>



### function SoundBank [2/2]

_Default copy constructor for the_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _class._
```C++
AGE::SoundBank::SoundBank (
    const SoundBank &
) = default
```



This function is used to create a new instance of the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object to be copied.



**Returns:**

A new instance of the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) class with the same data as the input parameter.


Default copy constructor for the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) class.


This function is used to create a new instance of the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) class by copying an existing one. It uses the '= default' syntax, which instructs the compiler to generate a default implementation for this member function.




**Parameters:**


* `other` The [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object to be copied.



**Returns:**

A new [**SoundBank**](class_a_g_e_1_1_sound_bank.md) instance that is a copy of the input [**SoundBank**](class_a_g_e_1_1_sound_bank.md). 





        

<hr>



### function ~SoundBank 

_Default destructor for the_ [_**SoundBank**_](class_a_g_e_1_1_sound_bank.md) _class._
```C++
AGE::SoundBank::~SoundBank () = default
```



This function is used to clean up any resources that the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object may be using, such as memory or file handles. It's important to ensure that all resources are properly released when they are no longer needed to prevent potential memory leaks or other issues.




**Returns:**

void


Destructor for the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) class.


This function is responsible for releasing any resources that were acquired by the [**SoundBank**](class_a_g_e_1_1_sound_bank.md) object, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AudioEngine/Public/Soundbank.h`

