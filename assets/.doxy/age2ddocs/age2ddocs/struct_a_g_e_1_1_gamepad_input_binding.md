

# Struct AGE::GamepadInputBinding



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GamepadInputBinding**](struct_a_g_e_1_1_gamepad_input_binding.md)








Inherits the following classes: [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)
















## Public Types inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
| typedef std::function&lt; void()&gt; | [**ActionCallbackFn**](struct_a_g_e_1_1_input_binding.md#typedef-actioncallbackfn)  <br> |
| typedef std::function&lt; void(float)&gt; | [**AxisCallbackFn**](struct_a_g_e_1_1_input_binding.md#typedef-axiscallbackfn)  <br> |






## Public Attributes

| Type | Name |
| ---: | :--- |
|  GamePad::Axes | [**m\_Axes**](#variable-m_axes)   = `GamePad::Axes::INVALIDAXES`<br> |
|  Binding::Type | [**m\_BindingType**](#variable-m_bindingtype)  <br> |
|  GamePad::Buttons | [**m\_Button**](#variable-m_button)   = `GamePad::Buttons::INVALID`<br> |


## Public Attributes inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_BindingName**](struct_a_g_e_1_1_input_binding.md#variable-m_bindingname)  <br> |
|  KeyState::State | [**m\_State**](struct_a_g_e_1_1_input_binding.md#variable-m_state)   = `KeyState::Pressed`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**GamepadInputBinding**](#function-gamepadinputbinding-14) (const std::string\_view & Name, Binding::Type type) <br> |
|   | [**GamepadInputBinding**](#function-gamepadinputbinding-24) (const std::string\_view & Name, GamePad::Buttons button, Binding::Type type) <br> |
|   | [**GamepadInputBinding**](#function-gamepadinputbinding-34) (const std::string\_view & Name, GamePad::Axes axes, Binding::Type type) <br> |
| virtual uint16\_t | [**GetKey**](#function-getkey) () override const<br> |
|   | [**~GamepadInputBinding**](#function-gamepadinputbinding) () override<br> |


## Public Functions inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  void | [**ActionExecute**](struct_a_g_e_1_1_input_binding.md#function-actionexecute) () <br> |
|  void | [**AxisExecute**](struct_a_g_e_1_1_input_binding.md#function-axisexecute) () <br> |
|  void | [**BindActionFunction**](struct_a_g_e_1_1_input_binding.md#function-bindactionfunction) (ActionCallbackFn Func) <br> |
|  void | [**BindAxisFunction**](struct_a_g_e_1_1_input_binding.md#function-bindaxisfunction) (AxisCallbackFn Func) <br> |
|  void | [**GenerateNewHandle**](struct_a_g_e_1_1_input_binding.md#function-generatenewhandle) () <br> |
|  float | [**GetAxisValue**](struct_a_g_e_1_1_input_binding.md#function-getaxisvalue) () const<br> |
|  int32\_t | [**GetHandle**](struct_a_g_e_1_1_input_binding.md#function-gethandle) () const<br> |
|  std::string | [**GetInputType**](struct_a_g_e_1_1_input_binding.md#function-getinputtype) () const<br> |
| virtual uint16\_t | [**GetKey**](struct_a_g_e_1_1_input_binding.md#function-getkey) () const = 0<br> |
|  std::string | [**GetName**](struct_a_g_e_1_1_input_binding.md#function-getname) () const<br> |
|  bool | [**IsPaired**](struct_a_g_e_1_1_input_binding.md#function-ispaired) () const<br> |
|  bool | [**IsValid**](struct_a_g_e_1_1_input_binding.md#function-isvalid) () <br> |
|  void | [**SetAxisValue**](struct_a_g_e_1_1_input_binding.md#function-setaxisvalue) (float value) <br> |
|  void | [**SetInputType**](struct_a_g_e_1_1_input_binding.md#function-setinputtype) (const std::string\_view & type) <br> |
|  void | [**SetPaired**](struct_a_g_e_1_1_input_binding.md#function-setpaired) (bool value) <br> |
|  bool | [**operator==**](struct_a_g_e_1_1_input_binding.md#function-operator) (const [**InputBinding**](struct_a_g_e_1_1_input_binding.md) & rhs) <br> |
| virtual  | [**~InputBinding**](struct_a_g_e_1_1_input_binding.md#function-inputbinding) () = default<br> |




## Public Static Functions inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](struct_a_g_e_1_1_input_binding.md#function-creategamepadbinding-12) (const std::string\_view & Name, GamePad::Buttons button=GamePad::Buttons::INVALID, Binding::Type bindingtype=Binding::Type::INVALID) <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](struct_a_g_e_1_1_input_binding.md#function-creategamepadbinding-22) (const std::string\_view & Name, GamePad::Axes axes=GamePad::Axes::INVALIDAXES, Binding::Type bindingtype=Binding::Type::Axis) <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateInvalid**](struct_a_g_e_1_1_input_binding.md#function-createinvalid) () <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateKBMBinding**](struct_a_g_e_1_1_input_binding.md#function-createkbmbinding) (const std::string\_view & Name, Key::Keys keycode=Key::INVALID, Binding::Type bindingtype=Binding::INVALID) <br> |












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






































## Public Attributes Documentation




### variable m\_Axes 

```C++
GamePad::Axes AGE::GamepadInputBinding::m_Axes;
```




<hr>



### variable m\_BindingType 

```C++
Binding::Type AGE::GamepadInputBinding::m_BindingType;
```




<hr>



### variable m\_Button 

```C++
GamePad::Buttons AGE::GamepadInputBinding::m_Button;
```




<hr>
## Public Functions Documentation




### function GamepadInputBinding [1/4]

```C++
inline AGE::GamepadInputBinding::GamepadInputBinding (
    const std::string_view & Name,
    Binding::Type type
) 
```




<hr>



### function GamepadInputBinding [2/4]

```C++
inline AGE::GamepadInputBinding::GamepadInputBinding (
    const std::string_view & Name,
    GamePad::Buttons button,
    Binding::Type type
) 
```




<hr>



### function GamepadInputBinding [3/4]

```C++
inline AGE::GamepadInputBinding::GamepadInputBinding (
    const std::string_view & Name,
    GamePad::Axes axes,
    Binding::Type type
) 
```




<hr>



### function GetKey 

```C++
inline virtual uint16_t AGE::GamepadInputBinding::GetKey () override const
```



Implements [*AGE::InputBinding::GetKey*](struct_a_g_e_1_1_input_binding.md#function-getkey)


<hr>



### function ~GamepadInputBinding 

```C++
AGE::GamepadInputBinding::~GamepadInputBinding () override
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/InputBinding.h`

