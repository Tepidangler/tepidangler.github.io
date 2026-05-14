

# Class AGE::JsonParser



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**JsonParser**](class_a_g_e_1_1_json_parser.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**JsonParser**](#function-jsonparser-12) () = default<br>_Default constructor for_ [_**JsonParser**_](class_a_g_e_1_1_json_parser.md) _class._ |
|   | [**JsonParser**](#function-jsonparser-22) (const std::string & FilePath) <br>_Constructor for_ [_**JsonParser**_](class_a_g_e_1_1_json_parser.md) _class. Initializes the object with a JSON file path to parse._ |
|  bool | [**SaveJsonFile**](#function-savejsonfile) (const std::filesystem::path & Filepath, std::vector&lt; T &gt; & Data) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  nlohmann::json | [**LoadJsonFile**](#function-loadjsonfile) (const std::filesystem::path & Filepath) <br>_Loads a JSON file from the given path._  |
|  std::string | [**Parse**](#function-parse) (const std::string & FilePath) <br>_Parses a JSON file and returns its content as a string._  |
|  std::string | [**ParseString**](#function-parsestring) (const std::string & String) <br>_Parses a JSON string and returns its array representation._  |


























## Public Functions Documentation




### function JsonParser [1/2]

_Default constructor for_ [_**JsonParser**_](class_a_g_e_1_1_json_parser.md) _class._
```C++
AGE::JsonParser::JsonParser () = default
```



Default constructor for [**JsonParser**](class_a_g_e_1_1_json_parser.md) class. 


        

<hr>



### function JsonParser [2/2]

_Constructor for_ [_**JsonParser**_](class_a_g_e_1_1_json_parser.md) _class. Initializes the object with a JSON file path to parse._
```C++
AGE::JsonParser::JsonParser (
    const std::string & FilePath
) 
```





**Parameters:**


* `FilePath` The path of the JSON file to be parsed.

Constructs a [**JsonParser**](class_a_g_e_1_1_json_parser.md) object with the given file path.


This function initializes a new instance of the [**JsonParser**](class_a_g_e_1_1_json_parser.md) class, which is used to parse JSON files. The file path provided should point to a valid JSON file.




**Parameters:**


* `FilePath` A string representing the path to the JSON file that will be parsed by this object. 




        

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

_Loads a JSON file from the given path._ 
```C++
static nlohmann::json AGE::JsonParser::LoadJsonFile (
    const std::filesystem::path & Filepath
) 
```



This function attempts to load a JSON file at the provided path and returns its content as a nlohmann::json object. If the file does not exist, it logs an error message and returns an empty json object. If the file is empty or corrupted, it also logs a warning message and returns an empty json object.




**Parameters:**


* `Filepath` The path to the JSON file to load. 



**Returns:**

nlohmann::json An object containing the content of the loaded JSON file. Returns an empty json object if the file does not exist or is empty/corrupted.


Loads a JSON file from the given path.


This function attempts to load a JSON file at the specified location and parse it into a nlohmann::json object. If the file does not exist, an empty json object is returned with a warning message. If the file exists but is empty or corrupted, another warning message is returned.




**Parameters:**


* `Filepath` The path to the JSON file to load. 



**Returns:**

A nlohmann::json object containing the data from the loaded file, or an empty json object if the file does not exist or is empty/corrupted. 





        

<hr>



### function Parse 

_Parses a JSON file and returns its content as a string._ 
```C++
static std::string AGE::JsonParser::Parse (
    const std::string & FilePath
) 
```





**Parameters:**


* `FilePath` The path to the JSON file that should be parsed. 



**Returns:**

A string containing the contents of the JSON file, or an empty string if the file could not be opened or parsed.


Parses a JSON file and returns its content as a string. 

**Parameters:**


* `FilePath` The path to the JSON file that should be parsed. 



**Returns:**

A string containing the contents of the JSON file, or an empty string if the file could not be opened or parsed. 





        

<hr>



### function ParseString 

_Parses a JSON string and returns its array representation._ 
```C++
static std::string AGE::JsonParser::ParseString (
    const std::string & String
) 
```



This function takes in a JSON string, parses it using the nlohmann::json library, converts it to an array (if possible), and then returns this array as a string.




**Parameters:**


* `String` The input JSON string to be parsed. 



**Returns:**

A string representation of the parsed JSON data's array. If the JSON data is not an array, "Unknown" will be returned.


Parses a JSON string and returns its array representation.


This function takes in a JSON string, parses it using the nlohmann::json library, converts it to an array (if possible), and then returns this array as a string.




**Parameters:**


* `String` The input JSON string that needs to be parsed. 



**Returns:**

A string representation of the parsed JSON data's array part. If the JSON data is not an array, or if it cannot be converted into a string, "Unknown" will be returned. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Parser/Public/JsonParser.h`

