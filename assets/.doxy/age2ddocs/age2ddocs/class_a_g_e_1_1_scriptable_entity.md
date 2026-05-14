

# Class AGE::ScriptableEntity



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md)








Inherits the following classes: std::enable_shared_from_this< ScriptableEntity >


















## Public Attributes

| Type | Name |
| ---: | :--- |
|  viCOMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**AddBeginPlayFunctions**](#function-addbeginplayfunctions) ([**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md), [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; Func) <br> |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br>_This function adds a component of type T to the entity._  |
| virtual void | [**AddTickFunctions**](#function-addtickfunctions) ([**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)&lt; [**AGENode**](struct_a_g_e_1_1_a_g_e_node.md), [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) &gt; Func) <br> |
| virtual void | [**ClearFunctions**](#function-clearfunctions) () <br> |
|  T & | [**GetComponent**](#function-getcomponent) () <br>_Retrieves the component of type T from the entity._  |
|  vi rtual UU ID | [**GetID**](#function-getid) () <br>_Returns the unique identifier of the entity._  |
|  rt ual [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetLocation**](#function-getlocation) () <br>_Returns the location of an object in a three-dimensional space._  |
|  vi rtual st d::string | [**GetName**](#function-getname) () <br>_Returns the name of the object._  |
|  vi rtual st d::string | [**GetScriptableEntityType**](#function-getscriptableentitytype) () <br>_This function returns the scriptable entity type as a string._  |
|  vi rtual bo ol | [**IsCharacter**](#function-ischaracter) () <br>_Checks whether the scriptable entity is of type "Character"._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
|  vi rtual vo id | [**OnHit**](#function-onhit) () <br>_This function is called when an object gets hit by another object._  |
|  vi rtual vo id | [**OnOverlapStart**](#function-onoverlapstart) () <br>_This function is called when an overlap starts between two objects._  |
|  vi rtual vo id | [**OnOverlapStop**](#function-onoverlapstop) () <br>_This function is called when an overlap stops._  |
|  vi rtual vo id | [**SetLocation**](#function-setlocation) (const [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) & Location) <br>_Sets the location of an object._  |
|  vi rtual ~S | [**criptableEntity**](#function-criptableentity) () <br>_Virtual destructor for the_ [_**ScriptableEntity**_](class_a_g_e_1_1_scriptable_entity.md) _class._ |
























## Protected Functions

| Type | Name |
| ---: | :--- |
|  vi rtual En tity & | [**GetEntityHandle**](#function-getentityhandle) () <br>_This function returns a reference to the entity object._  |
| virtual void | [**OnBeginPlay**](#function-onbeginplay) () <br> |
| virtual void | [**OnCreate**](#function-oncreate) () <br> |
| virtual void | [**OnDestroy**](#function-ondestroy) () <br> |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
| virtual void | [**PushComp**](#function-pushcomp) () <br>_Pushes this scriptable entity into the application's scriptable component stack._  |
| virtual void | [**Reset**](#function-reset) () <br> |




## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
viCOMMENT AGE::ScriptableEntity::__pad0__;
```




<hr>
## Public Functions Documentation




### function AddBeginPlayFunctions 

```C++
inline virtual void AGE::ScriptableEntity::AddBeginPlayFunctions (
    AGEFunction < AGENode , ScriptableEntity > Func
) 
```




<hr>



### function AddComponent 

_This function adds a component of type T to the entity._ 
```C++
template<typename T, typename ... Args>
inline T & AGE::ScriptableEntity::AddComponent (
    Args &&... args
) 
```





**Template parameters:**


* `T` The type of the component to be added. 
* `Args` The types of any additional arguments required by the AddComponent method. 



**Parameters:**


* `args` Any additional arguments required by the AddComponent method. 



**Returns:**

Returns the result of calling m\_Entity's AddComponent method with template parameter T and provided arguments.


This function adds a component of type T to the entity. 

**Template parameters:**


* `T` The type of the component to be added. 
* `Args` The types of any additional arguments required by the AddComponent method. 



**Parameters:**


* `args` Any additional arguments required by the AddComponent method. 



**Returns:**

Returns the result of calling m\_Entity's AddComponent method with template parameter T and provided arguments. 





        

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

_Retrieves the component of type T from the entity._ 
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


This function retrieves a component of type T from the entity using the GetComponent method from the m\_Entity object, which is assumed to provide this functionality. If the component exists, it returns it; otherwise, it returns a default value for type T.




**Returns:**

The component of type T if it exists, or a default value for type T if it does not exist.


Gets the component of type T from the entity.


This function retrieves a component of type T from the entity. It uses the GetComponent method from the m\_Entity object, which is assumed to be an instance of some class that provides this functionality.




**Returns:**

The component of type T if it exists, otherwise it returns a default value for type T. 





        

<hr>



### function GetID 

_Returns the unique identifier of the entity._ 
```C++
inline vi rtual UU ID AGE::ScriptableEntity::GetID () 
```



This function retrieves and returns the unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)) associated with an entity. The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) is a universally unique identifier that is used to identify entities in a system.




**Returns:**

A [**UUID**](class_a_g_e_1_1_u_u_i_d.md) representing the identity of the entity.


This function returns the ID of an entity. 

**Returns:**

The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) (Universally Unique Identifier) of the entity. 





        

<hr>



### function GetLocation 

_Returns the location of an object in a three-dimensional space._ 
```C++
inline rt ual Vector3 AGE::ScriptableEntity::GetLocation () 
```





**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the location of the object. If no specific location is set, it returns a default constructed one. 





        

<hr>



### function GetName 

_Returns the name of the object._ 
```C++
inline vi rtual st d::string AGE::ScriptableEntity::GetName () 
```



This function returns a string that represents the name of the object. It is designed to be overridden in derived classes, so it will return an empty string by default.




**Returns:**

A std::string representing the name of the object. In this case, it will always return an empty string.


This function returns the name of an object. 

**Returns:**

A string representing the name of the object. In this case, it will always be an empty string as there is no specific name set for the object. 





        

<hr>



### function GetScriptableEntityType 

_This function returns the scriptable entity type as a string._ 
```C++
inline vi rtual st d::string AGE::ScriptableEntity::GetScriptableEntityType () 
```





**Returns:**

A string representing the scriptable entity type, or "Unknown" if not known.


This function returns the scriptable entity type as a string. 

**Returns:**

A string representing the scriptable entity type, or an empty string if no specific type is set. 





        

<hr>



### function IsCharacter 

_Checks whether the scriptable entity is of type "Character"._ 
```C++
inline vi rtual bo ol AGE::ScriptableEntity::IsCharacter () 
```





**Return value:**


* `-` bool 



**Author:**

De'Lano Wilcox 


This function compares the result of `GetScriptableEntityType` with the string literal "Character", and returns true if they match. Otherwise, it returns false.




**Returns:**

True if the scriptable entity type equals "Character", False otherwise.


Checks whether the scriptable entity type is a character.


This function compares the scriptable entity type to "Character". If they match, it returns true; otherwise, false.




**Returns:**

True if the scriptable entity type is "Character", false otherwise. 





        

<hr>



### function OnEvent 

```C++
inline virtual void AGE::ScriptableEntity::OnEvent (
    Event & E
) 
```




<hr>



### function OnHit 

_This function is called when an object gets hit by another object._ 
```C++
inline vi rtual vo id AGE::ScriptableEntity::OnHit () 
```





**Returns:**

None


This function is called when an object gets hit by another object.




**Returns:**

void 





        

<hr>



### function OnOverlapStart 

_This function is called when an overlap starts between two objects._ 
```C++
inline vi rtual vo id AGE::ScriptableEntity::OnOverlapStart () 
```



The exact behavior of this function depends on the specific implementation in any derived classes. It's assumed that it will be overridden by those classes to provide their own functionality.




**Returns:**

void


This function is called when an overlap starts.




**Returns:**

Unknown 





        

<hr>



### function OnOverlapStop 

_This function is called when an overlap stops._ 
```C++
inline vi rtual vo id AGE::ScriptableEntity::OnOverlapStop () 
```



Detailed explanation of what this function does goes here. It should be concise and clear, explaining the purpose and behavior of the function in a way that's understandable to someone unfamiliar with the codebase.




**Returns:**

void


This function is called when an overlap occurs between two objects. The exact behavior of this function is not known as it has not been implemented yet. 

**Returns:**

Unknown 





        

<hr>



### function SetLocation 

_Sets the location of an object._ 
```C++
inline vi rtual vo id AGE::ScriptableEntity::SetLocation (
    const AGE::Vector3 & Location
) 
```



This function sets the location of an object in a three-dimensional space. The location is represented by a [**Vector3**](struct_a_g_e_1_1_vector3.md) structure, which contains x, y and z coordinates.




**Parameters:**


* `Location` A const reference to an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) representing the new location of the object. 



**Returns:**

void


Sets the location of an object.


This function sets the location of an object in a 3D space. The location is represented by a [**Vector3**](struct_a_g_e_1_1_vector3.md) structure, which contains x, y and z coordinates.




**Parameters:**


* `Location` A const reference to an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) representing the new location of the object. 



**Returns:**

Unknown 





        

<hr>



### function criptableEntity 

_Virtual destructor for the_ [_**ScriptableEntity**_](class_a_g_e_1_1_scriptable_entity.md) _class._
```C++
inline vi rtual ~S AGE::ScriptableEntity::criptableEntity () 
```



This function is a virtual destructor that cleans up any resources used by an instance of the class when it's no longer needed. It does not take any parameters and returns nothing.


Constructor for the CriptableEntity class. 


        

<hr>
## Protected Functions Documentation




### function GetEntityHandle 

_This function returns a reference to the entity object._ 
```C++
inline vi rtual En tity & AGE::ScriptableEntity::GetEntityHandle () 
```





**Returns:**

A reference to the entity object (m\_Entity).


This function returns a reference to the entity object. 

**Returns:**

A reference to the entity object (m\_Entity). 





        

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

_Pushes this scriptable entity into the application's scriptable component stack._ 
```C++
virtual void AGE::ScriptableEntity::PushComp () 
```



This function pushes the current instance of [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) (`this`) into the stack of scriptable components in the [**App**](class_a_g_e_1_1_app.md) class. It does not return anything, so its return type is void.


Pushes this scriptable entity into the application's scriptable component stack.


This function pushes a reference to this [**ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) instance onto the stack of scriptable components in the [**App**](class_a_g_e_1_1_app.md) class. It is used when a new scriptable object needs to be added to the system. 


        

<hr>



### function Reset 

```C++
inline virtual void AGE::ScriptableEntity::Reset () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/ScriptableEntity.h`

