

# Struct AGE::InvalidInputBinding\_t



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**InvalidInputBinding\_t**](struct_a_g_e_1_1_invalid_input_binding__t.md)








Inherits the following classes: [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)
















## Public Types inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; void()&gt; | [**ActionCallbackFn**](struct_a_g_e_1_1_input_binding.md#typedef-actioncallbackfn)  <br> |
| typedef std::function&lt; void(float)&gt; | [**AxisCallbackFn**](struct_a_g_e_1_1_input_binding.md#typedef-axiscallbackfn)  <br> |








## Public Attributes inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_BindingName**](struct_a_g_e_1_1_input_binding.md#variable-m_bindingname)  <br> |
|  KeyState::State | [**m\_State**](struct_a_g_e_1_1_input_binding.md#variable-m_state)   = `KeyState::Pressed`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint16\_t | [**GetKey**](#function-getkey) () override const<br>_This function returns a constant 16-bit unsigned integer with the maximum value._  |
|   | [**InvalidInputBinding\_t**](#function-invalidinputbinding_t) () <br>_Default constructor for_ [_**InvalidInputBinding\_t**_](struct_a_g_e_1_1_invalid_input_binding__t.md) _class. Initializes the binding name to "INVALID"._ |
|   | [**~InvalidInputBinding\_t**](#function-invalidinputbinding_t) () = default<br>_Default destructor for the_ [_**InvalidInputBinding\_t**_](struct_a_g_e_1_1_invalid_input_binding__t.md) _class. This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return a value and has no parameters._ |


## Public Functions inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  void | [**ActionExecute**](struct_a_g_e_1_1_input_binding.md#function-actionexecute) () <br>_Executes the binded action function._  |
|  void | [**AxisExecute**](struct_a_g_e_1_1_input_binding.md#function-axisexecute) () <br>_Executes the axis function with the stored m\_AxisValue._  |
|  void | [**BindActionFunction**](struct_a_g_e_1_1_input_binding.md#function-bindactionfunction) (ActionCallbackFn Func) <br>_This function binds an action callback function to the class instance._  |
|  void | [**BindAxisFunction**](struct_a_g_e_1_1_input_binding.md#function-bindaxisfunction) (AxisCallbackFn Func) <br>_This function binds an axis callback function to the game controller._  |
|  void | [**GenerateNewHandle**](struct_a_g_e_1_1_input_binding.md#function-generatenewhandle) () <br>_This function generates a new handle for an object. The generated handle is unique and sequential, starting from 1._  |
|  float | [**GetAxisValue**](struct_a_g_e_1_1_input_binding.md#function-getaxisvalue) () const<br>_This function returns the current value of the axis._  |
|  int32\_t | [**GetHandle**](struct_a_g_e_1_1_input_binding.md#function-gethandle) () const<br>_This function returns the handle value of an object._  |
|  std::string | [**GetInputType**](struct_a_g_e_1_1_input_binding.md#function-getinputtype) () const<br>_This function returns the type of input used in the system._  |
| virtual uint16\_t | [**GetKey**](struct_a_g_e_1_1_input_binding.md#function-getkey) () const = 0<br> |
|  std::string | [**GetName**](struct_a_g_e_1_1_input_binding.md#function-getname) () const<br>_Returns the name of the binding._  |
|  bool | [**IsPaired**](struct_a_g_e_1_1_input_binding.md#function-ispaired) () const<br>_Checks whether the object is paired._  |
|  bool | [**IsValid**](struct_a_g_e_1_1_input_binding.md#function-isvalid) () <br>_Checks whether the object handle is valid._  |
|  void | [**SetAxisValue**](struct_a_g_e_1_1_input_binding.md#function-setaxisvalue) (float value) <br>_This function sets the axis value to a given float value._  |
|  void | [**SetInputType**](struct_a_g_e_1_1_input_binding.md#function-setinputtype) (const std::string\_view & type) <br>_Sets the input type for a specific component._  |
|  void | [**SetPaired**](struct_a_g_e_1_1_input_binding.md#function-setpaired) (bool value) <br>_Sets the paired status of an object._  |
|  bool | [**operator==**](struct_a_g_e_1_1_input_binding.md#function-operator) (const [**InputBinding**](struct_a_g_e_1_1_input_binding.md) & rhs) <br>_Compares two_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _objects for equality based on their validity and handle values._ |
| virtual  | [**~InputBinding**](struct_a_g_e_1_1_input_binding.md#function-inputbinding) () = default<br>_Virtual destructor for the_ [_**InputBinding**_](struct_a_g_e_1_1_input_binding.md) _class._ |




## Public Static Functions inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](struct_a_g_e_1_1_input_binding.md#function-creategamepadbinding-12) (const std::string\_view & Name, GamePad::Buttons button=GamePad::Buttons::INVALID, Binding::Type bindingtype=Binding::Type::INVALID) <br>_Creates a gamepad input binding._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](struct_a_g_e_1_1_input_binding.md#function-creategamepadbinding-22) (const std::string\_view & Name, GamePad::Axes axes=GamePad::Axes::INVALIDAXES, Binding::Type bindingtype=Binding::Type::Axis) <br>_Creates a gamepad input binding._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateInvalid**](struct_a_g_e_1_1_input_binding.md#function-createinvalid) () <br>_Creates an invalid input binding instance._  |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateKBMBinding**](struct_a_g_e_1_1_input_binding.md#function-createkbmbinding) (const std::string\_view & Name, Key::Keys keycode=Key::INVALID, Binding::Type bindingtype=Binding::INVALID) <br>_Creates an input binding object. The function checks if the provided key code is valid and creates a corresponding_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object accordingly. If the keycode is invalid, it still creates a_[_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object with only the name and type parameters._ |












## Protected Attributes inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  ActionCallbackFn | [**BindedActionFunction**](struct_a_g_e_1_1_input_binding.md#variable-bindedactionfunction)  <br> |
|  AxisCallbackFn | [**BindedAxisFunction**](struct_a_g_e_1_1_input_binding.md#variable-bindedaxisfunction)  <br> |
|  uint8\_t | [**bConsumeInput**](struct_a_g_e_1_1_input_binding.md#variable-bconsumeinput)   = `1`<br> |
|  uint8\_t | [**bExecuteWhenPaused**](struct_a_g_e_1_1_input_binding.md#variable-bexecutewhenpaused)   = `0`<br> |
|  uint8\_t | [**bPaired**](struct_a_g_e_1_1_input_binding.md#variable-bpaired)   = `1`<br> |
|  float | [**m\_AxisValue**](struct_a_g_e_1_1_input_binding.md#variable-m_axisvalue)   = `0.f`<br> |
|  int | [**m\_Handle**](struct_a_g_e_1_1_input_binding.md#variable-m_handle)  <br> |
|  std::string | [**m\_InputType**](struct_a_g_e_1_1_input_binding.md#variable-m_inputtype)  <br> |






































## Public Functions Documentation




### function GetKey 

_This function returns a constant 16-bit unsigned integer with the maximum value._ 
```C++
inline virtual uint16_t AGE::InvalidInputBinding_t::GetKey () override const
```





**Returns:**

A constant 16-bit unsigned integer with the maximum value (UINT16\_MAX). 





        
Implements [*AGE::InputBinding::GetKey*](struct_a_g_e_1_1_input_binding.md#function-getkey)


<hr>



### function InvalidInputBinding\_t 

_Default constructor for_ [_**InvalidInputBinding\_t**_](struct_a_g_e_1_1_invalid_input_binding__t.md) _class. Initializes the binding name to "INVALID"._
```C++
inline AGE::InvalidInputBinding_t::InvalidInputBinding_t () 
```




<hr>



### function ~InvalidInputBinding\_t 

_Default destructor for the_ [_**InvalidInputBinding\_t**_](struct_a_g_e_1_1_invalid_input_binding__t.md) _class. This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return a value and has no parameters._
```C++
AGE::InvalidInputBinding_t::~InvalidInputBinding_t () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/InputBinding.h`

