

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
|  void | [**SetQuestFilepath**](#function-setquestfilepath) (const std::filesystem::path & Filepath) <br> |
|  void | [**UpdateActionBindings**](#function-updateactionbindings) (const std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; & Bindings) <br> |
|  void | [**UpdateAxisBindings**](#function-updateaxisbindings) (const std::vector&lt; Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; &gt; & Bindings) <br> |




























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

```C++
inline void AGE::ProjectInfo::SetQuestFilepath (
    const std::filesystem::path & Filepath
) 
```




<hr>



### function UpdateActionBindings 

```C++
inline void AGE::ProjectInfo::UpdateActionBindings (
    const std::vector< Ref< InputBinding > > & Bindings
) 
```




<hr>



### function UpdateAxisBindings 

```C++
inline void AGE::ProjectInfo::UpdateAxisBindings (
    const std::vector< Ref< InputBinding > > & Bindings
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Project/Public/Project.h`

