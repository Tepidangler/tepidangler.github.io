

# Struct AGE::AGEFunction

**template &lt;typename R, typename E&gt;**



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; rttr::variant &gt; | [**Args**](#variable-args)  <br> |
|  E \* | [**Entt**](#variable-entt)  <br> |
|  uint64\_t | [**EnttID**](#variable-enttid)  <br> |
|  uint64\_t | [**RefID**](#variable-refid)  <br> |
|  Ref&lt; R &gt; | [**Reference**](#variable-reference)  <br> |
|  std::string | [**Val**](#variable-val)  <br> |
|  bool | [**bIsUtilFunction**](#variable-bisutilfunction)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEFunction**](#function-agefunction-13) () = default<br> |
|   | [**AGEFunction**](#function-agefunction-23) (const std::string & Exec, std::vector&lt; rttr::variant &gt; Arguments, E \* Value=nullptr, Ref&lt; R &gt; & Ptr=nullptr) <br> |
|   | [**AGEFunction**](#function-agefunction-33) (const [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) &) = default<br> |
|  rttr::variant | [**Execute**](#function-execute) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime=0.f) <br> |
| virtual  | [**~AGEFunction**](#function-agefunction) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) & Data) <br> |






















## Protected Functions

| Type | Name |
| ---: | :--- |
|  rttr::variant | [**Function**](#function-function) (Ref&lt; R &gt; & Ptr, [**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime=0.f) <br> |




## Public Attributes Documentation




### variable Args 

```C++
std::vector<rttr::variant> AGE::AGEFunction< R, E >::Args;
```




<hr>



### variable Entt 

```C++
E* AGE::AGEFunction< R, E >::Entt;
```




<hr>



### variable EnttID 

```C++
uint64_t AGE::AGEFunction< R, E >::EnttID;
```




<hr>



### variable RefID 

```C++
uint64_t AGE::AGEFunction< R, E >::RefID;
```




<hr>



### variable Reference 

```C++
Ref<R> AGE::AGEFunction< R, E >::Reference;
```




<hr>



### variable Val 

```C++
std::string AGE::AGEFunction< R, E >::Val;
```




<hr>



### variable bIsUtilFunction 

```C++
bool AGE::AGEFunction< R, E >::bIsUtilFunction;
```




<hr>
## Public Functions Documentation




### function AGEFunction [1/3]

```C++
AGE::AGEFunction::AGEFunction () = default
```




<hr>



### function AGEFunction [2/3]

```C++
inline AGE::AGEFunction::AGEFunction (
    const std::string & Exec,
    std::vector< rttr::variant > Arguments,
    E * Value=nullptr,
    Ref< R > & Ptr=nullptr
) 
```




<hr>



### function AGEFunction [3/3]

```C++
AGE::AGEFunction::AGEFunction (
    const AGEFunction &
) = default
```




<hr>



### function Execute 

```C++
inline rttr::variant AGE::AGEFunction::Execute (
    TimeStep DeltaTime=0.f
) 
```




<hr>



### function ~AGEFunction 

```C++
virtual AGE::AGEFunction::~AGEFunction () = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::AGEFunction::Deserialize (
    DataReader * Serializer,
    AGEFunction & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::AGEFunction::Serialize (
    DataWriter * Serializer,
    const AGEFunction & Data
) 
```




<hr>
## Protected Functions Documentation




### function Function 

```C++
inline rttr::variant AGE::AGEFunction::Function (
    Ref< R > & Ptr,
    TimeStep DeltaTime=0.f
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/Functions.h`

