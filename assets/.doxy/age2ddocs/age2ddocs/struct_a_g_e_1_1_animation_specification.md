

# Struct AGE::AnimationSpecification



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  float | [**Height**](#variable-height)  <br> |
|  CharMovementStatus | [**MovementStatus**](#variable-movementstatus)   = `CharMovementStatus::UNDEFINED`<br> |
|  std::string | [**Name**](#variable-name)   = `""`<br> |
|  int | [**NumberOfFrames**](#variable-numberofframes)   = `0`<br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**Texture**](#variable-texture)  <br> |
|  float | [**Width**](#variable-width)  <br> |
|  bool | [**bIsReadyToLoad**](#variable-bisreadytoload)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**IsReadyToLoad**](#function-isreadytoload) () <br>_Checks if the animation is ready to be loaded._  |
|  void | [**SetIsReadyToLoad**](#function-setisreadytoload) (bool Value) <br>_Sets the value of bIsReadyToLoad variable._  |




























## Public Attributes Documentation




### variable Height 

```C++
float AGE::AnimationSpecification::Height;
```




<hr>



### variable MovementStatus 

```C++
CharMovementStatus AGE::AnimationSpecification::MovementStatus;
```




<hr>



### variable Name 

```C++
std::string AGE::AnimationSpecification::Name;
```




<hr>



### variable NumberOfFrames 

```C++
int AGE::AnimationSpecification::NumberOfFrames;
```




<hr>



### variable Texture 

```C++
Ref<Texture2D> AGE::AnimationSpecification::Texture;
```




<hr>



### variable Width 

```C++
float AGE::AnimationSpecification::Width;
```




<hr>



### variable bIsReadyToLoad 

```C++
bool AGE::AnimationSpecification::bIsReadyToLoad;
```




<hr>
## Public Functions Documentation




### function IsReadyToLoad 

_Checks if the animation is ready to be loaded._ 
```C++
inline bool AGE::AnimationSpecification::IsReadyToLoad () 
```



This function checks several conditions to determine if an animation is ready to be loaded. It first checks if `bIsReadyToLoad` is true, then verifies that the Name of the animation is not empty and that it has more than one frame. Finally, it ensures that the movement status of the character is defined. If any of these conditions are not met, an error message is logged and `bIsReadyToLoad` is set to false.




**Returns:**

True if the animation is ready to be loaded, false otherwise.


Checks if the animation is ready to be loaded.


This function checks several conditions to determine if an animation can be loaded. It first checks if `bIsReadyToLoad` is false, in which case it returns false. If `Name` is empty, it logs an error and sets `bIsReadyToLoad` to false before returning false. If the number of frames is not greater than 1, it also logs an error and sets `bIsReadyToLoad` to false. Finally, if `MovementStatus` is undefined, it logs an error and sets `bIsReadyToLoad` to false. In all other cases, it returns true.




**Returns:**

True if the animation can be loaded, false otherwise. 





        

<hr>



### function SetIsReadyToLoad 

_Sets the value of bIsReadyToLoad variable._ 
```C++
inline void AGE::AnimationSpecification::SetIsReadyToLoad (
    bool Value
) 
```



This function sets the boolean variable 'bIsReadyToLoad' to a given value. It is used to indicate whether the system is ready to load data or not.




**Parameters:**


* `Value` The new value for bIsReadyToLoad, which can be either true (indicating readiness) or false (indicating non-readiness).

Sets the state of Ready to Load.


This function sets the value of bIsReadyToLoad variable, which indicates whether the system is ready to load data or not.




**Parameters:**


* `Value` The new boolean value for bIsReadyToLoad. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Animation/Public/Animation.h`

