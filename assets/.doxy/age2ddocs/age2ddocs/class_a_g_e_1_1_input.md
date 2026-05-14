

# Class AGE::Input



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Input**](class_a_g_e_1_1_input.md)



_This class provides methods for checking the state of input devices._ [More...](#detailed-description)

* `#include <Input.h>`







































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetJoyStickLeftTrigger**](#function-getjoysticklefttrigger) (uint16\_t ID) <br> |
|  float | [**GetJoyStickLeftX**](#function-getjoystickleftx) (uint16\_t ID) <br> |
|  std::pair&lt; float, float &gt; | [**GetJoyStickLeftXY**](#function-getjoystickleftxy) (uint16\_t ID) <br> |
|  float | [**GetJoyStickLeftY**](#function-getjoysticklefty) (uint16\_t ID) <br> |
|  float | [**GetJoyStickRightTrigger**](#function-getjoystickrighttrigger) (uint16\_t ID) <br> |
|  float | [**GetJoyStickRightX**](#function-getjoystickrightx) (uint16\_t ID) <br> |
|  std::pair&lt; float, float &gt; | [**GetJoyStickRightXY**](#function-getjoystickrightxy) (uint16\_t ID) <br> |
|  float | [**GetJoyStickRightY**](#function-getjoystickrighty) (uint16\_t ID) <br> |
|  float | [**GetMouseX**](#function-getmousex) () <br> |
|  std::pair&lt; float, float &gt; | [**GetMouseXY**](#function-getmousexy) () <br> |
|  float | [**GetMouseY**](#function-getmousey) () <br> |
|  bool | [**IsGamepadButtonPressed**](#function-isgamepadbuttonpressed) (uint16\_t ID, uint8\_t Button) <br> |
|  bool | [**IsJoyStickConnected**](#function-isjoystickconnected) (uint16\_t ID) <br> |
|  bool | [**IsKeyPressed**](#function-iskeypressed) (int Keycode) <br> |
|  bool | [**IsMouseButtonPressed**](#function-ismousebuttonpressed) (int Button) <br> |


























## Detailed Description


It includes functions to check if a key, mouse button or gamepad button is pressed, as well as getting the position of the mouse and joystick.


This class provides methods for checking the state of input devices.


It includes functions to check if a key, mouse button or gamepad button is pressed, as well as getting the position of the mouse and joystick. 


    
## Public Static Functions Documentation




### function GetJoyStickLeftTrigger 

```C++
static float AGE::Input::GetJoyStickLeftTrigger (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickLeftX 

```C++
static float AGE::Input::GetJoyStickLeftX (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickLeftXY 

```C++
static std::pair< float, float > AGE::Input::GetJoyStickLeftXY (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickLeftY 

```C++
static float AGE::Input::GetJoyStickLeftY (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickRightTrigger 

```C++
static float AGE::Input::GetJoyStickRightTrigger (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickRightX 

```C++
static float AGE::Input::GetJoyStickRightX (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickRightXY 

```C++
static std::pair< float, float > AGE::Input::GetJoyStickRightXY (
    uint16_t ID
) 
```




<hr>



### function GetJoyStickRightY 

```C++
static float AGE::Input::GetJoyStickRightY (
    uint16_t ID
) 
```




<hr>



### function GetMouseX 

```C++
static float AGE::Input::GetMouseX () 
```




<hr>



### function GetMouseXY 

```C++
static std::pair< float, float > AGE::Input::GetMouseXY () 
```




<hr>



### function GetMouseY 

```C++
static float AGE::Input::GetMouseY () 
```




<hr>



### function IsGamepadButtonPressed 

```C++
static bool AGE::Input::IsGamepadButtonPressed (
    uint16_t ID,
    uint8_t Button
) 
```




<hr>



### function IsJoyStickConnected 

```C++
static bool AGE::Input::IsJoyStickConnected (
    uint16_t ID
) 
```




<hr>



### function IsKeyPressed 

```C++
static bool AGE::Input::IsKeyPressed (
    int Keycode
) 
```




<hr>



### function IsMouseButtonPressed 

```C++
static bool AGE::Input::IsMouseButtonPressed (
    int Button
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Input.h`

