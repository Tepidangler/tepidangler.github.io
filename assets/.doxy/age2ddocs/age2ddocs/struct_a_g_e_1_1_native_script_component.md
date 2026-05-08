

# Struct AGE::NativeScriptComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  void(\* | [**DestroyScript**](#variable-destroyscript)  <br> |
|  [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* | [**Instance**](#variable-instance)   = `nullptr`<br> |
|  [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \*(\* | [**InstantiateScript**](#variable-instantiatescript)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Bind**](#function-bind) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable DestroyScript 

```C++
void(* AGE::NativeScriptComponent::DestroyScript) (NativeScriptComponent *);
```




<hr>



### variable Instance 

```C++
ScriptableEntity* AGE::NativeScriptComponent::Instance;
```




<hr>



### variable InstantiateScript 

```C++
ScriptableEntity *(* AGE::NativeScriptComponent::InstantiateScript) ();
```




<hr>
## Public Functions Documentation




### function Bind 

```C++
template<typename T>
inline void AGE::NativeScriptComponent::Bind () 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::NativeScriptComponent::Deserialize (
    DataReader * Serializer,
    NativeScriptComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::NativeScriptComponent::Serialize (
    DataWriter * Serializer,
    const NativeScriptComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

