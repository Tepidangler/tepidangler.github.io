

# Class AGE::ScriptableWidget



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md)








Inherits the following classes: std::enable_shared_from_this< ScriptableWidget >


































## Public Functions

| Type | Name |
| ---: | :--- |
|  T & | [**AddComponent**](#function-addcomponent) (Args &&... args) <br>_This function adds a component of type T to the entity._  |
|  T & | [**GetComponent**](#function-getcomponent) () <br>_This function returns a reference to the component of type T associated with the entity._  |
| virtual [**UUID**](class_a_g_e_1_1_u_u_i_d.md) | [**GetID**](#function-getid) () <br>_This function returns the unique identifier (_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _) of an entity._ |
| virtual std::string | [**GetName**](#function-getname) () <br>_Returns the name of this object._  |
| virtual bool | [**IsVisible**](#function-isvisible) () <br>_This function checks whether the object is visible or not._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
| virtual void | [**SetVisibility**](#function-setvisibility) (bool Visibility) <br>_Sets the visibility of an object._  |
| virtual  | [**~ScriptableWidget**](#function-scriptablewidget) () <br>_Virtual destructor for the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _class._ |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**bIsVisible**](#variable-bisvisible)   = `true`<br> |
|  std::string | [**m\_Name**](#variable-m_name)   = `""`<br> |
|  [**ScreenResolution**](struct_a_g_e_1_1_screen_resolution.md) | [**m\_Resolution**](#variable-m_resolution)  <br> |
|  EWidgetStack | [**m\_Stack**](#variable-m_stack)   = `EWidgetStack::INVALID`<br> |
|  std::vector&lt; Ref&lt; [**UIComponent**](class_a_g_e_1_1_u_i_component.md) &gt; &gt; | [**m\_UIComponents**](#variable-m_uicomponents)  <br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
| virtual [**Entity**](class_a_g_e_1_1_entity.md) & | [**GetEntityHandle**](#function-getentityhandle) () <br>_Returns a reference to the entity object._  |
| virtual void | [**OnConstruct**](#function-onconstruct) () <br>_This function is called when the object is being constructed._  |
| virtual void | [**OnDestroy**](#function-ondestroy) () <br>_This function is called when the object is being destroyed._  |
| virtual void | [**OnInit**](#function-oninit) () <br>_Initializes the object._  |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function is called every frame to update the game state based on the time elapsed since the last call._  |
| virtual void | [**Reset**](#function-reset) () <br>_This function is used to reset the state of an object or a system. It does not take any parameters and returns nothing. The exact effect depends on the specific implementation of the class that uses this method._  |




## Public Functions Documentation




### function AddComponent 

_This function adds a component of type T to the entity._ 
```C++
template<typename T, typename ... Args>
inline T & AGE::ScriptableWidget::AddComponent (
    Args &&... args
) 
```





**Template parameters:**


* `T` The type of the component that is being added. 
* `Args` The types of any additional arguments required for the component's construction. 



**Parameters:**


* `args` The arguments necessary for constructing the new component. 



**Returns:**

A reference to the newly created component.


Adds a component of type T to the entity. 

**Template parameters:**


* `T` The type of the component to be added. 
* `Args` The types of any additional arguments required by the component's constructor. 



**Parameters:**


* `args` Any additional arguments required by the component's constructor. 



**Returns:**

A reference to the newly created component. 





        

<hr>



### function GetComponent 

_This function returns a reference to the component of type T associated with the entity._ 
```C++
template<typename T>
inline T & AGE::ScriptableWidget::GetComponent () 
```





**Parameters:**


* `None` 



**Returns:**

A reference to the component of type T.


This function returns a reference to the component of type T associated with an entity.




**Parameters:**


* `None` 



**Returns:**

A reference to the component of type T. 





        

<hr>



### function GetID 

_This function returns the unique identifier (_ [_**UUID**_](class_a_g_e_1_1_u_u_i_d.md) _) of an entity._
```C++
inline virtual UUID AGE::ScriptableWidget::GetID () 
```





**Returns:**

The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the entity as a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object.


This function returns the unique identifier ([**UUID**](class_a_g_e_1_1_u_u_i_d.md)) of an entity. 

**Returns:**

The [**UUID**](class_a_g_e_1_1_u_u_i_d.md) of the entity as a [**UUID**](class_a_g_e_1_1_u_u_i_d.md) object. 





        

<hr>



### function GetName 

_Returns the name of this object._ 
```C++
inline virtual std::string AGE::ScriptableWidget::GetName () 
```



This function returns the name of the object as a string. It is used to identify the object in various contexts.




**Returns:**

std::string - The name of the object.


Returns the name of this object.




**Returns:**

The name as a string. 





        

<hr>



### function IsVisible 

_This function checks whether the object is visible or not._ 
```C++
inline virtual bool AGE::ScriptableWidget::IsVisible () 
```





**Returns:**

Returns true if the object is visible, false otherwise.


This function checks whether the object is visible. 

**Returns:**

Returns true if the object is visible, false otherwise. 





        

<hr>



### function OnEvent 

```C++
inline virtual void AGE::ScriptableWidget::OnEvent (
    Event & E
) 
```




<hr>



### function SetVisibility 

_Sets the visibility of an object._ 
```C++
inline virtual void AGE::ScriptableWidget::SetVisibility (
    bool Visibility
) 
```



This function sets the visibility state of an object to either visible or not visible (hidden). The new visibility state is stored in the member variable 'bIsVisible'.




**Parameters:**


* `Visibility` A boolean value indicating whether the object should be visible (true) or hidden (false).



**Returns:**

void


Sets the visibility of an object.


This function sets the visibility state of an object to either visible or not visible (hidden). The new visibility state is stored in the member variable 'bIsVisible'.




**Parameters:**


* `Visibility` A boolean value indicating whether the object should be visible (true) or hidden (false). 




        

<hr>



### function ~ScriptableWidget 

_Virtual destructor for the_ [_**ScriptableWidget**_](class_a_g_e_1_1_scriptable_widget.md) _class._
```C++
inline virtual AGE::ScriptableWidget::~ScriptableWidget () 
```



This function is responsible for freeing any resources that were allocated by the widget, such as memory or file handles. It's a virtual function to allow subclasses of [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) to override this behavior if necessary.




**Returns:**

void


Virtual destructor for the [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) class.


This function is responsible for freeing any resources that were allocated by the widget, such as memory or file handles. It's a virtual function to allow subclasses of [**ScriptableWidget**](class_a_g_e_1_1_scriptable_widget.md) to override this behavior if necessary. 


        

<hr>
## Protected Attributes Documentation




### variable bIsVisible 

```C++
bool AGE::ScriptableWidget::bIsVisible;
```




<hr>



### variable m\_Name 

```C++
std::string AGE::ScriptableWidget::m_Name;
```




<hr>



### variable m\_Resolution 

```C++
ScreenResolution AGE::ScriptableWidget::m_Resolution;
```




<hr>



### variable m\_Stack 

```C++
EWidgetStack AGE::ScriptableWidget::m_Stack;
```




<hr>



### variable m\_UIComponents 

```C++
std::vector<Ref<UIComponent> > AGE::ScriptableWidget::m_UIComponents;
```




<hr>
## Protected Functions Documentation




### function GetEntityHandle 

_Returns a reference to the entity object._ 
```C++
inline virtual Entity & AGE::ScriptableWidget::GetEntityHandle () 
```



This function returns a reference to the internal entity object, which can be used for further operations on it.




**Returns:**

A reference to the entity object ([**Entity**](class_a_g_e_1_1_entity.md)&).


This function returns a reference to the entity object. 

**Returns:**

A reference to the entity object (m\_Entity). 





        

<hr>



### function OnConstruct 

_This function is called when the object is being constructed._ 
```C++
inline virtual void AGE::ScriptableWidget::OnConstruct () 
```





**Returns:**

None


This function is called when the object is being constructed.


It does not take any parameters and does not return anything. The exact behavior of this function depends on its implementation in derived classes. 


        

<hr>



### function OnDestroy 

_This function is called when the object is being destroyed._ 
```C++
inline virtual void AGE::ScriptableWidget::OnDestroy () 
```





**Returns:**

None


This function is called when the object is being destroyed.




**Returns:**

None 





        

<hr>



### function OnInit 

_Initializes the object._ 
```C++
inline virtual void AGE::ScriptableWidget::OnInit () 
```



This function is responsible for initializing the object and its internal state. It does not take any parameters and does not return anything.


Initializes the object.


This function is responsible for initializing the object and its internal state. It does not take any parameters and does not return anything. 


        

<hr>



### function OnUpdate 

_This function is called every frame to update the game state based on the time elapsed since the last call._ 
```C++
inline virtual void AGE::ScriptableWidget::OnUpdate (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The time step representing the amount of time that has passed since the previous frame. 



**Returns:**

void No return value expected as this function does not provide any meaningful result.


This function is called every frame to update the game state.




**Parameters:**


* `DeltaTime` The time elapsed since the last frame, used for smooth movement and animation. 




        

<hr>



### function Reset 

_This function is used to reset the state of an object or a system. It does not take any parameters and returns nothing. The exact effect depends on the specific implementation of the class that uses this method._ 
```C++
inline virtual void AGE::ScriptableWidget::Reset () 
```





**Returns:**

void


This function resets the state of an object to its initial state.


The exact behavior of this function depends on the specific implementation of the class that contains it. It may reset all internal data, set default values, or perform other actions as specified by the class's design.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/ScriptableWidget.h`

