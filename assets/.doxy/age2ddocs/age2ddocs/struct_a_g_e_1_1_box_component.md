

# Struct AGE::BoxComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**BoxComponent**](struct_a_g_e_1_1_box_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**Color**](#variable-color)   = `{ 1.f }`<br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Texture**](#variable-texture)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**BoxComponent**](#function-boxcomponent-12) () = default<br>_Default constructor for the_ [_**BoxComponent**_](struct_a_g_e_1_1_box_component.md) _class._ |
|   | [**BoxComponent**](#function-boxcomponent-22) (const [**BoxComponent**](struct_a_g_e_1_1_box_component.md) &) = default<br>_Default copy constructor for the_ [_**BoxComponent**_](struct_a_g_e_1_1_box_component.md) _class._ |




























## Public Attributes Documentation




### variable Color 

```C++
Vector4 AGE::BoxComponent::Color;
```




<hr>



### variable Texture 

```C++
Ref<Texture2D> AGE::BoxComponent::Texture;
```




<hr>
## Public Functions Documentation




### function BoxComponent [1/2]

_Default constructor for the_ [_**BoxComponent**_](struct_a_g_e_1_1_box_component.md) _class._
```C++
AGE::BoxComponent::BoxComponent () = default
```




<hr>



### function BoxComponent [2/2]

_Default copy constructor for the_ [_**BoxComponent**_](struct_a_g_e_1_1_box_component.md) _class._
```C++
AGE::BoxComponent::BoxComponent (
    const BoxComponent &
) = default
```



This function is used to create a new instance of the [**BoxComponent**](struct_a_g_e_1_1_box_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The [**BoxComponent**](struct_a_g_e_1_1_box_component.md) object to be copied. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

