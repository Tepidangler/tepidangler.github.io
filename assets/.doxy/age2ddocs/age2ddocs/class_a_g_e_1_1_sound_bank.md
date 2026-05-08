

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
|  [**UUID**](class_a_g_e_1_1_u_u_i_d.md) & | [**GetAssetID**](#function-getassetid) () <br> |
|  uint32\_t | [**GetBankID**](#function-getbankid) () <br> |
|  std::string & | [**GetBankName**](#function-getbankname) () <br> |
|  std::filesystem::path & | [**GetFilePath**](#function-getfilepath) () <br> |
|  void | [**SetBankID**](#function-setbankid) (uint32\_t ID) <br> |
|  void | [**SetBankName**](#function-setbankname) (const std::string & Name) <br> |
|   | [**SoundBank**](#function-soundbank-12) (const std::filesystem::path & FilePath, [**UUID**](class_a_g_e_1_1_u_u_i_d.md) ID) <br> |
|   | [**SoundBank**](#function-soundbank-22) (const [**SoundBank**](class_a_g_e_1_1_sound_bank.md) &) = default<br> |
|   | [**~SoundBank**](#function-soundbank) () = default<br> |




























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

```C++
inline UUID & AGE::SoundBank::GetAssetID () 
```




<hr>



### function GetBankID 

```C++
inline uint32_t AGE::SoundBank::GetBankID () 
```




<hr>



### function GetBankName 

```C++
inline std::string & AGE::SoundBank::GetBankName () 
```




<hr>



### function GetFilePath 

```C++
inline std::filesystem::path & AGE::SoundBank::GetFilePath () 
```




<hr>



### function SetBankID 

```C++
inline void AGE::SoundBank::SetBankID (
    uint32_t ID
) 
```




<hr>



### function SetBankName 

```C++
inline void AGE::SoundBank::SetBankName (
    const std::string & Name
) 
```




<hr>



### function SoundBank [1/2]

```C++
AGE::SoundBank::SoundBank (
    const std::filesystem::path & FilePath,
    UUID ID
) 
```




<hr>



### function SoundBank [2/2]

```C++
AGE::SoundBank::SoundBank (
    const SoundBank &
) = default
```




<hr>



### function ~SoundBank 

```C++
AGE::SoundBank::~SoundBank () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Audio/AudioEngine/Public/Soundbank.h`

