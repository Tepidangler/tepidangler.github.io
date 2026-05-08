

# Class AGE::JsonParser



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**JsonParser**](class_a_g_e_1_1_json_parser.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**JsonParser**](#function-jsonparser-12) () = default<br> |
|   | [**JsonParser**](#function-jsonparser-22) (const std::string & FilePath) <br> |
|  bool | [**SaveJsonFile**](#function-savejsonfile) (const std::filesystem::path & Filepath, std::vector&lt; T &gt; & Data) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  nlohmann::json | [**LoadJsonFile**](#function-loadjsonfile) (const std::filesystem::path & Filepath) <br> |
|  std::string | [**Parse**](#function-parse) (const std::string & FilePath) <br> |
|  std::string | [**ParseString**](#function-parsestring) (const std::string & String) <br> |


























## Public Functions Documentation




### function JsonParser [1/2]

```C++
AGE::JsonParser::JsonParser () = default
```




<hr>



### function JsonParser [2/2]

```C++
AGE::JsonParser::JsonParser (
    const std::string & FilePath
) 
```




<hr>



### function SaveJsonFile 

```C++
template<typename T>
bool AGE::JsonParser::SaveJsonFile (
    const std::filesystem::path & Filepath,
    std::vector< T > & Data
) 
```




<hr>
## Public Static Functions Documentation




### function LoadJsonFile 

```C++
static nlohmann::json AGE::JsonParser::LoadJsonFile (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function Parse 

```C++
static std::string AGE::JsonParser::Parse (
    const std::string & FilePath
) 
```




<hr>



### function ParseString 

```C++
static std::string AGE::JsonParser::ParseString (
    const std::string & String
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Parser/Public/JsonParser.h`

