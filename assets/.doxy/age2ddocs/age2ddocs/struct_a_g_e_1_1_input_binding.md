

# Struct AGE::InputBinding



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**InputBinding**](struct_a_g_e_1_1_input_binding.md)










Inherited by the following classes: [AGE::GamepadInputBinding](struct_a_g_e_1_1_gamepad_input_binding.md),  [AGE::InvalidInputBinding\_t](struct_a_g_e_1_1_invalid_input_binding__t.md),  [AGE::KBMInputBinding](struct_a_g_e_1_1_k_b_m_input_binding.md)












## Public Types

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; void()&gt; | [**ActionCallbackFn**](#typedef-actioncallbackfn)  <br> |
| typedef std::function&lt; void(float)&gt; | [**AxisCallbackFn**](#typedef-axiscallbackfn)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_BindingName**](#variable-m_bindingname)  <br> |
|  KeyState::State | [**m\_State**](#variable-m_state)   = `KeyState::Pressed`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**ActionExecute**](#function-actionexecute) () <br>_Executes the binded action function._  |
|  void | [**AxisExecute**](#function-axisexecute) () <br>_Executes the axis function with the stored m\_AxisValue._  |
|  void | [**BindActionFunction**](#function-bindactionfunction) (ActionCallbackFn Func) <br>_This function binds an action callback function to the class instance._  |
|  void | [**BindAxisFunction**](#function-bindaxisfunction) (AxisCallbackFn Func) <br>_This function binds an axis callback function to the game controller._  |
|  void | [**GenerateNewHandle**](#function-generatenewhandle) () <br>_This function generates a new handle for an object. The generated handle is unique and sequential, starting from 1._  |
|  float | [**GetAxisValue**](#function-getaxisvalue) () const<br>_This function returns the current value of the axis._  |
|  int32\_t | [**GetHandle**](#function-gethandle) () const<br>_This function returns the handle value of an object._  |
|  std::string | [**GetInputType**](#function-getinputtype) () const<br>_This function returns the type of input used in the system._  |
| virtual uint16\_t | [**GetKey**](#function-getkey) () const = 0<br> |
|  std::string | [**GetName**](#function-getname) () const<br>_Returns the name of the binding._  |
|  bool | [**IsPaired**](#function-ispaired) () const<br>_Checks whether the object is paired._  |
|  bool | [**IsValid**](#function-isvalid) () <br>_Checks whether the object handle is valid._  |
|  void | [**SetAxisValue**](#function-setaxisvalue) (float value) <br>_This function sets the axis value to a given float value._  |
|  void | [**SetInputType**](#function-setinputtype) (const std::string\_view & type) <br>_Sets the input type for a specific component._  |
|  void | [**SetPaired**](#function-setpaired) (bool value) <br>_Sets the paired status of an object._  |
|  bool | [**operator==**](#function-operator) (const [**InputBinding**](struct_a_g_e_1_1_input_binding.md) & rhs) <br>_Compares two_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _objects for equality based on their validity and handle values._ |
| virtual  | [**~InputBinding**](#function-inputbinding) () = default<br>_Virtual destructor for the_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](#function-creategamepadbinding-12) (const std::string\_view & Name, GamePad::Buttons button=GamePad::Buttons::INVALID, Binding::Type bindingtype=Binding::Type::INVALID) <br>_Creates a gamepad input binding._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](#function-creategamepadbinding-22) (const std::string\_view & Name, GamePad::Axes axes=GamePad::Axes::INVALIDAXES, Binding::Type bindingtype=Binding::Type::Axis) <br>_Creates a gamepad input binding._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateInvalid**](#function-createinvalid) () <br>_Creates an invalid input binding instance._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateKBMBinding**](#function-createkbmbinding) (const std::string\_view & Name, Key::Keys keycode=Key::INVALID, Binding::Type bindingtype=Binding::INVALID) <br>_Creates an input binding object. The function checks if the provided key code is valid and creates a corresponding_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object accordingly. If the keycode is invalid, it still creates a_[_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object with only the name and type parameters._ |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  ActionCallbackFn | [**BindedActionFunction**](#variable-bindedactionfunction)  <br> |
|  AxisCallbackFn | [**BindedAxisFunction**](#variable-bindedaxisfunction)  <br> |
|  uint8\_t | [**bConsumeInput**](#variable-bconsumeinput)   = `1`<br> |
|  uint8\_t | [**bExecuteWhenPaused**](#variable-bexecutewhenpaused)   = `0`<br> |
|  uint8\_t | [**bPaired**](#variable-bpaired)   = `1`<br> |
|  float | [**m\_AxisValue**](#variable-m_axisvalue)   = `0.f`<br> |
|  int | [**m\_Handle**](#variable-m_handle)  <br> |
|  std::string | [**m\_InputType**](#variable-m_inputtype)  <br> |




















## Public Types Documentation




### typedef ActionCallbackFn 

```C++
using AGE::InputBinding::ActionCallbackFn =  std::function<void()>;
```




<hr>



### typedef AxisCallbackFn 

```C++
using AGE::InputBinding::AxisCallbackFn =  std::function<void(float)>;
```




<hr>
## Public Attributes Documentation




### variable m\_BindingName 

```C++
std::string AGE::InputBinding::m_BindingName;
```




<hr>



### variable m\_State 

```C++
KeyState::State AGE::InputBinding::m_State;
```




<hr>
## Public Functions Documentation




### function ActionExecute 

_Executes the binded action function._ 
```C++
inline void AGE::InputBinding::ActionExecute () 
```



This function calls the BindedActionFunction, which is presumably a method that performs some action when called. The exact behavior of this function depends on its implementation and cannot be accurately described here.




**Returns:**

void 





        

<hr>



### function AxisExecute 

_Executes the axis function with the stored m\_AxisValue._ 
```C++
inline void AGE::InputBinding::AxisExecute () 
```



This function calls the BindedAxisFunction member function of the class, passing in the value of m\_AxisValue as an argument. It is assumed that this member function handles the actual execution of the axis function.




**Returns:**

void 





        

<hr>



### function BindActionFunction 

_This function binds an action callback function to the class instance._ 
```C++
inline void AGE::InputBinding::BindActionFunction (
    ActionCallbackFn Func
) 
```





**Parameters:**


* `Func` The ActionCallbackFn type function that will be bound as the new action callback function. 



**Returns:**

None 





        

<hr>



### function BindAxisFunction 

_This function binds an axis callback function to the game controller._ 
```C++
inline void AGE::InputBinding::BindAxisFunction (
    AxisCallbackFn Func
) 
```





**Parameters:**


* `Func` The function that will be called when a specific event on an axis occurs. 




        

<hr>



### function GenerateNewHandle 

_This function generates a new handle for an object. The generated handle is unique and sequential, starting from 1._ 
```C++
inline void AGE::InputBinding::GenerateNewHandle () 
```





**Returns:**

void 





        

<hr>



### function GetAxisValue 

_This function returns the current value of the axis._ 
```C++
inline float AGE::InputBinding::GetAxisValue () const
```





**Returns:**

A float representing the current value of the axis. 





        

<hr>



### function GetHandle 

_This function returns the handle value of an object._ 
```C++
inline int32_t AGE::InputBinding::GetHandle () const
```





**Returns:**

The integer representation of the handle. 





        

<hr>



### function GetInputType 

_This function returns the type of input used in the system._ 
```C++
inline std::string AGE::InputBinding::GetInputType () const
```





**Returns:**

A string representing the type of input, which can be "Unknown" if it is not known or has not been set yet. 





        

<hr>



### function GetKey 

```C++
virtual uint16_t AGE::InputBinding::GetKey () const = 0
```




<hr>



### function GetName 

_Returns the name of the binding._ 
```C++
inline std::string AGE::InputBinding::GetName () const
```





**Returns:**

A string containing the name of the binding. If no name is set, returns an empty string. 





        

<hr>



### function IsPaired 

_Checks whether the object is paired._ 
```C++
inline bool AGE::InputBinding::IsPaired () const
```



This function returns a boolean value indicating whether the object is currently paired or not.




**Returns:**

True if the object is paired, false otherwise. 





        

<hr>



### function IsValid 

_Checks whether the object handle is valid._ 
```C++
inline bool AGE::InputBinding::IsValid () 
```



This function checks if the object's handle is not equal to -1, indicating that it is a valid handle.




**Returns:**

True if the handle is valid (not equal to -1), false otherwise. 





        

<hr>



### function SetAxisValue 

_This function sets the axis value to a given float value._ 
```C++
inline void AGE::InputBinding::SetAxisValue (
    float value
) 
```





**Parameters:**


* `value` The new value for the axis. 



**Returns:**

void 





        

<hr>



### function SetInputType 

_Sets the input type for a specific component._ 
```C++
inline void AGE::InputBinding::SetInputType (
    const std::string_view & type
) 
```





**Parameters:**


* `type` A string view representing the new input type. 



**Returns:**

void 





        

<hr>



### function SetPaired 

_Sets the paired status of an object._ 
```C++
inline void AGE::InputBinding::SetPaired (
    bool value
) 
```



This function sets the 'bPaired' member variable to a specified boolean value, indicating whether or not the object is in a pairing state.




**Parameters:**


* `value` A boolean value representing the new paired status of the object. 




        

<hr>



### function operator== 

_Compares two_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _objects for equality based on their validity and handle values._
```C++
inline bool AGE::InputBinding::operator== (
    const InputBinding & rhs
) 
```





**Parameters:**


* `rhs` The right-hand side of the comparison. 



**Returns:**

True if both objects are valid and have the same handle value, false otherwise. 





        

<hr>



### function ~InputBinding 

_Virtual destructor for the_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _class._
```C++
virtual AGE::InputBinding::~InputBinding () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function CreateGamepadBinding [1/2]

_Creates a gamepad input binding._ 
```C++
static Ref< InputBinding > AGE::InputBinding::CreateGamepadBinding (
    const std::string_view & Name,
    GamePad::Buttons button=GamePad::Buttons::INVALID,
    Binding::Type bindingtype=Binding::Type::INVALID
) 
```



This function creates an instance of [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) based on the provided parameters. If the button parameter is not INVALID, it returns a reference to a new [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) object with the specified Name, button and binding type. Otherwise, it returns a reference to a new [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) object with only the Name and binding type.




**Parameters:**


* `Name` The name of the input binding. 
* `button` The gamepad button that triggers this binding. If INVALID, no specific button is associated with this binding. 
* `bindingtype` The type of the input binding (e.&lt;｜begin▁of▁sentence｜&gt;g., keyboard, mouse).



**Returns:**

A reference to a new [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) object. 





        

<hr>



### function CreateGamepadBinding [2/2]

_Creates a gamepad input binding._ 
```C++
static Ref< InputBinding > AGE::InputBinding::CreateGamepadBinding (
    const std::string_view & Name,
    GamePad::Axes axes=GamePad::Axes::INVALIDAXES,
    Binding::Type bindingtype=Binding::Type::Axis
) 
```



This function creates an instance of [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) based on the provided parameters. If axes are specified, it will create a [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) with both name and axes. Otherwise, it will only use the name. The type of binding is also passed in as a parameter.




**Parameters:**


* `Name` The name of the gamepad input. 
* `axes` The axes to be used for the gamepad input (optional). 
* `bindingtype` The type of the binding, such as keyboard or mouse.



**Returns:**

A reference to a [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md) object. 





        

<hr>



### function CreateInvalid 

_Creates an invalid input binding instance._ 
```C++
static Ref< InputBinding > AGE::InputBinding::CreateInvalid () 
```



This function creates and returns a reference to an InvalidInputBinding object, which is a subclass of [**InputBinding**](struct_a_g_e_1_1_input_binding.md). It represents an invalid or undefined input binding.




**Returns:**

A Ref&lt;InvalidInputBinding\_t&gt; representing the created invalid input binding. 





        

<hr>



### function CreateKBMBinding 

_Creates an input binding object. The function checks if the provided key code is valid and creates a corresponding_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object accordingly. If the keycode is invalid, it still creates a_[_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object with only the name and type parameters._
```C++
static Ref< InputBinding > AGE::InputBinding::CreateKBMBinding (
    const std::string_view & Name,
    Key::Keys keycode=Key::INVALID,
    Binding::Type bindingtype=Binding::INVALID
) 
```





**Parameters:**


* `Name` The name of the input binding. 
* `keycode` The key code associated with the input binding. 
* `bindingtype` The type of the input binding (e.g., keyboard, mouse).



**Returns:**

A reference to an [**InputBinding**](struct_a_g_e_1_1_input_binding.md) object. If the provided key code is valid, this will be a [**KBMInputBinding**](struct_a_g_e_1_1_k_b_m_input_binding.md) object; otherwise, it will still be a [**KBMInputBinding**](struct_a_g_e_1_1_k_b_m_input_binding.md) object with only the name and type parameters. 





        

<hr>
## Protected Attributes Documentation




### variable BindedActionFunction 

```C++
ActionCallbackFn AGE::InputBinding::BindedActionFunction;
```




<hr>



### variable BindedAxisFunction 

```C++
AxisCallbackFn AGE::InputBinding::BindedAxisFunction;
```




<hr>



### variable bConsumeInput 

```C++
uint8_t AGE::InputBinding::bConsumeInput;
```




<hr>



### variable bExecuteWhenPaused 

```C++
uint8_t AGE::InputBinding::bExecuteWhenPaused;
```




<hr>



### variable bPaired 

```C++
uint8_t AGE::InputBinding::bPaired;
```




<hr>



### variable m\_AxisValue 

```C++
float AGE::InputBinding::m_AxisValue;
```




<hr>



### variable m\_Handle 

```C++
int AGE::InputBinding::m_Handle;
```




<hr>



### variable m\_InputType 

```C++
std::string AGE::InputBinding::m_InputType;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/InputBinding.h`

