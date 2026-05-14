

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
|  void | [**Bind**](#function-bind) () <br>_Binds a lambda function to instantiate an instance of class T. Also binds another lambda function for destroying the instance of_ [_**Widget**_](struct_a_g_e_1_1_widget.md) _._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**Widget**](struct_a_g_e_1_1_widget.md) & Data) <br>_This function deserializes data from a serialized format into an instance of the_ [_**Widget**_](struct_a_g_e_1_1_widget.md) _class._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Widget**](struct_a_g_e_1_1_widget.md) & Data) <br>_This function serializes a widget object into a data writer._  |


























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

_Binds a lambda function to instantiate an instance of class T. Also binds another lambda function for destroying the instance of_ [_**Widget**_](struct_a_g_e_1_1_widget.md) _._
```C++
template<typename T>
inline void AGE::Widget::Bind () 
```



The first lambda function creates a new instance of class T and casts it to ScriptableWidget\*. The second lambda function deletes the instance of [**Widget**](struct_a_g_e_1_1_widget.md), then sets its Instance pointer to nullptr.


Binds a lambda function to create an instance of type T and another lambda function to destroy it.


This function sets the InstantiateScript lambda to a new function that creates a new instance of type T using static\_cast. It also sets DestroyScript lambda to delete the [**Widget**](struct_a_g_e_1_1_widget.md)'s instance and set it to nullptr.




**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes data from a serialized format into an instance of the_ [_**Widget**_](struct_a_g_e_1_1_widget.md) _class._
```C++
static inline void AGE::Widget::Deserialize (
    DataReader * Serializer,
    Widget & Data
) 
```



The function takes in a pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and a reference to a [**Widget**](struct_a_g_e_1_1_widget.md) object. It does not return anything, but it modifies the [**Widget**](struct_a_g_e_1_1_widget.md) object by filling its fields with data read from the [**DataReader**](class_a_g_e_1_1_data_reader.md).




**Parameters:**


* `Serializer` A pointer to an instance of the [**DataReader**](class_a_g_e_1_1_data_reader.md) class that provides the serialized data. 
* `Data` A reference to an instance of the [**Widget**](struct_a_g_e_1_1_widget.md) class where the deserialized data will be stored.

This function deserializes data from a serialized format into an object of type [**Widget**](struct_a_g_e_1_1_widget.md).


The function takes in a pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) and a reference to a [**Widget**](struct_a_g_e_1_1_widget.md) object. It does not return anything, but it modifies the [**Widget**](struct_a_g_e_1_1_widget.md) object by filling its fields with data read from the [**DataReader**](class_a_g_e_1_1_data_reader.md).




**Parameters:**


* `Serializer` A pointer to an instance of [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 
* `Data` The [**Widget**](struct_a_g_e_1_1_widget.md) object to be filled with deserialized data. 




        

<hr>



### function Serialize 

_This function serializes a widget object into a data writer._ 
```C++
static inline void AGE::Widget::Serialize (
    DataWriter * Serializer,
    const Widget & Data
) 
```





**Parameters:**


* `Serializer` Pointer to the data writer where the widget will be written. 
* `Data` The widget that needs to be serialized.

This function serializes a widget object into a data writer.


The function takes in two parameters - a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) and a constant reference to a [**Widget**](struct_a_g_e_1_1_widget.md). It does not return anything, hence the void return type.




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for serialization. 
* `Data` A constant reference to the [**Widget**](struct_a_g_e_1_1_widget.md) object that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/Widget.h`

