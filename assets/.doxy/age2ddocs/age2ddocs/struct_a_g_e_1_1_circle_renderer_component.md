

# Struct AGE::CircleRendererComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**Color**](#variable-color)   = `{ 1.f,1.f,1.f,1.f }`<br> |
|  float | [**Fade**](#variable-fade)   = `.005f`<br> |
|  float | [**Thickness**](#variable-thickness)   = `1.f`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**CircleRendererComponent**](#function-circlerenderercomponent-12) () = default<br>_Default constructor for the_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _class._ |
|   | [**CircleRendererComponent**](#function-circlerenderercomponent-22) (const [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) &) = default<br>_Default copy constructor for the_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _class. This function is used to create a new instance of the class by copying an existing one, which can be useful in certain situations such as when you need to pass objects around by value or return them from functions._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) & Data) <br>_This function deserializes a_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) & Data) <br>_This function serializes the data of a circle renderer component into a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


























## Public Attributes Documentation




### variable Color 

```C++
Vector4 AGE::CircleRendererComponent::Color;
```




<hr>



### variable Fade 

```C++
float AGE::CircleRendererComponent::Fade;
```




<hr>



### variable Thickness 

```C++
float AGE::CircleRendererComponent::Thickness;
```




<hr>
## Public Functions Documentation




### function CircleRendererComponent [1/2]

_Default constructor for the_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _class._
```C++
AGE::CircleRendererComponent::CircleRendererComponent () = default
```




<hr>



### function CircleRendererComponent [2/2]

_Default copy constructor for the_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _class. This function is used to create a new instance of the class by copying an existing one, which can be useful in certain situations such as when you need to pass objects around by value or return them from functions._
```C++
AGE::CircleRendererComponent::CircleRendererComponent (
    const CircleRendererComponent &
) = default
```





**Parameters:**


* `other` The existing instance of the class that will be copied. 




        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes a_ [_**CircleRendererComponent**_](struct_a_g_e_1_1_circle_renderer_component.md) _from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._
```C++
static inline void AGE::CircleRendererComponent::Deserialize (
    DataReader * Serializer,
    CircleRendererComponent & Data
) 
```



The function reads data from the serialized format and populates the given [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) with this data.




**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains the serialized data. 
* `Data` Reference to the [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes the data of a circle renderer component into a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::CircleRendererComponent::Serialize (
    DataWriter * Serializer,
    const CircleRendererComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where the data will be written. 
* `Data` The [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) whose data is being serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

