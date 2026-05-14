

# Class AGE::Animation



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Animation**](class_a_g_e_1_1_animation.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Animation**](#function-animation-12) () <br>_Default constructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class. Initializes all member variables to default values._ |
|   | [**Animation**](#function-animation-22) (const [**Animation**](class_a_g_e_1_1_animation.md) &) = default<br>_Copy constructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class._ |
|  int | [**GetCurrentFrame**](#function-getcurrentframe) () <br>_Returns the current frame number._  |
|  Ref&lt; [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) &gt; | [**GetCurrentTexture**](#function-getcurrenttexture) () <br>_Gets the current texture._  |
|  int | [**GetFrameRate**](#function-getframerate) () <br>_Returns the current frame rate._  |
|  int | [**GetMaxFrames**](#function-getmaxframes) () <br>_This function returns the maximum number of frames that can be processed by the system._  |
|  bool | [**GetOscillate**](#function-getoscillate) () <br>_Returns the oscillation state of the system._  |
|  void | [**LoadAnimation**](#function-loadanimation) (const [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) Anim) <br>_Loads an animation into the system based on the provided specification._  |
|  void | [**LoadAnimations**](#function-loadanimations) (const std::vector&lt; [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) &gt; & Anims) <br>_Loads a set of animations into the animation system._  |
|  void | [**OnAnimate**](#function-onanimate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_Updates the object's animation based on elapsed time._  |
|  void | [**OnDestroy**](#function-ondestroy) () <br>_This function is called when the object is being destroyed._  |
|  void | [**SetCurrentFrame**](#function-setcurrentframe) (int Frame) <br>_Set the Current_ [_**Animation**_](class_a_g_e_1_1_animation.md) _Frame._ |
|  void | [**SetCurrentTexture**](#function-setcurrenttexture) (CharMovementStatus status) <br>_Sets the current texture based on the character movement status._  |
|  void | [**SetFrameRate**](#function-setframerate) (int Rate) <br>_Sets the frame rate for a video processing system._  |
|  void | [**SetMaxFrames**](#function-setmaxframes) (int Frames) <br>_Sets the maximum number of frames allowed in a video sequence._  |
|  void | [**SetOscillate**](#function-setoscillate) (bool Osc) <br>_Sets the oscillation state of an object._  |
|   | [**~Animation**](#function-animation) () = default<br>_Destructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class._ |




























## Public Functions Documentation




### function Animation [1/2]

_Default constructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class. Initializes all member variables to default values._
```C++
AGE::Animation::Animation () 
```





**Parameters:**


* `None` 



**Returns:**

None


Constructor for the [**Animation**](class_a_g_e_1_1_animation.md) class. Initializes all member variables to default values.


This constructor initializes m\_CurrentFrame, m\_MaxFrames, and m\_FrameInc to 0 and 1 respectively. It also sets m\_FrameRate to 100 and m\_OldTime to 0. The boolean variable bOscillate is set to false. A [**Timer**](class_a_g_e_1_1_timer.md) object is created and assigned to m\_Timer.




**Returns:**

[**Animation**](class_a_g_e_1_1_animation.md) object with all member variables initialized to default values. 





        

<hr>



### function Animation [2/2]

_Copy constructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class._
```C++
AGE::Animation::Animation (
    const Animation &
) = default
```



This function creates a new instance of [**Animation**](class_a_g_e_1_1_animation.md) that is an exact copy of the provided one. It uses the '= default' directive to delegate the work to the compiler, which means it simply calls the copy constructor of the base class (if any) and then copies all non-static data members.




**Parameters:**


* `other` The instance of [**Animation**](class_a_g_e_1_1_animation.md) to be copied.

Copy constructor for the [**Animation**](class_a_g_e_1_1_animation.md) class.


This function creates a new instance of an [**Animation**](class_a_g_e_1_1_animation.md) object by copying all its attributes from another existing [**Animation**](class_a_g_e_1_1_animation.md) object. The copy is done using the '= default' directive, which uses the compiler-generated copy constructor.




**Parameters:**


* `other` The existing [**Animation**](class_a_g_e_1_1_animation.md) object to be copied. 




        

<hr>



### function GetCurrentFrame 

_Returns the current frame number._ 
```C++
inline int AGE::Animation::GetCurrentFrame () 
```



This function retrieves and returns the value of the member variable 'm\_CurrentFrame'. It represents the current frame in a sequence or animation, for instance.




**Returns:**

The current frame number as an integer. If no specific frame is set, it may return 0 or some default value indicating that there's currently no active frame.


This function returns the current frame number.




**Returns:**

The current frame number as an integer. If no frame is currently set, it will return -1. 





        

<hr>



### function GetCurrentTexture 

_Gets the current texture._ 
```C++
inline Ref< SubTexture2D > AGE::Animation::GetCurrentTexture () 
```



This function returns a reference to the currently active subtexture in the sprite sheet. The returned value is a const reference, meaning that it cannot be modified by this function.




**Returns:**

A constant reference to the current texture.


Gets the current texture being used in the game. 

**Returns:**

A reference to the [**SubTexture2D**](class_a_g_e_1_1_sub_texture2_d.md) object representing the current texture. 





        

<hr>



### function GetFrameRate 

_Returns the current frame rate._ 
```C++
inline int AGE::Animation::GetFrameRate () 
```



This function retrieves and returns the current frame rate of the application. The returned value is an integer representing the number of frames per second.




**Returns:**

int - Current frame rate in frames per second. If no frame rate has been set, it will return 0.


Returns the current frame rate.


This function retrieves and returns the current frame rate of the system. The returned value is an integer representing the number of frames per second.




**Returns:**

int - Current frame rate in frames per second. 





        

<hr>



### function GetMaxFrames 

_This function returns the maximum number of frames that can be processed by the system._ 
```C++
inline int AGE::Animation::GetMaxFrames () 
```





**Returns:**

int The maximum number of frames. If no limit is set, it will return -1.


This function returns the maximum number of frames that can be processed by the system. 

**Returns:**

int The maximum number of frames. If no limit is set, it will return a large value (e.g., INT\_MAX). 





        

<hr>



### function GetOscillate 

_Returns the oscillation state of the system._ 
```C++
inline bool AGE::Animation::GetOscillate () 
```



This function returns a boolean value indicating whether or not the system is in an oscillating mode. The actual behavior and meaning of this flag would depend on how it's implemented within the specific context of your codebase.




**Returns:**

True if the system is oscillating, false otherwise.


Returns the oscillation state of the system.


This function returns a boolean value indicating whether or not the system is in an oscillating mode. The actual implementation and meaning of this flag are specific to the application, so it's important to refer to the documentation for that context.




**Returns:**

True if the system is in oscillation mode, false otherwise. 





        

<hr>



### function LoadAnimation 

_Loads an animation into the system based on the provided specification._ 
```C++
void AGE::Animation::LoadAnimation (
    const AnimationSpecification Anim
) 
```



This function takes in a constant reference to an object of type `AnimationSpecification` and uses it to load an animation into the system. The animation is added to the member variable `m_AnimationTextures` as a pair with the key being the movement status from the [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md).




**Parameters:**


* `Anim` A constant reference to an object of type `AnimationSpecification` that contains all necessary information for loading an animation.



**Returns:**

void No return value is expected.


Loads an animation into the system based on the provided specification. 

**Parameters:**


* `Anim` The [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) containing details about the animation to be loaded. 




        

<hr>



### function LoadAnimations 

_Loads a set of animations into the animation system._ 
```C++
void AGE::Animation::LoadAnimations (
    const std::vector< AnimationSpecification > & Anims
) 
```



This function takes in a vector of [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) objects and loads them into the m\_AnimationTextures map. Each element in the vector is added as a pair to the map, with the key being the MovementStatus from each [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) object.




**Parameters:**


* `Anims` - A const reference to a vector of [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) objects. 



**Returns:**

void


Loads a list of animation specifications into the m\_AnimationTextures map.


This function takes in a vector of [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) objects and adds them to the m\_AnimationTextures map, using the MovementStatus field as the key for each entry. The [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) object is then stored as the value associated with its corresponding MovementStatus key.




**Parameters:**


* `Anims` A vector of [**AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) objects to be loaded into the m\_AnimationTextures map. 




        

<hr>



### function OnAnimate 

_Updates the object's animation based on elapsed time._ 
```C++
void AGE::Animation::OnAnimate (
    TimeStep DeltaTime
) 
```



This function checks if enough time has passed to move to the next frame of the animation. If it has, the current frame index is updated and oscillates between min and max frames if the animation should be oscillating.




**Parameters:**


* `DeltaTime` The amount of time that has passed since the last update.

This function is used to animate the object based on a time step.


The function checks if enough time has passed since the last frame update. If it has, the current frame index is updated and oscillates between min and max frames if the 'bOscillate' flag is set. 

**Parameters:**


* `DeltaTime` The time elapsed since the last frame in seconds. 




        

<hr>



### function OnDestroy 

_This function is called when the object is being destroyed._ 
```C++
void AGE::Animation::OnDestroy () 
```





**Returns:**

void No return value.


This function is called when the object is being destroyed.




**Returns:**

void No return value. 





        

<hr>



### function SetCurrentFrame 

_Set the Current_ [_**Animation**_](class_a_g_e_1_1_animation.md) _Frame._
```C++
void AGE::Animation::SetCurrentFrame (
    int Frame
) 
```



This function sets the current frame of an animation. The frame number should be between 0 and m\_MaxFrames - 1, inclusive. If the provided frame is outside this range, the function does nothing.




**Parameters:**


* `Frame` The new frame to set as the current frame.

Set the Current Frame of [**Animation**](class_a_g_e_1_1_animation.md).


This function sets the current frame of an animation to a specified value. If the provided frame number is negative or larger than or equal to the maximum frames, it will return without doing anything.




**Parameters:**


* `Frame` The new frame number to set as the current frame. 




        

<hr>



### function SetCurrentTexture 

_Sets the current texture based on the character movement status._ 
```C++
void AGE::Animation::SetCurrentTexture (
    CharMovementStatus status
) 
```



This function sets the current texture of the animation object to a subtexture corresponding to the provided CharMovementStatus. The subtexture is chosen from the set of animation textures stored in m\_AnimationTextures, and it's determined by the status parameter.




**Parameters:**


* `status` The current movement status of the character. This determines which texture to use for rendering the animation.

Sets the current texture based on the character movement status.


This function sets the current texture of an animation object by taking a CharMovementStatus parameter which indicates the current state of the character. It uses this information to select and set the correct subtexture from the m\_AnimationTextures array. The selected subtexture is then assigned to m\_CurrentTexture.




**Parameters:**


* `status` The current movement status of the character. This can be any value defined in CharMovementStatus enum. 




        

<hr>



### function SetFrameRate 

_Sets the frame rate for a video processing system._ 
```C++
inline void AGE::Animation::SetFrameRate (
    int Rate
) 
```



This function sets the frame rate of the video processing system to the specified value. The frame rate is an integer representing the number of frames processed per second.




**Parameters:**


* `Rate` An integer representing the desired frame rate. Must be greater than 0 and less than or equal to 60. 



**Returns:**

void


Sets the frame rate for a video processing system.


This function sets the frame rate of the video processing system to the specified value. The frame rate is an integer representing the number of frames processed per second.




**Parameters:**


* `Rate` An integer representing the desired frame rate. 




        

<hr>



### function SetMaxFrames 

_Sets the maximum number of frames allowed in a video sequence._ 
```C++
inline void AGE::Animation::SetMaxFrames (
    int Frames
) 
```



This function sets the value for the member variable `m_MaxFrames` to the input parameter `Frames`. It is used to set the upper limit on the number of frames that can be processed in a video sequence.




**Parameters:**


* `Frames` The new maximum number of frames allowed. Must be greater than or equal to zero.

Sets the maximum number of frames allowed in a video sequence.


This function sets the value of the member variable `m_MaxFrames` to the input parameter `Frames`. It is used to limit the length of video sequences processed by other functions in the class.




**Parameters:**


* `Frames` The new maximum number of frames allowed. Must be a positive integer. 




        

<hr>



### function SetOscillate 

_Sets the oscillation state of an object._ 
```C++
inline void AGE::Animation::SetOscillate (
    bool Osc
) 
```



This function sets the 'bOscillate' variable to a specified boolean value, which determines whether or not the object should oscillate.




**Parameters:**


* `Osc` A boolean value indicating if the object should oscillate (true) or not (false).

Sets the oscillation state of an object. 

**Parameters:**


* `Osc` A boolean value indicating whether to oscillate or not. 




        

<hr>



### function ~Animation 

_Destructor for the_ [_**Animation**_](class_a_g_e_1_1_animation.md) _class._
```C++
AGE::Animation::~Animation () = default
```



This function is responsible for releasing any resources that were acquired by the animation object, such as memory or file handles. It does not return anything and has no parameters.


Destructor for the [**Animation**](class_a_g_e_1_1_animation.md) class.


This function is responsible for releasing any resources that were acquired by the animation object, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Animation/Public/Animation.h`

