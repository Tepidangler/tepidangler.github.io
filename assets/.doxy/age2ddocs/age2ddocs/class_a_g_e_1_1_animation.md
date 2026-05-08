

# Class AGE::Animation



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Animation**](class_a_g_e_1_1_animation.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Animation**](#function-animation-12) () <br> |
|   | [**Animation**](#function-animation-22) (const [**Animation**](class_a_g_e_1_1_animation.md) &) = default<br> |
|  int | [**GetCurrentFrame**](#function-getcurrentframe) () <br> |
|  Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; | [**GetCurrentTexture**](#function-getcurrenttexture) () <br> |
|  int | [**GetFrameRate**](#function-getframerate) () <br> |
|  int | [**GetMaxFrames**](#function-getmaxframes) () <br> |
|  bool | [**GetOscillate**](#function-getoscillate) () <br> |
|  void | [**LoadAnimation**](#function-loadanimation) (const [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) Anim) <br> |
|  void | [**LoadAnimations**](#function-loadanimations) (const std::vector&lt; [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) &gt; & Anims) <br> |
|  void | [**OnAnimate**](#function-onanimate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**OnDestroy**](#function-ondestroy) () <br> |
|  void | [**SetCurrentFrame**](#function-setcurrentframe) (int Frame) <br> |
|  void | [**SetCurrentTexture**](#function-setcurrenttexture) (CharMovementStatus status) <br> |
|  void | [**SetFrameRate**](#function-setframerate) (int Rate) <br> |
|  void | [**SetMaxFrames**](#function-setmaxframes) (int Frames) <br> |
|  void | [**SetOscillate**](#function-setoscillate) (bool Osc) <br> |
|   | [**~Animation**](#function-animation) () = default<br> |




























## Public Functions Documentation




### function Animation [1/2]

```C++
AGE::Animation::Animation () 
```




<hr>



### function Animation [2/2]

```C++
AGE::Animation::Animation (
    const Animation &
) = default
```




<hr>



### function GetCurrentFrame 

```C++
inline int AGE::Animation::GetCurrentFrame () 
```




<hr>



### function GetCurrentTexture 

```C++
inline Ref< SubTexture2D > AGE::Animation::GetCurrentTexture () 
```




<hr>



### function GetFrameRate 

```C++
inline int AGE::Animation::GetFrameRate () 
```




<hr>



### function GetMaxFrames 

```C++
inline int AGE::Animation::GetMaxFrames () 
```




<hr>



### function GetOscillate 

```C++
inline bool AGE::Animation::GetOscillate () 
```




<hr>



### function LoadAnimation 

```C++
void AGE::Animation::LoadAnimation (
    const AnimationSpecification Anim
) 
```




<hr>



### function LoadAnimations 

```C++
void AGE::Animation::LoadAnimations (
    const std::vector< AnimationSpecification > & Anims
) 
```




<hr>



### function OnAnimate 

```C++
void AGE::Animation::OnAnimate (
    TimeStep DeltaTime
) 
```




<hr>



### function OnDestroy 

```C++
void AGE::Animation::OnDestroy () 
```




<hr>



### function SetCurrentFrame 

```C++
void AGE::Animation::SetCurrentFrame (
    int Frame
) 
```




<hr>



### function SetCurrentTexture 

```C++
void AGE::Animation::SetCurrentTexture (
    CharMovementStatus status
) 
```




<hr>



### function SetFrameRate 

```C++
inline void AGE::Animation::SetFrameRate (
    int Rate
) 
```




<hr>



### function SetMaxFrames 

```C++
inline void AGE::Animation::SetMaxFrames (
    int Frames
) 
```




<hr>



### function SetOscillate 

```C++
inline void AGE::Animation::SetOscillate (
    bool Osc
) 
```




<hr>



### function ~Animation 

```C++
AGE::Animation::~Animation () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Animation/Public/Animation.h`

