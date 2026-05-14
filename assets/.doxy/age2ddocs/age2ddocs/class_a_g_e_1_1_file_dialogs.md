

# Class AGE::FileDialogs



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FileDialogs**](class_a_g_e_1_1_file_dialogs.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  std::string | [**OpenFile**](#function-openfile) (const std::string & Title, const std::filesystem::path & DefaultPath, std::vector&lt; std::string &gt; Filter) <br>_Opens a file dialog and returns the path of the selected file._  |
|  std::string | [**SaveFile**](#function-savefile) (const std::string & Title, const std::filesystem::path & DefaultPath, std::vector&lt; std::string &gt; Filter) <br>_This function opens a file dialog and allows the user to select a file for saving._  |


























## Public Static Functions Documentation




### function OpenFile 

_Opens a file dialog and returns the path of the selected file._ 
```C++
static std::string AGE::FileDialogs::OpenFile (
    const std::string & Title,
    const std::filesystem::path & DefaultPath,
    std::vector< std::string > Filter
) 
```



This function opens a file dialog with the given title, default path, and filter. If no file is selected, it returns an empty string. The returned string contains the path of the first selected file.




**Parameters:**


* `Title` The title of the file dialog. 
* `DefaultPath` The default path for the file dialog. 
* `Filter` A vector of strings representing the filter for the file dialog.



**Returns:**

Returns a string containing the path of the selected file, or an empty string if no file is selected. 





        

<hr>



### function SaveFile 

_This function opens a file dialog and allows the user to select a file for saving._ 
```C++
static std::string AGE::FileDialogs::SaveFile (
    const std::string & Title,
    const std::filesystem::path & DefaultPath,
    std::vector< std::string > Filter
) 
```





**Parameters:**


* `Title` The title of the file dialog. 
* `DefaultPath` The default path where the file dialog starts from. 
* `Filter` A vector of strings representing the types of files that can be selected in the dialog.



**Returns:**

Returns a string containing the path to the selected file, or an empty string if no file was selected. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Public/WindowsUtils.h`

