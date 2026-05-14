

# Class AGE::IniWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**IniWriter**](class_a_g_e_1_1_ini_writer.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**IniWriter**](#function-iniwriter) (const std::filesystem::path & Path) <br>_Constructs an_ [_**IniWriter**_](class_a_g_e_1_1_ini_writer.md) _object with a given path to the INI file._ |
|  bool | [**SaveFile**](#function-savefile) () <br>_Saves the INI file with the given path and content._  |
|  bool | [**Write**](#function-write) (const std::string & Section, const std::string & Key, const std::string & Value) <br>_Writes a key-value pair to the INI file._  |
|   | [**~IniWriter**](#function-iniwriter) () = default<br>_Destructor for the_ [_**IniWriter**_](class_a_g_e_1_1_ini_writer.md) _class._ |




























## Public Functions Documentation




### function IniWriter 

_Constructs an_ [_**IniWriter**_](class_a_g_e_1_1_ini_writer.md) _object with a given path to the INI file._
```C++
AGE::IniWriter::IniWriter (
    const std::filesystem::path & Path
) 
```





**Parameters:**


* `Path` The path to the INI file. 



**Returns:**

None


Constructor for the [**IniWriter**](class_a_g_e_1_1_ini_writer.md) class.


This constructor takes a const reference to std::filesystem::path as an argument, which is used to initialize the member variable m\_IniPath. It also sets the Unicode encoding for the INI file and attempts to load it from the provided path. If the loading fails (indicated by a return code less than 0), an error message is logged.




**Parameters:**


* `Path` The path of the INI file to be loaded. 




        

<hr>



### function SaveFile 

_Saves the INI file with the given path and content._ 
```C++
bool AGE::IniWriter::SaveFile () 
```



This function saves the current INI data to a file at the specified path. It uses the SaveFile method of the m\_Ini object, which writes the data to the file system. The function returns true if the save operation was successful (indicated by SI\_OK return code), and false otherwise.




**Returns:**

True if the INI file was successfully saved, False otherwise.


Saves the INI file with the given path and content.


This function saves the current INI data to a file at the specified path. It uses the SaveFile method of the m\_Ini object, which writes the contents of the INI structure into the file. The function returns true if the save operation was successful (indicated by SI\_OK return code), and false otherwise.




**Returns:**

True if the save operation was successful, false otherwise. 





        

<hr>



### function Write 

_Writes a key-value pair to the INI file._ 
```C++
bool AGE::IniWriter::Write (
    const std::string & Section,
    const std::string & Key,
    const std::string & Value
) 
```



This function writes a given value for a specific key in a specified section of an INI file. The operation is successful if the key was not present and has been inserted, or if the key was already present and has been updated.




**Parameters:**


* `Section` The name of the section to write into. 
* `Key` The key to be written. 
* `Value` The value to be associated with the given key.



**Returns:**

True if the operation is successful (key was inserted or updated), false otherwise.


Writes a key-value pair to an INI file.


This function writes the provided value for the given key in the specified section of the INI file. The function returns true if the operation was successful, false otherwise.




**Parameters:**


* `Section` The name of the section where the key-value pair will be written. 
* `Key` The key that will be associated with the provided value. 
* `Value` The value to be written for the given key in the specified section.



**Returns:**

True if the operation was successful, false otherwise. 





        

<hr>



### function ~IniWriter 

_Destructor for the_ [_**IniWriter**_](class_a_g_e_1_1_ini_writer.md) _class._
```C++
AGE::IniWriter::~IniWriter () = default
```



This function is responsible for releasing any resources that were acquired by the [**IniWriter**](class_a_g_e_1_1_ini_writer.md) object, such as memory or file handles. It does not return anything and has no parameters.


Default destructor for the [**IniWriter**](class_a_g_e_1_1_ini_writer.md) class.


This function is responsible for freeing any resources that were allocated by the [**IniWriter**](class_a_g_e_1_1_ini_writer.md) object, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/IniWriter.h`

