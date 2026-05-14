

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
|  void | [**Bind**](#function-bind) () <br>_Binds a new scriptable entity type to the_ [_**NativeScriptComponent**_](struct_a_g_e_1_1_native_script_component.md) _system._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md) & Data) <br>_This function deserializes data from a serialized format into the native script component._  |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md) & Data) <br>_This function serializes the given_ [_**NativeScriptComponent**_](struct_a_g_e_1_1_native_script_component.md) _into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


























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

_Binds a new scriptable entity type to the_ [_**NativeScriptComponent**_](struct_a_g_e_1_1_native_script_component.md) _system._
```C++
template<typename T>
inline void AGE::NativeScriptComponent::Bind () 
```



This function sets up the necessary functions for creating and destroying instances of a specific scriptable entity type (T). The InstantiateScript lambda creates an instance of T, while DestroyScript deletes it. These lambdas are set based on the compiler used to compile the code. If the compiler is not recognized or supported by AGE yet, an error message will be shown.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes data from a serialized format into the native script component._ 
```C++
static inline void AGE::NativeScriptComponent::Deserialize (
    DataReader * Serializer,
    NativeScriptComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to an instance of `DataReader` that provides the serialized data. 
* `Data` The reference to the `NativeScriptComponent` where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes the given_ [_**NativeScriptComponent**_](struct_a_g_e_1_1_native_script_component.md) _into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::NativeScriptComponent::Serialize (
    DataWriter * Serializer,
    const NativeScriptComponent & Data
) 
```





**Parameters:**


* `Serializer` The [**DataWriter**](class_a_g_e_1_1_data_writer.md) object to write data to. 
* `Data` The [**NativeScriptComponent**](struct_a_g_e_1_1_native_script_component.md) object to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

