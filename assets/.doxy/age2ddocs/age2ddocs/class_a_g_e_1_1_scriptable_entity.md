

# Class AGE::ScriptableEntity



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md)








Inherits the following classes: std::enable_shared_from_this< ScriptableEntity >


































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddBeginPlayFunctions**](#function-addbeginplayfunctions) ([**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md), [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; Func) <br> |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br> |
| virtual void | [**AddTickFunctions**](#function-addtickfunctions) ([**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md), [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; Func) <br> |
| virtual void | [**ClearFunctions**](#function-clearfunctions) () <br> |
|  T & | [**GetComponent**](#function-getcomponent) () <br> |
| virtual [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetID**](#function-getid) () <br> |
| virtual [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetLocation**](#function-getlocation) () <br> |
| virtual std::string | [**GetName**](#function-getname) () <br> |
| virtual std::string | [**GetScriptableEntityType**](#function-getscriptableentitytype) () <br> |
| virtual bool | [**IsCharacter**](#function-ischaracter) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
| virtual void | [**OnHit**](#function-onhit) () <br> |
| virtual void | [**OnOverlapStart**](#function-onoverlapstart) () <br> |
| virtual void | [**OnOverlapStop**](#function-onoverlapstop) () <br> |
| virtual void | [**SetLocation**](#function-setlocation) (const [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) & Location) <br> |
| virtual  | [**~ScriptableEntity**](#function-scriptableentity) () <br> |
























## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual [**Entity**](class_a_g_e_1_1_entity.md) & | [**GetEntityHandle**](#function-getentityhandle) () <br> |
| virtual void | [**OnBeginPlay**](#function-onbeginplay) () <br> |
| virtual void | [**OnCreate**](#function-oncreate) () <br> |
| virtual void | [**OnDestroy**](#function-ondestroy) () <br> |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**PushComp**](#function-pushcomp) () <br> |
| virtual void | [**Reset**](#function-reset) () <br> |




## Public Functions Documentation




### function AddBeginPlayFunctions 

```C++
inline virtual void AGE::ScriptableEntity::AddBeginPlayFunctions (
    AGEFunction < AGENode , ScriptableEntity > Func
) 
```




<hr>



### function AddComponent 

```C++
template<typename T, typename ... Args>
inline T & AGE::ScriptableEntity::AddComponent (
    Args &&... args
) 
```




<hr>



### function AddTickFunctions 

```C++
inline virtual void AGE::ScriptableEntity::AddTickFunctions (
    AGEFunction < AGENode , ScriptableEntity > Func
) 
```




<hr>



### function ClearFunctions 

```C++
inline virtual void AGE::ScriptableEntity::ClearFunctions () 
```




<hr>



### function GetComponent 

```C++
template<typename T>
inline T & AGE::ScriptableEntity::GetComponent () 
```





**Template parameters:**


* `T` - Represents Component within the [**Entity**](class_a_g_e_1_1_entity.md) Component System 



**Return value:**


* `-` T 



**Author:**

De'Lano Wilcox 





        

<hr>



### function GetID 

```C++
inline virtual UUID AGE::ScriptableEntity::GetID () 
```




<hr>



### function GetLocation 

```C++
inline virtual Vector3 AGE::ScriptableEntity::GetLocation () 
```




<hr>



### function GetName 

```C++
inline virtual std::string AGE::ScriptableEntity::GetName () 
```




<hr>



### function GetScriptableEntityType 

```C++
inline virtual std::string AGE::ScriptableEntity::GetScriptableEntityType () 
```




<hr>



### function IsCharacter 

```C++
inline virtual bool AGE::ScriptableEntity::IsCharacter () 
```





**Return value:**


* `-` bool 



**Author:**

De'Lano Wilcox 





        

<hr>



### function OnEvent 

```C++
inline virtual void AGE::ScriptableEntity::OnEvent (
    Event & E
) 
```




<hr>



### function OnHit 

```C++
inline virtual void AGE::ScriptableEntity::OnHit () 
```




<hr>



### function OnOverlapStart 

```C++
inline virtual void AGE::ScriptableEntity::OnOverlapStart () 
```




<hr>



### function OnOverlapStop 

```C++
inline virtual void AGE::ScriptableEntity::OnOverlapStop () 
```




<hr>



### function SetLocation 

```C++
inline virtual void AGE::ScriptableEntity::SetLocation (
    const AGE::Vector3 & Location
) 
```




<hr>



### function ~ScriptableEntity 

```C++
inline virtual AGE::ScriptableEntity::~ScriptableEntity () 
```




<hr>
## Protected Functions Documentation




### function GetEntityHandle 

```C++
inline virtual Entity & AGE::ScriptableEntity::GetEntityHandle () 
```




<hr>



### function OnBeginPlay 

```C++
inline virtual void AGE::ScriptableEntity::OnBeginPlay () 
```




<hr>



### function OnCreate 

```C++
inline virtual void AGE::ScriptableEntity::OnCreate () 
```




<hr>



### function OnDestroy 

```C++
inline virtual void AGE::ScriptableEntity::OnDestroy () 
```




<hr>



### function OnUpdate 

```C++
inline virtual void AGE::ScriptableEntity::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function PushComp 

```C++
virtual void AGE::ScriptableEntity::PushComp () 
```




<hr>



### function Reset 

```C++
inline virtual void AGE::ScriptableEntity::Reset () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/ScriptableEntity.h`

