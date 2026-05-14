

# Struct AGE::KBMInputBinding



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**KBMInputBinding**](struct_a_g_e_1_1_k_b_m_input_binding.md)








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
|  Binding::Type | [**m\_BindingType**](#variable-m_bindingtype)  <br> |
|  Key::Keys | [**m\_Key**](#variable-m_key)   = `Key::INVALID`<br> |


## Public Attributes inherited from AGE::InputBinding

See [AGE::InputBinding](struct_a_g_e_1_1_input_binding.md)

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_BindingName**](struct_a_g_e_1_1_input_binding.md#variable-m_bindingname)  <br> |
|  KeyState::State | [**m\_State**](struct_a_g_e_1_1_input_binding.md#variable-m_state)   = `KeyState::Pressed`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint16\_t | [**GetKey**](#function-getkey) () override const<br>_This function returns a key code based on the binding type._  |
|   | [**KBMInputBinding**](#function-kbminputbinding-13) (const std::string\_view & Name, Binding::Type type) <br>_Constructs a new instance of_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _._ |
|   | [**KBMInputBinding**](#function-kbminputbinding-23) (const std::string\_view & Name, Key::Keys keycode, Binding::Type type) <br>_Constructs a new_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object._ |
|   | [**~KBMInputBinding**](#function-kbminputbinding) () override<br>_Destructor for the_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _class._ |


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






































## Public Attributes Documentation




### variable m\_BindingType 

```C++
Binding::Type AGE::KBMInputBinding::m_BindingType;
```




<hr>



### variable m\_Key 

```C++
Key::Keys AGE::KBMInputBinding::m_Key;
```




<hr>
## Public Functions Documentation




### function GetKey 

_This function returns a key code based on the binding type._ 
```C++
inline virtual uint16_t AGE::KBMInputBinding::GetKey () override const
```



The function checks the value of m\_BindingType and returns different values depending on its state. If it's an Axis, it returns UINT16\_MAX as placeholder for future implementation. If it's an Action, it returns the value stored in m\_Key. For all other cases, it again returns UINT16&lt;｜begin▁of▁sentence｜&gt;MAX.




**Returns:**

uint16\_t The key code to be returned based on the binding type. 





        
Implements [*AGE::InputBinding::GetKey*](struct_a_g_e_1_1_input_binding.md#function-getkey)


<hr>



### function KBMInputBinding [1/3]

_Constructs a new instance of_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _._
```C++
inline AGE::KBMInputBinding::KBMInputBinding (
    const std::string_view & Name,
    Binding::Type type
) 
```



This constructor initializes the binding with the given name and type, setting default values for other members.




**Parameters:**


* `Name` The name of the input binding. 
* `type` The type of the input binding (Keyboard, Mouse etc.). 




        

<hr>



### function KBMInputBinding [2/3]

_Constructs a new_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _object._
```C++
inline AGE::KBMInputBinding::KBMInputBinding (
    const std::string_view & Name,
    Key::Keys keycode,
    Binding::Type type
) 
```



This constructor initializes the binding with a given name, keycode, and type. It also sets some default values for other members of the class.




**Parameters:**


* `Name` The name of the binding. 
* `keycode` The key code associated with this binding. 
* `type` The type of the binding (e.g., KeyPress, KeyRelease). 




        

<hr>



### function ~KBMInputBinding 

_Destructor for the_ [_**KBMInputBinding**_](struct_a_g_e_1_1_k_b_m_input_binding.md) _class._
```C++
AGE::KBMInputBinding::~KBMInputBinding () override
```



This function is responsible for releasing any resources that were acquired during the lifetime of this object, such as memory or file handles. It also ensures that all subclasses have a well-defined destructor to follow the Rule of 5 (copy constructor, copy assignment operator, move constructor, move assignment operator and destructor).




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/InputBinding.h`

