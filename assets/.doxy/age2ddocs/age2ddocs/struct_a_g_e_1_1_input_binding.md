

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
|  void | [**ActionExecute**](#function-actionexecute) () <br> |
|  void | [**AxisExecute**](#function-axisexecute) () <br> |
|  void | [**BindActionFunction**](#function-bindactionfunction) (ActionCallbackFn Func) <br> |
|  void | [**BindAxisFunction**](#function-bindaxisfunction) (AxisCallbackFn Func) <br> |
|  void | [**GenerateNewHandle**](#function-generatenewhandle) () <br> |
|  float | [**GetAxisValue**](#function-getaxisvalue) () const<br> |
|  int32\_t | [**GetHandle**](#function-gethandle) () const<br> |
|  std::string | [**GetInputType**](#function-getinputtype) () const<br> |
| virtual uint16\_t | [**GetKey**](#function-getkey) () const = 0<br> |
|  std::string | [**GetName**](#function-getname) () const<br> |
|  bool | [**IsPaired**](#function-ispaired) () const<br> |
|  bool | [**IsValid**](#function-isvalid) () <br> |
|  void | [**SetAxisValue**](#function-setaxisvalue) (float value) <br> |
|  void | [**SetInputType**](#function-setinputtype) (const std::string\_view & type) <br> |
|  void | [**SetPaired**](#function-setpaired) (bool value) <br> |
|  bool | [**operator==**](#function-operator) (const [**InputBinding**](struct_a_g_e_1_1_input_binding.md) & rhs) <br> |
| virtual  | [**~InputBinding**](#function-inputbinding) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](#function-creategamepadbinding-12) (const std::string\_view & Name, GamePad::Buttons button=GamePad::Buttons::INVALID, Binding::Type bindingtype=Binding::Type::INVALID) <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateGamepadBinding**](#function-creategamepadbinding-22) (const std::string\_view & Name, GamePad::Axes axes=GamePad::Axes::INVALIDAXES, Binding::Type bindingtype=Binding::Type::Axis) <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateInvalid**](#function-createinvalid) () <br> |
|  Ref&lt; [**InputBinding**](struct_a_g_e_1_1_input_binding.md) &gt; | [**CreateKBMBinding**](#function-createkbmbinding) (const std::string\_view & Name, Key::Keys keycode=Key::INVALID, Binding::Type bindingtype=Binding::INVALID) <br> |






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

```C++
inline void AGE::InputBinding::ActionExecute () 
```




<hr>



### function AxisExecute 

```C++
inline void AGE::InputBinding::AxisExecute () 
```




<hr>



### function BindActionFunction 

```C++
inline void AGE::InputBinding::BindActionFunction (
    ActionCallbackFn Func
) 
```




<hr>



### function BindAxisFunction 

```C++
inline void AGE::InputBinding::BindAxisFunction (
    AxisCallbackFn Func
) 
```




<hr>



### function GenerateNewHandle 

```C++
inline void AGE::InputBinding::GenerateNewHandle () 
```




<hr>



### function GetAxisValue 

```C++
inline float AGE::InputBinding::GetAxisValue () const
```




<hr>



### function GetHandle 

```C++
inline int32_t AGE::InputBinding::GetHandle () const
```




<hr>



### function GetInputType 

```C++
inline std::string AGE::InputBinding::GetInputType () const
```




<hr>



### function GetKey 

```C++
virtual uint16_t AGE::InputBinding::GetKey () const = 0
```




<hr>



### function GetName 

```C++
inline std::string AGE::InputBinding::GetName () const
```




<hr>



### function IsPaired 

```C++
inline bool AGE::InputBinding::IsPaired () const
```




<hr>



### function IsValid 

```C++
inline bool AGE::InputBinding::IsValid () 
```




<hr>



### function SetAxisValue 

```C++
inline void AGE::InputBinding::SetAxisValue (
    float value
) 
```




<hr>



### function SetInputType 

```C++
inline void AGE::InputBinding::SetInputType (
    const std::string_view & type
) 
```




<hr>



### function SetPaired 

```C++
inline void AGE::InputBinding::SetPaired (
    bool value
) 
```




<hr>



### function operator== 

```C++
inline bool AGE::InputBinding::operator== (
    const InputBinding & rhs
) 
```




<hr>



### function ~InputBinding 

```C++
virtual AGE::InputBinding::~InputBinding () = default
```




<hr>
## Public Static Functions Documentation




### function CreateGamepadBinding [1/2]

```C++
static Ref< InputBinding > AGE::InputBinding::CreateGamepadBinding (
    const std::string_view & Name,
    GamePad::Buttons button=GamePad::Buttons::INVALID,
    Binding::Type bindingtype=Binding::Type::INVALID
) 
```




<hr>



### function CreateGamepadBinding [2/2]

```C++
static Ref< InputBinding > AGE::InputBinding::CreateGamepadBinding (
    const std::string_view & Name,
    GamePad::Axes axes=GamePad::Axes::INVALIDAXES,
    Binding::Type bindingtype=Binding::Type::Axis
) 
```




<hr>



### function CreateInvalid 

```C++
static Ref< InputBinding > AGE::InputBinding::CreateInvalid () 
```




<hr>



### function CreateKBMBinding 

```C++
static Ref< InputBinding > AGE::InputBinding::CreateKBMBinding (
    const std::string_view & Name,
    Key::Keys keycode=Key::INVALID,
    Binding::Type bindingtype=Binding::INVALID
) 
```




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

