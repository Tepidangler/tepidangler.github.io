

# Struct AGE::UIComponentType



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum uint16\_t | [**Value**](#enum-value)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|  std::string & | [**ToString**](#function-tostring-14) () <br> |
|  std::string | [**ToString**](#function-tostring-24) () const<br> |
|  std::string | [**ToString**](#function-tostring-34) (Value Val) <br> |
|  std::string | [**ToString**](#function-tostring-44) (Value Val) const<br> |
|  Value | [**ToValue**](#function-tovalue-12) () <br> |
|  Value | [**ToValue**](#function-tovalue-22) () const<br> |
|   | [**UIComponentType**](#function-uicomponenttype-12) () = default<br> |
|   | [**UIComponentType**](#function-uicomponenttype-22) (Value Val) <br> |
|  constexpr | [**operator Value**](#function-operator-value) () const<br> |
|   | [**operator bool**](#function-operator-bool) () const<br> |
|   | [**string**](#function-string) () const<br> |
|  bool | [**operator!=**](#function-operator) ([**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) a) const<br> |
|  std::string | [**operator()**](#function-operator_1) (Value Val) const<br> |
|  bool | [**operator==**](#function-operator_2) ([**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) a) const<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) & Instance) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) & Instance) <br> |


























## Public Types Documentation




### enum Value 

```C++
enum AGE::UIComponentType::Value {
    TextComponent,
    TextBoxComponent,
    HorizontalBoxComponent,
    VerticalBoxComponent,
    ButtonComponent,
    ImageComponent
};
```




<hr>
## Public Functions Documentation




### function ToString [1/4]

```C++
inline std::string & AGE::UIComponentType::ToString () 
```




<hr>



### function ToString [2/4]

```C++
inline std::string AGE::UIComponentType::ToString () const
```




<hr>



### function ToString [3/4]

```C++
inline std::string AGE::UIComponentType::ToString (
    Value Val
) 
```




<hr>



### function ToString [4/4]

```C++
inline std::string AGE::UIComponentType::ToString (
    Value Val
) const
```




<hr>



### function ToValue [1/2]

```C++
inline Value AGE::UIComponentType::ToValue () 
```




<hr>



### function ToValue [2/2]

```C++
inline Value AGE::UIComponentType::ToValue () const
```




<hr>



### function UIComponentType [1/2]

```C++
AGE::UIComponentType::UIComponentType () = default
```




<hr>



### function UIComponentType [2/2]

```C++
inline AGE::UIComponentType::UIComponentType (
    Value Val
) 
```




<hr>



### function operator Value 

```C++
inline constexpr AGE::UIComponentType::operator Value () const
```




<hr>



### function operator bool 

```C++
explicit AGE::UIComponentType::operator bool () const
```




<hr>



### function string 

```C++
inline AGE::UIComponentType::string () const
```




<hr>



### function operator!= 

```C++
inline bool AGE::UIComponentType::operator!= (
    UIComponentType a
) const
```




<hr>



### function operator() 

```C++
inline std::string AGE::UIComponentType::operator() (
    Value Val
) const
```




<hr>



### function operator== 

```C++
inline bool AGE::UIComponentType::operator== (
    UIComponentType a
) const
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::UIComponentType::Deserialize (
    DataReader * Serializer,
    UIComponentType & Instance
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::UIComponentType::Serialize (
    DataWriter * Serializer,
    const UIComponentType & Instance
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/UIStructs.h`

