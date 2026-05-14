

# Class AGE::Project



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Project**](class_a_g_e_1_1_project.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**AddBuiltScenes**](#function-addbuiltscenes) () <br> |
|  [**ProjectConfig**](struct_a_g_e_1_1_project_config.md) & | [**GetConfig**](#function-getconfig) () <br>_This function returns the project configuration object._  |
|  [**ProjectInfo**](struct_a_g_e_1_1_project_info.md) & | [**GetInfo**](#function-getinfo) () <br>_Returns the_ [_**ProjectInfo**_](struct_a_g_e_1_1_project_info.md) _object associated with this class instance._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**CompileProject**](#function-compileproject) () <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**GetActive**](#function-getactive) () <br>_This function returns the currently active project._  |
|  std::filesystem::path | [**GetAssetDirectory**](#function-getassetdirectory) () <br>_Returns the path to the asset directory of the active project._  |
|  std::filesystem::path | [**GetAssetFileSystemPath**](#function-getassetfilesystempath) (const std::filesystem::path & Path) <br>_Returns the filesystem path for an asset._  |
|  std::filesystem::path | [**GetConfigDirectory**](#function-getconfigdirectory) () <br>_Returns the path to the configuration directory of the active project._  |
|  const std::filesystem::path & | [**GetProjectDirectory**](#function-getprojectdirectory) () <br>_Returns the project directory._  |
|  std::filesystem::path | [**GetQuestDirectory**](#function-getquestdirectory) () <br>_This function returns the directory path of the quest file for the active project._  |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**Load**](#function-load) (const std::filesystem::path & Path) <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**New**](#function-new) (const std::string & ProjectName) <br> |
|  bool | [**Package**](#function-package) (const std::filesystem::path & Path, int TargetPlatform) <br> |
|  void | [**ReadEditorConfig**](#function-readeditorconfig) (const std::filesystem::path & Path) <br>_Reads editor configuration from an INI file._  |
|  void | [**ReadProjectConfig**](#function-readprojectconfig) (const std::filesystem::path & Path) <br>_Reads the project configuration from an INI file and updates the_ [_**AppConfig**_](struct_a_g_e_1_1_app_config.md) _object accordingly._ |
|  bool | [**SaveActive**](#function-saveactive) (const std::filesystem::path & Path, uint16\_t AudioEngine, int Renderer, const std::filesystem::path & ScenePath, const std::filesystem::path & QuestPath=std::filesystem::path(), const std::filesystem::path & ConfigPath=std::filesystem::path()) <br>_Saves the active project to a specified path with various configuration options._  |
|  void | [**WriteEditorConfig**](#function-writeeditorconfig) (const std::filesystem::path & Path, const std::string & ProjectName) <br>_This function writes an EditorConfig file for a project at the specified path._  |
|  void | [**WriteProjectConfig**](#function-writeprojectconfig) (const std::filesystem::path & Path, const std::string & ProjectName) <br>_This function writes project configuration to an INI file._  |


























## Public Functions Documentation




### function AddBuiltScenes 

```C++
void AGE::Project::AddBuiltScenes () 
```




<hr>



### function GetConfig 

_This function returns the project configuration object._ 
```C++
inline ProjectConfig & AGE::Project::GetConfig () 
```





**Returns:**

A reference to the [**ProjectConfig**](struct_a_g_e_1_1_project_config.md) object. 





        

<hr>



### function GetInfo 

_Returns the_ [_**ProjectInfo**_](struct_a_g_e_1_1_project_info.md) _object associated with this class instance._
```C++
inline ProjectInfo & AGE::Project::GetInfo () 
```





**Returns:**

A reference to the [**ProjectInfo**](struct_a_g_e_1_1_project_info.md) object. 





        

<hr>
## Public Static Functions Documentation




### function CompileProject 

```C++
static void AGE::Project::CompileProject () 
```




<hr>



### function GetActive 

_This function returns the currently active project._ 
```C++
static inline Ref< Project > AGE::Project::GetActive () 
```





**Returns:**

A reference to the current [**Project**](class_a_g_e_1_1_project.md) object. If no project is currently active, this will be a nullptr. 





        

<hr>



### function GetAssetDirectory 

_Returns the path to the asset directory of the active project._ 
```C++
static inline std::filesystem::path AGE::Project::GetAssetDirectory () 
```



This function retrieves the path to the asset directory of the currently active project. It first asserts that there is an active project, and if not, it throws an error message "No Active Project!". Then it returns the path by appending the asset directory name from the active project's configuration to the project directory.




**Returns:**

std::filesystem::path The path to the asset directory of the active project. 





        

<hr>



### function GetAssetFileSystemPath 

_Returns the filesystem path for an asset._ 
```C++
static inline std::filesystem::path AGE::Project::GetAssetFileSystemPath (
    const std::filesystem::path & Path
) 
```



This function takes a relative path to an asset and returns its full filesystem path, based on the active project's directory. The provided path is appended to the asset directory of the active project.




**Parameters:**


* `Path` A const reference to the relative path to the asset. 



**Returns:**

std::filesystem::path Returns the complete filesystem path for the given asset. 





        

<hr>



### function GetConfigDirectory 

_Returns the path to the configuration directory of the active project._ 
```C++
static inline std::filesystem::path AGE::Project::GetConfigDirectory () 
```



This function retrieves the path to the configuration directory of the currently active project. It first checks if there is an active project by verifying that `s_ActiveProject` is not null, and throws an exception with a message "No Active Project!" if it's null. Then, it returns the path to the configuration file of the active project relative to the project directory using the '/' operator from the C++17 filesystem library.




**Returns:**

std::filesystem::path The path to the configuration directory. 





        

<hr>



### function GetProjectDirectory 

_Returns the project directory._ 
```C++
static inline const std::filesystem::path & AGE::Project::GetProjectDirectory () 
```



This function returns a reference to the filesystem path of the active project's directory. It is crucial for any operations related to files and directories within the project.




**Returns:**

A constant reference to the filesystem path of the active project's directory. 





        

<hr>



### function GetQuestDirectory 

_This function returns the directory path of the quest file for the active project._ 
```C++
static inline std::filesystem::path AGE::Project::GetQuestDirectory () 
```



The function first checks if there is an active project by verifying that s\_ActiveProject is not nullptr. If no active project exists, it throws an assertion error with a message "No Active Project!". It then retrieves the directory path of the quest file from the active project's information and returns this path. The function uses the '/' operator to concatenate the project directory path and the quest filepath.




**Returns:**

std::filesystem::path The directory path of the quest file for the active project. 





        

<hr>



### function Load 

```C++
static Ref< Project > AGE::Project::Load (
    const std::filesystem::path & Path
) 
```




<hr>



### function New 

```C++
static Ref< Project > AGE::Project::New (
    const std::string & ProjectName
) 
```




<hr>



### function Package 

```C++
static bool AGE::Project::Package (
    const std::filesystem::path & Path,
    int TargetPlatform
) 
```




<hr>



### function ReadEditorConfig 

_Reads editor configuration from an INI file._ 
```C++
static void AGE::Project::ReadEditorConfig (
    const std::filesystem::path & Path
) 
```





**Parameters:**


* `Path` The path to the INI file. 



**Returns:**

void


Reads and parses the EditorConfig file to get configuration settings for paths like LogPath and EditorAssetsPath.


This function reads an INI-style config file located at a given path, which is expected to be in the same directory as the executable. The config file should contain sections named "Paths" with keys "LogPath" and "EditorAssetsPath". If these keys have multiple values (indicated by `HasMulti`), they are read into vectors; otherwise, their single value is directly assigned to the corresponding fields in `AppConfig`.




**Parameters:**


* `Path` The path to the config file. 




        

<hr>



### function ReadProjectConfig 

_Reads the project configuration from an INI file and updates the_ [_**AppConfig**_](struct_a_g_e_1_1_app_config.md) _object accordingly._
```C++
static void AGE::Project::ReadProjectConfig (
    const std::filesystem::path & Path
) 
```



This function reads a set of paths for various parts of the game project, such as content, source code, shaders, and scenes. It uses an `IniReader` to read the values from the specified path in the filesystem. The configuration data is then used to update the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object. If multiple entries exist for a particular key (e.g., "GameContentPath"), all of them are stored as a vector of strings.




**Parameters:**


* `Path` The path to the INI file containing the project configuration data.

Reads the project configuration from an INI file located at a given path.


This function reads and parses the INI file located at the provided path, which is expected to contain paths for various game resources such as content, source code, shaders, etc. The parsed data is then used to set the corresponding properties in the [**AppConfig**](struct_a_g_e_1_1_app_config.md) object.




**Parameters:**


* `Path` The filesystem path of the INI file to read from. 




        

<hr>



### function SaveActive 

_Saves the active project to a specified path with various configuration options._ 
```C++
static bool AGE::Project::SaveActive (
    const std::filesystem::path & Path,
    uint16_t AudioEngine,
    int Renderer,
    const std::filesystem::path & ScenePath,
    const std::filesystem::path & QuestPath=std::filesystem::path(),
    const std::filesystem::path & ConfigPath=std::filesystem::path()
) 
```



This function serializes the current active project into a file at the given path, along with additional configurations such as audio engine, renderer, start scene, quest filepath and config filepath. It also adds built-in scenes if they haven't been added before.




**Parameters:**


* `Path` The path where to save the project. 
* [**AudioEngine**](class_a_g_e_1_1_audio_engine.md) The audio engine to be used for rendering audio in the project. 
* [**Renderer**](class_a_g_e_1_1_renderer.md) The renderer to be used for rendering graphics in the project. 
* `ScenePath` The path of the start scene file. 
* `QuestPath` The path of the quest file. 
* `ConfigPath` The path of the config file.



**Returns:**

Returns true if the serialization was successful, false otherwise. 





        

<hr>



### function WriteEditorConfig 

_This function writes an EditorConfig file for a project at the specified path._ 
```C++
static void AGE::Project::WriteEditorConfig (
    const std::filesystem::path & Path,
    const std::string & ProjectName
) 
```



The function takes two parameters, `Path` and `ProjectName`. It generates an INI configuration file named "EditorConfig.ini" in the directory pointed to by `Path`. The generated config includes paths for Logs ("/{ProjectName}/Logs/") and Editor Assets ("//{CWD}/Assets/"). Here, {ProjectName} is replaced with the actual project name provided as an argument and {CWD} stands for the current working directory. The function does not return anything, so it has a void return type.




**Parameters:**


* `Path` The path where the EditorConfig file will be created. 
* `ProjectName` The name of the project to use in generating paths.

This function writes an EditorConfig file for a project.


The function takes two parameters, a path and a project name. It then writes to the specified path an EditorConfig file with two sections "Paths". In this section, it sets up paths for Logs and Assets of the project. 

**Parameters:**


* `Path` The path where the EditorConfig file will be written. 
* `ProjectName` The name of the project. This is used in setting up the paths. 



**Returns:**

void No return value. 





        

<hr>



### function WriteProjectConfig 

_This function writes project configuration to an INI file._ 
```C++
static void AGE::Project::WriteProjectConfig (
    const std::filesystem::path & Path,
    const std::string & ProjectName
) 
```



The function takes two parameters, a const reference to a std::filesystem::path object and a string representing the name of the project. It then creates an instance of [**IniWriter**](class_a_g_e_1_1_ini_writer.md) with the path to the ProjectConfig.ini file as its argument. This writer is used to write four key-value pairs into the INI file: "GameContentPath", "GameSourcePath", "GameShadersPath" and "GameScenesPath". The values for these keys are formatted strings that represent paths relative to the project directory, using the provided ProjectName as a variable.




**Parameters:**


* `Path` A const reference to a std::filesystem::path object representing the path to the project directory. 
* `ProjectName` A string representing the name of the project.



**Returns:**

void


Writes project configuration to an INI file.


This function writes the paths for various project components into an INI file located at the specified path. The paths written include GameContentPath, GameSourcePath, GameShadersPath and GameScenesPath.




**Parameters:**


* `Path` The path where the INI file will be saved. 
* `ProjectName` The name of the project for which to write the configuration.



**Returns:**

void No return value is expected as this function directly writes into an INI file. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Project/Public/Project.h`

