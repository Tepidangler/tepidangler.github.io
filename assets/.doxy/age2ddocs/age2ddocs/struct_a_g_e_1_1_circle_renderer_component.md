

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
|   | [**CircleRendererComponent**](#function-circlerenderercomponent-12) () = default<br> |
|   | [**CircleRendererComponent**](#function-circlerenderercomponent-22) (const [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) &) = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**CircleRendererComponent**](struct_a_g_e_1_1_circle_renderer_component.md) & Data) <br> |


























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

```C++
AGE::CircleRendererComponent::CircleRendererComponent () = default
```




<hr>



### function CircleRendererComponent [2/2]

```C++
AGE::CircleRendererComponent::CircleRendererComponent (
    const CircleRendererComponent &
) = default
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::CircleRendererComponent::Deserialize (
    DataReader * Serializer,
    CircleRendererComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::CircleRendererComponent::Serialize (
    DataWriter * Serializer,
    const CircleRendererComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

