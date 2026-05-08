

# Class AGE::Instrumentor



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Instrumentor**](class_a_g_e_1_1_instrumentor.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**BeginSession**](#function-beginsession) (const std::string & name, const std::string & filepath="results.json") <br> |
|  void | [**EndSession**](#function-endsession) () <br> |
|   | [**Instrumentor**](#function-instrumentor-13) (const [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) &) = delete<br> |
|   | [**Instrumentor**](#function-instrumentor-23) ([**Instrumentor**](class_a_g_e_1_1_instrumentor.md) &&) = delete<br> |
|  void | [**WriteProfile**](#function-writeprofile) (const [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) & result) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) & | [**Get**](#function-get) () <br> |


























## Public Functions Documentation




### function BeginSession 

```C++
inline void AGE::Instrumentor::BeginSession (
    const std::string & name,
    const std::string & filepath="results.json"
) 
```




<hr>



### function EndSession 

```C++
inline void AGE::Instrumentor::EndSession () 
```




<hr>



### function Instrumentor [1/3]

```C++
AGE::Instrumentor::Instrumentor (
    const Instrumentor &
) = delete
```




<hr>



### function Instrumentor [2/3]

```C++
AGE::Instrumentor::Instrumentor (
    Instrumentor &&
) = delete
```




<hr>



### function WriteProfile 

```C++
inline void AGE::Instrumentor::WriteProfile (
    const ProfileResult & result
) 
```




<hr>
## Public Static Functions Documentation




### function Get 

```C++
static inline Instrumentor & AGE::Instrumentor::Get () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Debug/Public/Instrumentor.h`

