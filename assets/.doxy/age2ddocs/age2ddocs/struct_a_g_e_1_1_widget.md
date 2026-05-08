

# Struct AGE::Widget



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Widget**](struct_a_g_e_1_1_widget.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  void(\* | [**DestroyScript**](#variable-destroyscript)  <br> |
|  [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) \* | [**Instance**](#variable-instance)   = `nullptr`<br> |
|  [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) \*(\* | [**InstantiateScript**](#variable-instantiatescript)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Bind**](#function-bind) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**Widget**](struct_a_g_e_1_1_widget.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Widget**](struct_a_g_e_1_1_widget.md) & Data) <br> |


























## Public Attributes Documentation




### variable DestroyScript 

```C++
void(* AGE::Widget::DestroyScript) (Widget *);
```




<hr>



### variable Instance 

```C++
ScriptableWidget* AGE::Widget::Instance;
```




<hr>



### variable InstantiateScript 

```C++
ScriptableWidget *(* AGE::Widget::InstantiateScript) ();
```




<hr>
## Public Functions Documentation




### function Bind 

```C++
template<typename T>
inline void AGE::Widget::Bind () 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::Widget::Deserialize (
    DataReader * Serializer,
    Widget & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::Widget::Serialize (
    DataWriter * Serializer,
    const Widget & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/Widget.h`

