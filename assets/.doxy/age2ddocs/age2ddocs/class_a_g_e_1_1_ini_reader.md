

# Class AGE::IniReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**IniReader**](class_a_g_e_1_1_ini_reader.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**IniReader**](#function-inireader) (const std::filesystem::path & Path) <br> |
|  std::string | [**Read**](#function-read) (const std::string & Section, const std::string & Key, bool & HasMultipleValues) <br> |
|  std::vector&lt; std::string &gt; | [**ReadAll**](#function-readall) (const std::string & Section, const std::string & Key) <br> |
|   | [**~IniReader**](#function-inireader) () = default<br> |




























## Public Functions Documentation




### function IniReader 

```C++
AGE::IniReader::IniReader (
    const std::filesystem::path & Path
) 
```




<hr>



### function Read 

```C++
std::string AGE::IniReader::Read (
    const std::string & Section,
    const std::string & Key,
    bool & HasMultipleValues
) 
```




<hr>



### function ReadAll 

```C++
std::vector< std::string > AGE::IniReader::ReadAll (
    const std::string & Section,
    const std::string & Key
) 
```




<hr>



### function ~IniReader 

```C++
AGE::IniReader::~IniReader () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/IniReader.h`

