

# Struct AGE::ProjectInfo



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ProjectInfo**](struct_a_g_e_1_1_project_info.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; | [**ActionBindings**](#variable-actionbindings)  <br> |
|  uint16\_t | [**AudioEngine**](#variable-audioengine)   = `0`<br> |
|  std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; | [**AxisBindings**](#variable-axisbindings)  <br> |
|  std::vector&lt; std::filesystem::path &gt; | [**BuiltScenes**](#variable-builtscenes)  <br> |
|  std::filesystem::path | [**ConfigFilepath**](#variable-configfilepath)  <br> |
|  std::filesystem::path | [**QuestFilepath**](#variable-questfilepath)  <br> |
|  int | [**Renderer**](#variable-renderer)   = `1`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**SetQuestFilepath**](#function-setquestfilepath) (const std::filesystem::path & Filepath) <br>_Sets the quest file path._  |
|  void | [**UpdateActionBindings**](#function-updateactionbindings) (const std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; & Bindings) <br>_Updates the action bindings with new input bindings._  |
|  void | [**UpdateAxisBindings**](#function-updateaxisbindings) (const std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; & Bindings) <br>_Updates the Axis bindings with new input bindings._  |




























## Public Attributes Documentation




### variable ActionBindings 

```C++
std::vector<Ref<InputBinding> > AGE::ProjectInfo::ActionBindings;
```




<hr>



### variable AudioEngine 

```C++
uint16_t AGE::ProjectInfo::AudioEngine;
```




<hr>



### variable AxisBindings 

```C++
std::vector<Ref<InputBinding> > AGE::ProjectInfo::AxisBindings;
```




<hr>



### variable BuiltScenes 

```C++
std::vector<std::filesystem::path> AGE::ProjectInfo::BuiltScenes;
```




<hr>



### variable ConfigFilepath 

```C++
std::filesystem::path AGE::ProjectInfo::ConfigFilepath;
```




<hr>



### variable QuestFilepath 

```C++
std::filesystem::path AGE::ProjectInfo::QuestFilepath;
```




<hr>



### variable Renderer 

```C++
int AGE::ProjectInfo::Renderer;
```




<hr>
## Public Functions Documentation




### function SetQuestFilepath 

_Sets the quest file path._ 
```C++
inline void AGE::ProjectInfo::SetQuestFilepath (
    const std::filesystem::path & Filepath
) 
```



This function sets the QuestFilepath member variable to a new value, which represents the path of the quest file. The parameter 'Filepath' is used as input for setting this member variable.




**Parameters:**


* `Filepath` A const reference to std::filesystem::path representing the new quest file path. 




        

<hr>



### function UpdateActionBindings 

_Updates the action bindings with new input bindings._ 
```C++
inline void AGE::ProjectInfo::UpdateActionBindings (
    const std::vector< Ref< InputBinding > > & Bindings
) 
```



This function takes a vector of references to [**InputBinding**](struct_a_g_e_1_1_input_binding.md) objects and appends them to the existing ActionBindings list. The purpose is to update or extend the current set of actions that can be performed by the user.




**Parameters:**


* `Bindings` A constant reference to a vector of [**InputBinding**](struct_a_g_e_1_1_input_binding.md) objects, which represent new bindings to add. Each element in this vector represents an action and its associated input binding.



**Returns:**

void No return value is expected as all changes are made directly on the ActionBindings list. 





        

<hr>



### function UpdateAxisBindings 

_Updates the Axis bindings with new input bindings._ 
```C++
inline void AGE::ProjectInfo::UpdateAxisBindings (
    const std::vector< Ref< InputBinding > > & Bindings
) 
```



This function takes a vector of [**InputBinding**](struct_a_g_e_1_1_input_binding.md) references and adds them to the existing Axis Bindings. The new bindings are appended at the end of the current list.




**Parameters:**


* `Bindings` - A const reference to a std::vector of [**InputBinding**](struct_a_g_e_1_1_input_binding.md) references. Each element in this vector represents an input binding that will be added to the existing set of axis bindings.



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Project/Public/Project.h`

