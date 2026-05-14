

# Struct AGE::TagComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TagComponent**](struct_a_g_e_1_1_tag_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**Tag**](#variable-tag)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**TagComponent**](#function-tagcomponent-13) () = default<br>_Default constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._ |
|   | [**TagComponent**](#function-tagcomponent-23) (const [**TagComponent**](struct_a_g_e_1_1_tag_component.md) &) = default<br>_Default copy constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._ |
|   | [**TagComponent**](#function-tagcomponent-33) (const std::string T) <br>_Constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._ |




























## Public Attributes Documentation




### variable Tag 

```C++
std::string AGE::TagComponent::Tag;
```




<hr>
## Public Functions Documentation




### function TagComponent [1/3]

_Default constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._
```C++
AGE::TagComponent::TagComponent () = default
```




<hr>



### function TagComponent [2/3]

_Default copy constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._
```C++
AGE::TagComponent::TagComponent (
    const TagComponent &
) = default
```



This function is used to create a new instance of the [**TagComponent**](struct_a_g_e_1_1_tag_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The existing [**TagComponent**](struct_a_g_e_1_1_tag_component.md) instance to copy. 




        

<hr>



### function TagComponent [3/3]

_Constructor for the_ [_**TagComponent**_](struct_a_g_e_1_1_tag_component.md) _class._
```C++
inline AGE::TagComponent::TagComponent (
    const std::string T
) 
```



This constructor initializes a new instance of the [**TagComponent**](struct_a_g_e_1_1_tag_component.md) class with a given tag string. The tag is set during object creation and cannot be changed afterwards.




**Parameters:**


* `T` A const reference to a std::string representing the tag. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

