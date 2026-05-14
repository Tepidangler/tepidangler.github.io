

# Struct AGE::MovementComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MovementComponent**](struct_a_g_e_1_1_movement_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**Speed**](#variable-speed)   = `.5f`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**MovementComponent**](#function-movementcomponent-12) () = default<br>_Default constructor for the_ [_**MovementComponent**_](struct_a_g_e_1_1_movement_component.md) _class._ |
|   | [**MovementComponent**](#function-movementcomponent-22) (const [**MovementComponent**](struct_a_g_e_1_1_movement_component.md) &) = default<br>_Default copy constructor for the_ [_**MovementComponent**_](struct_a_g_e_1_1_movement_component.md) _class._ |




























## Public Attributes Documentation




### variable Speed 

```C++
float AGE::MovementComponent::Speed;
```




<hr>
## Public Functions Documentation




### function MovementComponent [1/2]

_Default constructor for the_ [_**MovementComponent**_](struct_a_g_e_1_1_movement_component.md) _class._
```C++
AGE::MovementComponent::MovementComponent () = default
```



This function initializes a new instance of the [**MovementComponent**](struct_a_g_e_1_1_movement_component.md) class with default values. It does not take any parameters and returns nothing. The component is initialized to have no movement properties set.




**Returns:**

void 





        

<hr>



### function MovementComponent [2/2]

_Default copy constructor for the_ [_**MovementComponent**_](struct_a_g_e_1_1_movement_component.md) _class._
```C++
AGE::MovementComponent::MovementComponent (
    const MovementComponent &
) = default
```



This function is used to create a new instance of the [**MovementComponent**](struct_a_g_e_1_1_movement_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use the default implementation provided by the compiler.




**Parameters:**


* `other` The existing [**MovementComponent**](struct_a_g_e_1_1_movement_component.md) instance to copy. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

