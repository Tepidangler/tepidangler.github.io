

# Class AGE::IniReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**IniReader**](class_a_g_e_1_1_ini_reader.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**IniReader**](#function-inireader) (const std::filesystem::path & Path) <br>_Constructor for the_ [_**IniReader**_](class_a_g_e_1_1_ini_reader.md) _class. Takes a path to an .ini file as input and loads it into memory._ |
|  std::string | [**Read**](#function-read) (const std::string & Section, const std::string & Key, bool & HasMultipleValues) <br>_This function reads a value from the INI file._  |
|  std::vector&lt; std::string &gt; | [**ReadAll**](#function-readall) (const std::string & Section, const std::string & Key) <br>_Reads all values associated with a given key in a specified section of the INI file._  |
|   | [**~IniReader**](#function-inireader) () = default<br>_Destructor for the_ [_**IniReader**_](class_a_g_e_1_1_ini_reader.md) _class._ |




























## Public Functions Documentation




### function IniReader 

_Constructor for the_ [_**IniReader**_](class_a_g_e_1_1_ini_reader.md) _class. Takes a path to an .ini file as input and loads it into memory._
```C++
AGE::IniReader::IniReader (
    const std::filesystem::path & Path
) 
```





**Parameters:**


* `Path` The filesystem path to the .ini file that will be loaded.

Constructor for the [**IniReader**](class_a_g_e_1_1_ini_reader.md) class. It takes a file path as input and loads the INI file at that location into memory. 

**Parameters:**


* `Path` The filesystem path to the INI file which is to be loaded. 




        

<hr>



### function Read 

_This function reads a value from the INI file._ 
```C++
std::string AGE::IniReader::Read (
    const std::string & Section,
    const std::string & Key,
    bool & HasMultipleValues
) 
```



The function retrieves a value associated with a given key in a specified section of the INI file. If the key does not exist, it logs an error message and returns an empty string.




**Parameters:**


* `Section` The name of the section to read from. 
* `Key` The key for which to retrieve a value. 
* `HasMultipleValues` A flag indicating whether the key has multiple values in the INI file.



**Returns:**

Returns the value associated with the given key, or an empty string if the key does not exist.


This function reads a value from the INI file.


The function takes three parameters - section name, key and a boolean reference to indicate if there are multiple values for the given key in the specified section. It returns an empty string if it fails to read the value or the key-value pair does not exist.




**Parameters:**


* `Section` A constant reference to the section name where the key is located. 
* `Key` A constant reference to the key whose value needs to be retrieved. 
* `HasMultipleValues` A boolean reference that indicates if there are multiple values for the given key in the specified section.



**Returns:**

Returns a string containing the value of the key-value pair, or an empty string if it fails to read the value or the key-value pair does not exist. 





        

<hr>



### function ReadAll 

_Reads all values associated with a given key in a specified section of the INI file._ 
```C++
std::vector< std::string > AGE::IniReader::ReadAll (
    const std::string & Section,
    const std::string & Key
) 
```



This function retrieves all values associated with a specific key within a particular section of the INI file. If no such key exists, it logs an error message and returns an empty vector. The results are sorted based on their load order as defined by CSimpleIniA::Entry::LoadOrder().




**Parameters:**


* `Section` A string representing the name of the section in the INI file to be read from. 
* `Key` A string representing the key whose values are to be retrieved. 



**Returns:**

A vector of strings containing all values associated with the provided key in the specified section, sorted based on their load order. If no such key exists, an empty vector is returned.


Reads all values associated with a given key in a specified section of the INI file.


This function retrieves all values associated with a specific key within a particular section of the INI file. If no such key exists, it returns an empty vector.




**Parameters:**


* `Section` The name of the section to search for keys in. 
* `Key` The key whose associated values are being retrieved. 



**Returns:**

A vector containing all values associated with the provided key in the specified section. If no such key exists, it returns an empty vector. 





        

<hr>



### function ~IniReader 

_Destructor for the_ [_**IniReader**_](class_a_g_e_1_1_ini_reader.md) _class._
```C++
AGE::IniReader::~IniReader () = default
```



This function is responsible for freeing any resources that were allocated during the lifetime of an instance of this class.


Destructor for the [**IniReader**](class_a_g_e_1_1_ini_reader.md) class.


This function is responsible for freeing any resources that were allocated during the lifetime of an instance of this class, such as memory or file handles. It's important to ensure that all resources are properly released when they are no longer needed to prevent potential memory leaks or other issues in your program.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/IniReader.h`

