

# Class AGE::Project



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Project**](class_a_g_e_1_1_project.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**AddBuiltScenes**](#function-addbuiltscenes) () <br> |
|  [**ProjectConfig**](struct_a_g_e_1_1_project_config.md) & | [**GetConfig**](#function-getconfig) () <br> |
|  [**ProjectInfo**](struct_a_g_e_1_1_project_info.md) & | [**GetInfo**](#function-getinfo) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**CompileProject**](#function-compileproject) () <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**GetActive**](#function-getactive) () <br> |
|  std::filesystem::path | [**GetAssetDirectory**](#function-getassetdirectory) () <br> |
|  std::filesystem::path | [**GetAssetFileSystemPath**](#function-getassetfilesystempath) (const std::filesystem::path & Path) <br> |
|  std::filesystem::path | [**GetConfigDirectory**](#function-getconfigdirectory) () <br> |
|  const std::filesystem::path & | [**GetProjectDirectory**](#function-getprojectdirectory) () <br> |
|  std::filesystem::path | [**GetQuestDirectory**](#function-getquestdirectory) () <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**Load**](#function-load) (const std::filesystem::path & Path) <br> |
|  Ref&lt; [**Project**](class_a_g_e_1_1_project.md) &gt; | [**New**](#function-new) (const std::string & ProjectName) <br> |
|  bool | [**Package**](#function-package) (const std::filesystem::path & Path, int TargetPlatform) <br> |
|  void | [**ReadEditorConfig**](#function-readeditorconfig) (const std::filesystem::path & Path) <br> |
|  void | [**ReadProjectConfig**](#function-readprojectconfig) (const std::filesystem::path & Path) <br> |
|  bool | [**SaveActive**](#function-saveactive) (const std::filesystem::path & Path, uint16\_t AudioEngine, int Renderer, const std::filesystem::path & ScenePath, const std::filesystem::path & QuestPath=std::filesystem::path(), const std::filesystem::path & ConfigPath=std::filesystem::path()) <br> |
|  void | [**WriteEditorConfig**](#function-writeeditorconfig) (const std::filesystem::path & Path, const std::string & ProjectName) <br> |
|  void | [**WriteProjectConfig**](#function-writeprojectconfig) (const std::filesystem::path & Path, const std::string & ProjectName) <br> |


























## Public Functions Documentation




### function AddBuiltScenes 

```C++
void AGE::Project::AddBuiltScenes () 
```




<hr>



### function GetConfig 

```C++
inline ProjectConfig & AGE::Project::GetConfig () 
```




<hr>



### function GetInfo 

```C++
inline ProjectInfo & AGE::Project::GetInfo () 
```




<hr>
## Public Static Functions Documentation




### function CompileProject 

```C++
static void AGE::Project::CompileProject () 
```




<hr>



### function GetActive 

```C++
static inline Ref< Project > AGE::Project::GetActive () 
```




<hr>



### function GetAssetDirectory 

```C++
static inline std::filesystem::path AGE::Project::GetAssetDirectory () 
```




<hr>



### function GetAssetFileSystemPath 

```C++
static inline std::filesystem::path AGE::Project::GetAssetFileSystemPath (
    const std::filesystem::path & Path
) 
```




<hr>



### function GetConfigDirectory 

```C++
static inline std::filesystem::path AGE::Project::GetConfigDirectory () 
```




<hr>



### function GetProjectDirectory 

```C++
static inline const std::filesystem::path & AGE::Project::GetProjectDirectory () 
```




<hr>



### function GetQuestDirectory 

```C++
static inline std::filesystem::path AGE::Project::GetQuestDirectory () 
```




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

```C++
static void AGE::Project::ReadEditorConfig (
    const std::filesystem::path & Path
) 
```




<hr>



### function ReadProjectConfig 

```C++
static void AGE::Project::ReadProjectConfig (
    const std::filesystem::path & Path
) 
```




<hr>



### function SaveActive 

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




<hr>



### function WriteEditorConfig 

```C++
static void AGE::Project::WriteEditorConfig (
    const std::filesystem::path & Path,
    const std::string & ProjectName
) 
```




<hr>



### function WriteProjectConfig 

```C++
static void AGE::Project::WriteProjectConfig (
    const std::filesystem::path & Path,
    const std::string & ProjectName
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Project/Public/Project.h`

