

# Namespace AGE::GamePad



[**Namespace List**](namespaces.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GamePad**](namespace_a_g_e_1_1_game_pad.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum JoyStickID | [**GamePad**](#enum-gamepad)  <br> |
| enum JoyStickCode | [**Axes**](#enum-axes)  <br> |
| enum GamePadCode | [**Buttons**](#enum-buttons)  <br> |
| enum uint16\_t | [**XInputMasks**](#enum-xinputmasks)  <br> |
















































## Public Types Documentation




### enum GamePad 

```C++
enum AGE::GamePad::GamePad {
    JoyStick1 = 0,
    JoyStick2 = 1,
    JoyStick3 = 2,
    JoyStick4 = 3,
    JoyStick5 = 4,
    JoyStick6 = 5,
    JoyStick7 = 6,
    JoyStick8 = 7,
    JoyStick9 = 8,
    JoyStick10 = 9,
    JoyStick11 = 10,
    JoyStick12 = 11,
    JoyStick13 = 12,
    JoyStick14 = 13,
    JoyStick15 = 14,
    JoyStick16 = 15,
    JoyStickLast = JoyStick16
};
```




<hr>



### enum Axes 

```C++
enum AGE::GamePad::Axes {
    GamePadAxisLeftX = 0,
    GamePadAxisLeftY = 1,
    GamePadAxisRightX = 2,
    GamePadAxisRightY = 3,
    GamePadAxisLeftTrigger = 4,
    GamePadAxisRightTrigger = 5,
    GamePadAxisLast = GamePadAxisRightTrigger,
    INVALIDAXES = UINT16_MAX
};
```




<hr>



### enum Buttons 

```C++
enum AGE::GamePad::Buttons {
    GamePadButtonA =0,
    GamePadButtonB =1,
    GamePadButtonX =2,
    GamePadButtonY =3,
    GamePadButtonLB =4,
    GamePadButtonRB =5,
    GamePadButtonBack =6,
    GamePadButtonStart =7,
    GamePadButtonGUIDE =8,
    GamePadButtonLeftThumb =9,
    GamePadButtonRightThumb =10,
    GamePadButtonDpadUp =11,
    GamePadButtonDpadRight =12,
    GamePadButtonDpadDown =13,
    GamePadButtonDpadLeft =14,
    GamePadButtonLast =GamePadButtonDpadLeft,
    GamePadButtonCross =GamePadButtonA,
    GamePadButtonCircle =GamePadButtonB,
    GamePadButtonSquare =GamePadButtonX,
    GamePadButtonTriangle =GamePadButtonY,
    INVALID = UINT8_MAX
};
```




<hr>



### enum XInputMasks 

```C++
enum AGE::GamePad::XInputMasks {
    XInputDpadUp = 0x0001,
    XInputDpadDown = 0x0002,
    XInputDpadLeft = 0x0004,
    XInputDpadRight = 0x0008,
    XInputStart = 0x0010,
    XInputBack = 0x0020,
    XInputLeftThumb = 0x0040,
    XInputRightThumb = 0x0080,
    XInputLeftShoulder = 0x0100,
    XInputRightShoulder = 0x0200,
    XInputButtonA = 0x1000,
    XInputButtonB = 0x2000,
    XInputButtonX = 0x4000,
    XInputButtonY = 0x8000
};
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/GamepadCodes.h`

