

# Class AGE::SceneCamera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneCamera**](class_a_g_e_1_1_scene_camera.md)








Inherits the following classes: [AGE::Camera](class_a_g_e_1_1_camera.md)
























## Public Attributes inherited from AGE::Camera

See [AGE::Camera](class_a_g_e_1_1_camera.md)

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](class_a_g_e_1_1_camera.md#variable-__pad0__)  <br>_Default constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._ |
|  COMMENT | [**\_\_pad1\_\_**](class_a_g_e_1_1_camera.md#variable-__pad1__)  <br> |
|  COMMENT | [**\_\_pad2\_\_**](class_a_g_e_1_1_camera.md#variable-__pad2__)  <br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetOrthographicFarClip**](#function-getorthographicfarclip) () const<br>_This function returns the orthographic far clip value._  |
|  float | [**GetOrthographicNearClip**](#function-getorthographicnearclip) () const<br>_This function returns the near clipping plane of the camera in orthographic mode._  |
|  float | [**GetOrthographicSize**](#function-getorthographicsize) () const<br>_This function returns the orthographic size of the camera._  |
|  float | [**GetPerspectiveFarClip**](#function-getperspectivefarclip) () const<br>_This function returns the perspective far clip value._  |
|  float | [**GetPerspectiveNearClip**](#function-getperspectivenearclip) () const<br>_This function returns the near clipping plane of the perspective projection._  |
|  float | [**GetPerspectiveVerticalFOV**](#function-getperspectiveverticalfov) () const<br>_This function returns the vertical field of view for a perspective camera._  |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br>_Returns the projection type of this object._  |
|   | [**SceneCamera**](#function-scenecamera) () <br>_Constructor for the_ [_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _class. Initializes a new instance of_[_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _and calls RecalculateProjection to set up the projection matrix._ |
|  void | [**SetOrthographic**](#function-setorthographic) (float Size, float NearClip, float FarClip) <br>_Sets the camera's projection to Orthographic._  |
|  void | [**SetOrthographicFarClip**](#function-setorthographicfarclip) (float FarClip) <br>_Sets the far clip plane for an orthographic projection._  |
|  void | [**SetOrthographicNearClip**](#function-setorthographicnearclip) (float NearClip) <br>_Sets the near clipping plane for an orthographic projection._  |
|  void | [**SetOrthographicSize**](#function-setorthographicsize) (float Size) <br>_Sets the orthographic size for the camera._  |
|  void | [**SetPerspective**](#function-setperspective) (float VerticalFOV, float NearClip, float FarClip) <br>_Sets the perspective parameters of the camera._  |
|  void | [**SetPerspectiveFarClip**](#function-setperspectivefarclip) (float FarClip) <br>_Sets the perspective far clip plane value._  |
|  void | [**SetPerspectiveNearClip**](#function-setperspectivenearclip) (float NearClip) <br>_Sets the perspective near clip plane value._  |
|  void | [**SetPerspectiveVerticalFOV**](#function-setperspectiveverticalfov) (float VerticalFOV) <br>_Sets the vertical field of view for the perspective projection._  |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) override<br>_This function sets the projection type and adjusts the corresponding parameters accordingly._  |
|  void | [**SetViewportSize**](#function-setviewportsize) (uint32\_t Width, uint32\_t Height) <br>_Set the viewport size of the scene camera._  |
| virtual  | [**~SceneCamera**](#function-scenecamera) () = default<br>_Virtual destructor for the_ [_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _class._ |


## Public Functions inherited from AGE::Camera

See [AGE::Camera](class_a_g_e_1_1_camera.md)

| Type | Name |
| ---: | :--- |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-13) () = default<br> |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-23) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Projection) <br> |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-33) ([**Vector4**](struct_a_g_e_1_1_vector4.md) Eye, [**Vector4**](struct_a_g_e_1_1_vector4.md) At, [**Vector4**](struct_a_g_e_1_1_vector4.md) Up) <br>_Constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class that initializes a camera with an eye position, at position and up direction._ |
|  const [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](class_a_g_e_1_1_camera.md#function-getconstantbufferdata-12) () const<br>_This function returns the constant buffer data._  |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](class_a_g_e_1_1_camera.md#function-getconstantbufferdata-22) () <br>_This function returns the constant buffer data._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](class_a_g_e_1_1_camera.md#function-getprojection-12) () const<br>_Returns the projection matrix used for rendering._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](class_a_g_e_1_1_camera.md#function-getprojection-22) () <br>_Returns the projection matrix of the camera._  |
|  ProjectionType | [**GetProjectionType**](class_a_g_e_1_1_camera.md#function-getprojectiontype) () const<br>_Returns the projection type of this object._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](class_a_g_e_1_1_camera.md#function-getworldmatrix-12) () const<br>_Returns the world matrix of the object._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](class_a_g_e_1_1_camera.md#function-getworldmatrix-22) () <br>_Returns the world matrix of the object._  |
| virtual void | [**SetProjectionType**](class_a_g_e_1_1_camera.md#function-setprojectiontype) (ProjectionType Type) <br>_Sets the projection type of the object._  |
| virtual  | [**~Camera**](class_a_g_e_1_1_camera.md#function-camera) () <br>_Virtual destructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._ |
















## Protected Attributes inherited from AGE::Camera

See [AGE::Camera](class_a_g_e_1_1_camera.md)

| Type | Name |
| ---: | :--- |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**m\_ConstantBuffer**](class_a_g_e_1_1_camera.md#variable-m_constantbuffer)  <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_Projection**](class_a_g_e_1_1_camera.md#variable-m_projection)   = `{ 1.f }`<br> |
|  ProjectionType | [**m\_ProjectionType**](class_a_g_e_1_1_camera.md#variable-m_projectiontype)   = `ProjectionType::Orthographic`<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_World**](class_a_g_e_1_1_camera.md#variable-m_world)   = `{ 1.f }`<br> |






































## Public Functions Documentation




### function GetOrthographicFarClip 

_This function returns the orthographic far clip value._ 
```C++
inline float AGE::SceneCamera::GetOrthographicFarClip () const
```





**Returns:**

A float representing the orthographic far clip value.


Returns the orthographic far clip plane value.


This function returns the current value of the orthographic far clip plane, which is used to determine how far objects are clipped in an orthographic perspective.




**Returns:**

The current value of m\_OrthographicFar as a float. 





        

<hr>



### function GetOrthographicNearClip 

_This function returns the near clipping plane of the camera in orthographic mode._ 
```C++
inline float AGE::SceneCamera::GetOrthographicNearClip () const
```





**Returns:**

A float representing the near clipping plane value.


Returns the near clipping plane for an orthographic camera. 

**Returns:**

The near clipping plane value as a float. 





        

<hr>



### function GetOrthographicSize 

_This function returns the orthographic size of the camera._ 
```C++
inline float AGE::SceneCamera::GetOrthographicSize () const
```





**Returns:**

A float representing the current orthographic size.


Returns the orthographic size of the camera. 

**Returns:**

A float representing the current orthographic size. 





        

<hr>



### function GetPerspectiveFarClip 

_This function returns the perspective far clip value._ 
```C++
inline float AGE::SceneCamera::GetPerspectiveFarClip () const
```





**Returns:**

A float representing the perspective far clip value.


This function returns the perspective far clip plane value. 

**Returns:**

A float representing the perspective far clip plane value. 





        

<hr>



### function GetPerspectiveNearClip 

_This function returns the near clipping plane of the perspective projection._ 
```C++
inline float AGE::SceneCamera::GetPerspectiveNearClip () const
```





**Returns:**

A float representing the near clipping plane value.


Returns the perspective near clip plane value.


This function returns the current value of the perspective near clip plane, which is used in rendering calculations to determine what objects are visible on the screen.




**Returns:**

The current value of the perspective near clip plane as a float. 





        

<hr>



### function GetPerspectiveVerticalFOV 

_This function returns the vertical field of view for a perspective camera._ 
```C++
inline float AGE::SceneCamera::GetPerspectiveVerticalFOV () const
```





**Returns:**

A float representing the vertical FOV in degrees.


This function returns the vertical field of view for a perspective camera. 

**Returns:**

A float representing the vertical FOV in degrees. 





        

<hr>



### function GetProjectionType 

_Returns the projection type of this object._ 
```C++
inline ProjectionType AGE::SceneCamera::GetProjectionType () const
```





**Returns:**

The ProjectionType of this object, which can be either ORTHOGRAPHIC or PERSPECTIVE.


Gets the projection type of this object.




**Returns:**

The ProjectionType of this object. 





        

<hr>



### function SceneCamera 

_Constructor for the_ [_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _class. Initializes a new instance of_[_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _and calls RecalculateProjection to set up the projection matrix._
```C++
AGE::SceneCamera::SceneCamera () 
```



Constructor for the [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) class. Initializes a new instance of the [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) with default values and calculates the projection matrix. 


        

<hr>



### function SetOrthographic 

_Sets the camera's projection to Orthographic._ 
```C++
void AGE::SceneCamera::SetOrthographic (
    float Size,
    float NearClip,
    float FarClip
) 
```



This function sets the camera's projection type to Orthographic and updates the size, near clip, and far clip values. It then calls RecalculateProjection() to recreate the projection matrix based on these new values. 

**Parameters:**


* `Size` The desired orthographic size (width or height). 
* `NearClip` The distance from the camera to the near clipping plane. 
* `FarClip` The distance from the camera to the far clipping plane.

Sets the camera's projection to an orthographic projection.


This function sets the camera's projection type to Orthographic and updates the size, near clip, and far clip values for the new projection. It then calls RecalculateProjection() to recreate the projection matrix based on these new parameters.




**Parameters:**


* `Size` The desired orthographic size (half of width or height). 
* `NearClip` The distance from the camera to the near clipping plane. 
* `FarClip` The distance from the camera to the far clipping plane. 




        

<hr>



### function SetOrthographicFarClip 

_Sets the far clip plane for an orthographic projection._ 
```C++
inline void AGE::SceneCamera::SetOrthographicFarClip (
    float FarClip
) 
```



This function sets the 'm\_OrthographicFar' variable to the provided parameter 'FarClip'. It then calls RecalculateProjection() to update any associated projection matrices with this new value.




**Parameters:**


* `FarClip` The new far clip plane value.

Sets the far clip plane for an orthographic projection.


This function sets the 'm\_OrthographicFar' member variable to the provided parameter, and then calls the 'RecalculateProjection()' function to update the projection matrix based on this new value. The purpose of this function is to allow for dynamic adjustment of the far clip plane distance in an orthographic projection.




**Parameters:**


* `FarClip` A float representing the desired far clip plane distance. 




        

<hr>



### function SetOrthographicNearClip 

_Sets the near clipping plane for an orthographic projection._ 
```C++
inline void AGE::SceneCamera::SetOrthographicNearClip (
    float NearClip
) 
```



This function sets the value of the member variable `m_OrthographicNear` to the provided parameter `NearClip`, and then calls the `RecalculateProjection()` function to update the projection matrix based on this new near clipping plane value.




**Parameters:**


* `NearClip` The new near clipping plane value. This should be a positive number that is less than or equal to the far clipping plane value (`m_OrthographicFar`).

Sets the near clip plane for an orthographic projection.


This function sets the value of the member variable `m_OrthographicNear` to the provided parameter `NearClip`, and then calls the `RecalculateProjection()` function to update the projection matrix based on this new near clip plane value.




**Parameters:**


* `NearClip` The new near clip plane value to be set. This should be a positive float number representing the distance from the camera to the near clipping plane in world units. 




        

<hr>



### function SetOrthographicSize 

_Sets the orthographic size for the camera._ 
```C++
inline void AGE::SceneCamera::SetOrthographicSize (
    float Size
) 
```



This function sets the orthographic size of the camera, which determines how large the visible area is in world units. The aspect ratio and near/far planes are also updated to maintain the same view frustum.




**Parameters:**


* `Size` The new orthographic size for the camera. Must be greater than 0.

Sets the orthographic size for the camera. 

**Parameters:**


* `Size` The new orthographic size to be set. 



**Returns:**

None 





        

<hr>



### function SetPerspective 

_Sets the perspective parameters of the camera._ 
```C++
void AGE::SceneCamera::SetPerspective (
    float VerticalFOV,
    float NearClip,
    float FarClip
) 
```



This function sets the vertical field of view (FOV), near clip plane, and far clip plane for a perspective projection. It also recalculates the projection matrix based on these new values.




**Parameters:**


* `VerticalFOV` The vertical field of view in degrees. 
* `NearClip` The distance to the near clipping plane. 
* `FarClip` The distance to the far clipping plane.



**Returns:**

void


Set the perspective parameters of the camera.


This function sets the vertical field of view (FOV), near clip plane, and far clip plane for a perspective projection. It also recalculates the projection matrix based on these new values.




**Parameters:**


* `VerticalFOV` The vertical field of view in degrees. 
* `NearClip` The distance to the near clipping plane. 
* `FarClip` The distance to the far clipping plane.



**Returns:**

void 





        

<hr>



### function SetPerspectiveFarClip 

_Sets the perspective far clip plane value._ 
```C++
inline void AGE::SceneCamera::SetPerspectiveFarClip (
    float FarClip
) 
```



This function sets the far clip plane of the perspective projection matrix to a new value. It updates the member variable m\_PerspectiveFar with the provided parameter and then calls RecalculateProjection() to recalculate the projection matrix based on the updated values.




**Parameters:**


* `FarClip` The new far clip plane value.

Sets the perspective far clip plane value.


This function sets the far clip plane of the perspective projection matrix to a new value. It updates the member variable m\_PerspectiveFar with the provided parameter and then calls RecalculateProjection() to recalculate the projection matrix based on the updated values.




**Parameters:**


* `FarClip` The new far clip plane value. 




        

<hr>



### function SetPerspectiveNearClip 

_Sets the perspective near clip plane value._ 
```C++
inline void AGE::SceneCamera::SetPerspectiveNearClip (
    float NearClip
) 
```



This function sets the near clipping plane for a perspective projection matrix. It updates the private member variable m\_PerspectiveNear with the provided NearClip parameter and then calls RecalculateProjection() to recalculate the projection matrix based on the new near clip plane value.




**Parameters:**


* `NearClip` The new near clipping plane value.

Sets the perspective near clip plane value.


This function sets the near clipping plane for a perspective projection matrix. It updates the member variable m\_PerspectiveNear with the provided NearClip parameter and then calls RecalculateProjection() to recalculate the projection matrix based on the new near clip plane value.




**Parameters:**


* `NearClip` The new near clipping plane value to be set. 




        

<hr>



### function SetPerspectiveVerticalFOV 

_Sets the vertical field of view for the perspective projection._ 
```C++
inline void AGE::SceneCamera::SetPerspectiveVerticalFOV (
    float VerticalFOV
) 
```



This function sets the value of the member variable `m_PerspectiveFOV` to the input parameter `VerticalFOV`, and then calls the `RecalculateProjection()` function to update the perspective matrix based on this new field of view.




**Parameters:**


* `VerticalFOV` The new vertical field of view in degrees.

Sets the vertical field of view for a perspective projection.


This function updates the private member variable `m_PerspectiveFOV` with the provided value and then calls `RecalculateProjection()` to update any associated projection matrices based on this new FOV value.




**Parameters:**


* `VerticalFOV` The new vertical field of view angle in degrees. 




        

<hr>



### function SetProjectionType 

_This function sets the projection type and adjusts the corresponding parameters accordingly._ 
```C++
inline virtual void AGE::SceneCamera::SetProjectionType (
    ProjectionType Type
) override
```





**Parameters:**


* `Type` The new ProjectionType to be set.



**Returns:**

void


Sets the projection type and adjusts the corresponding parameters.


This function sets the ProjectionType to the provided value and then calls either SetPerspective or SetOrthographic, depending on the new ProjectionType. The SetPerspective function is called if the ProjectionType is 0 (perspective), while the SetOrthographic function is called for any other value.




**Parameters:**


* `Type` The new ProjectionType to set. 




        
Implements [*AGE::Camera::SetProjectionType*](class_a_g_e_1_1_camera.md#function-setprojectiontype)


<hr>



### function SetViewportSize 

_Set the viewport size of the scene camera._ 
```C++
void AGE::SceneCamera::SetViewportSize (
    uint32_t Width,
    uint32_t Height
) 
```



This function sets the width and height of the viewport, calculates the aspect ratio based on these dimensions, and updates the projection matrix accordingly.




**Parameters:**


* `Width` The new width of the viewport. 
* `Height` The new height of the viewport.

Sets the viewport size and recalculates the projection matrix.


This function sets the width and height of the viewport, calculates the aspect ratio from these values, and then calls RecalculateProjection() to update the projection matrix based on this new aspect ratio. 

**Parameters:**


* `Width` The width of the viewport in pixels. 
* `Height` The height of the viewport in pixels. 




        

<hr>



### function ~SceneCamera 

_Virtual destructor for the_ [_**SceneCamera**_](class_a_g_e_1_1_scene_camera.md) _class._
```C++
virtual AGE::SceneCamera::~SceneCamera () = default
```



This function is responsible for releasing any resources that were acquired by the [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) object, such as memory or file handles. It does not return anything and has no parameters.


Virtual destructor for the [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) class.


This function is responsible for releasing any resources that were acquired by the [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) object during its lifetime. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/SceneCamera.h`

