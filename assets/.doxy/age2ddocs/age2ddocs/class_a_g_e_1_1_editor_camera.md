

# Class AGE::EditorCamera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**EditorCamera**](class_a_g_e_1_1_editor_camera.md)








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
|   | [**EditorCamera**](#function-editorcamera-13) () = default<br>_Default constructor for the_ [_**EditorCamera**_](class_a_g_e_1_1_editor_camera.md) _class._ |
|   | [**EditorCamera**](#function-editorcamera-23) (float FOV, float AspectRatio, float NearClip, float FarClip) <br>_Constructor for the_ [_**EditorCamera**_](class_a_g_e_1_1_editor_camera.md) _class._ |
|   | [**EditorCamera**](#function-editorcamera-33) (float Size, float NearClip, float FarClip) <br> |
|  float | [**GetDistance**](#function-getdistance) () const<br>_This function returns the distance value._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetForwardDirection**](#function-getforwarddirection) () const<br>_Get the forward direction of the camera in world space coordinates._  |
|  glm::quat | [**GetOrientation**](#function-getorientation) () const<br>_Get the orientation of the editor camera as a quaternion._  |
|  float | [**GetPitch**](#function-getpitch) () const<br>_This function returns the current pitch value._  |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetPosition**](#function-getposition) () const<br>_Returns the current position of the object._  |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br>_Returns the projection type of this object._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetRightDirection**](#function-getrightdirection) () const<br>_Get the right direction of the camera._  |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetUpDirection**](#function-getupdirection) () const<br>_This function returns the up direction of the camera in world space coordinates._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewMatrix**](#function-getviewmatrix-12) () <br>_Returns the view matrix of the camera._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewMatrix**](#function-getviewmatrix-22) () const<br>_Returns the view matrix of the camera._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewProjMatrix**](#function-getviewprojmatrix-12) () <br>_This function returns the view-projection matrix of the camera._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewProjMatrix**](#function-getviewprojmatrix-22) () const<br>_Calculates the view-projection matrix for this camera._  |
|  float | [**GetYaw**](#function-getyaw) () const<br>_This function returns the yaw value of an object._  |
|  void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br>_Handles events related to the camera._  |
|  void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**SetDistance**](#function-setdistance) (float Distance) <br>_This function sets the distance value._  |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) <br>_Sets the projection type of the object._  |
|  void | [**SetViewportSize**](#function-setviewportsize) (float Width, float Height) <br>_Set the viewport size and update the projection matrix._  |


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




### function EditorCamera [1/3]

_Default constructor for the_ [_**EditorCamera**_](class_a_g_e_1_1_editor_camera.md) _class._
```C++
AGE::EditorCamera::EditorCamera () = default
```



This function initializes an instance of the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class with default values. It does not take any parameters and returns nothing.


Default constructor for the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class. 


        

<hr>



### function EditorCamera [2/3]

_Constructor for the_ [_**EditorCamera**_](class_a_g_e_1_1_editor_camera.md) _class._
```C++
AGE::EditorCamera::EditorCamera (
    float FOV,
    float AspectRatio,
    float NearClip,
    float FarClip
) 
```



This constructor initializes an instance of the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class with a given field of view (FOV), aspect ratio, near clip plane and far clip plane. It also calls UpdateView to update the camera's view matrix based on these parameters.




**Parameters:**


* `FOV` The Field of View for the camera in degrees. 
* `AspectRatio` The aspect ratio of the camera view (width/height). 
* `NearClip` The distance to the near clipping plane. 
* `FarClip` The distance to the far clipping plane.

Constructor for the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class.


This constructor initializes an instance of the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class with a specified field of view (FOV), aspect ratio, near clip plane and far clip plane. It also calls UpdateView() to update the camera's view matrix based on these parameters.




**Parameters:**


* `FOV` The Field of View for the camera in degrees. 
* `AspectRatio` The aspect ratio of the camera (width/height). 
* `NearClip` The distance from the camera to the near clip plane. 
* `FarClip` The distance from the camera to the far clip plane. 




        

<hr>



### function EditorCamera [3/3]

```C++
AGE::EditorCamera::EditorCamera (
    float Size,
    float NearClip,
    float FarClip
) 
```




<hr>



### function GetDistance 

_This function returns the distance value._ 
```C++
inline float AGE::EditorCamera::GetDistance () const
```





**Returns:**

A floating-point number representing the distance.


This function returns the distance value. 

**Returns:**

A floating-point number representing the distance. 





        

<hr>



### function GetForwardDirection 

_Get the forward direction of the camera in world space coordinates._ 
```C++
Vector3 AGE::EditorCamera::GetForwardDirection () const
```



This function returns a [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the forward direction of the camera. The direction is calculated by rotating the default forward vector (-Z axis) by the current orientation of the camera.




**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the forward direction of the camera.


Get the forward direction of the camera in world space coordinates.


This function returns a [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the forward direction of the camera. The direction is calculated by rotating the default forward vector (-Z axis) by the current orientation of the camera.




**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the forward direction of the camera. 





        

<hr>



### function GetOrientation 

_Get the orientation of the editor camera as a quaternion._ 
```C++
glm::quat AGE::EditorCamera::GetOrientation () const
```



This function returns the current orientation of the editor camera in the form of a quaternion. The quaternion is defined by four components (x, y, z, w) and represents a rotation in 3D space. In this case, it's being used to represent pitch and yaw angles of the camera.




**Returns:**

glm::quat A quaternion representing the current orientation of the editor camera. The components are (-pitch, -yaw, 0.f).


Get the orientation of the editor camera as a quaternion.


This function returns the current orientation of the editor camera in the form of a quaternion. The quaternion is defined by an array of four components, where the first three represent the rotation angles around the x, y and z axes respectively. In this case, we are only considering the yaw (y-axis) and pitch (x-axis) rotations, so the third component is zero.




**Returns:**

glm::quat A quaternion representing the current orientation of the editor camera. 





        

<hr>



### function GetPitch 

_This function returns the current pitch value._ 
```C++
inline float AGE::EditorCamera::GetPitch () const
```





**Returns:**

A float representing the current pitch value. If there is an error in retrieving the value, it will return Unknown.


This function returns the current pitch value. 

**Returns:**

The pitch value as a float. If no pitch is set, it will return Unknown. 





        

<hr>



### function GetPosition 

_Returns the current position of the object._ 
```C++
inline const Vector3 & AGE::EditorCamera::GetPosition () const
```





**Returns:**

A constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the current position.


Returns the current position of the object. 

**Returns:**

A constant reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the current position. 





        

<hr>



### function GetProjectionType 

_Returns the projection type of this object._ 
```C++
inline ProjectionType AGE::EditorCamera::GetProjectionType () const
```





**Returns:**

ProjectionType - The current projection type of this object.


Returns the projection type of the camera. 

**Returns:**

ProjectionType - The current projection type (ORTHOGRAPHIC, PERSPECTIVE). 





        

<hr>



### function GetRightDirection 

_Get the right direction of the camera._ 
```C++
Vector3 AGE::EditorCamera::GetRightDirection () const
```



This function returns the right direction vector of the camera. The direction is calculated by rotating a standard (1,0,0) vector around the y-axis by the current orientation of the camera.




**Returns:**

[**Vector3**](struct_a_g_e_1_1_vector3.md) - The right direction vector of the camera.


Get the right direction of the camera in world space.


This function returns the right direction vector of the camera in world space. The direction is calculated by rotating the initial x-axis (1,0,0) by the current orientation of the camera.




**Returns:**

[**Vector3**](struct_a_g_e_1_1_vector3.md) - The right direction vector of the camera in world space. 





        

<hr>



### function GetUpDirection 

_This function returns the up direction of the camera in world space coordinates._ 
```C++
Vector3 AGE::EditorCamera::GetUpDirection () const
```





**Returns:**

A [**Vector3**](struct_a_g_e_1_1_vector3.md) representing the up direction in world space.


Get the up direction of the camera in world space coordinates.


This function returns the up direction of the camera in world space coordinates. The direction is calculated by rotating the default up direction (0,1,0) by the current orientation of the camera.




**Returns:**

[**Vector3**](struct_a_g_e_1_1_vector3.md) - The up direction of the camera in world space coordinates. 





        

<hr>



### function GetViewMatrix [1/2]

_Returns the view matrix of the camera._ 
```C++
inline Matrix4D AGE::EditorCamera::GetViewMatrix () 
```



This function returns the current view matrix used by the camera in the scene. The returned value is a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the view transformation.




**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object containing the view matrix.


Returns the view matrix of the camera.


This function returns the current view matrix used by the camera in the scene. The view matrix is a transformation matrix that defines the position and orientation of the camera in the world space.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) - The 4x4 view matrix. 





        

<hr>



### function GetViewMatrix [2/2]

_Returns the view matrix of the camera._ 
```C++
inline const Matrix4D AGE::EditorCamera::GetViewMatrix () const
```



This function returns the current view matrix of the camera, which is used to transform world space coordinates into camera space for rendering.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The view matrix of the camera.


Returns the view matrix of the camera.


This function returns the current view matrix used by the camera in the scene. The returned matrix can be used for rendering objects from a specific point of view.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) - The 4x4 view matrix. 





        

<hr>



### function GetViewProjMatrix [1/2]

_This function returns the view-projection matrix of the camera._ 
```C++
inline Matrix4D AGE::EditorCamera::GetViewProjMatrix () 
```





**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The result is a 4x4 matrix that represents the combined transformation from world space to camera space.


Calculates the view-projection matrix of the camera.


This function multiplies the projection and view matrices to get the final view-projection matrix. The resulting [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object represents this transformation.




**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the combined view-projection matrix. 





        

<hr>



### function GetViewProjMatrix [2/2]

_Calculates the view-projection matrix for this camera._ 
```C++
inline const Matrix4D AGE::EditorCamera::GetViewProjMatrix () const
```



This function multiplies the projection and view matrices of the camera to get the final view-projection matrix. The resulting [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object represents the combined transformations of the camera.




**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the combined transformation of the camera's projection and view matrices.


Calculates the view-projection matrix for this camera instance.


This function multiplies the projection and view matrices of the camera to get the final view-projection matrix. The resulting [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object represents the combined transformation that takes a point in world space and transforms it into eye space (viewing coordinates) before projecting onto the screen.




**Returns:**

A [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object representing the combined projection and view matrices of this camera instance. 





        

<hr>



### function GetYaw 

_This function returns the yaw value of an object._ 
```C++
inline float AGE::EditorCamera::GetYaw () const
```





**Returns:**

A float representing the current yaw angle in radians.


This function returns the current yaw value of an object. 

**Returns:**

A float representing the current yaw value. 





        

<hr>



### function OnEvent 

_Handles events related to the camera._ 
```C++
void AGE::EditorCamera::OnEvent (
    Event & E
) 
```



This function is responsible for dispatching specific event types that are relevant to the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class, such as mouse scrolling events.




**Parameters:**


* `E` The event to be handled.

Handles events for the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md) class.


This function is responsible for dispatching specific event types that are relevant to the [**EditorCamera**](class_a_g_e_1_1_editor_camera.md), such as [**MouseScrolledEvent**](class_a_g_e_1_1_mouse_scrolled_event.md). It uses an [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md) object to handle these events and calls appropriate callback functions (in this case, OnMouseScrolled). The function takes a reference to an [**Event**](class_a_g_e_1_1_event.md) object as its parameter.




**Parameters:**


* `E` Reference to the event that needs to be handled. 




        

<hr>



### function OnUpdate 

```C++
void AGE::EditorCamera::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function SetDistance 

_This function sets the distance value._ 
```C++
inline void AGE::EditorCamera::SetDistance (
    float Distance
) 
```





**Parameters:**


* `Distance` The new distance value to be set.

This function sets the distance value. 

**Parameters:**


* `Distance` The new distance value to be set. 




        

<hr>



### function SetProjectionType 

_Sets the projection type of the object._ 
```C++
inline virtual void AGE::EditorCamera::SetProjectionType (
    ProjectionType Type
) 
```





**Parameters:**


* `Type` The ProjectionType to be set. 



**Returns:**

void


Sets the projection type of the object.


This function sets the ProjectionType member variable to a given value. It allows for easy switching between different types of projections.




**Parameters:**


* `Type` The new ProjectionType to be set. 




        
Implements [*AGE::Camera::SetProjectionType*](class_a_g_e_1_1_camera.md#function-setprojectiontype)


<hr>



### function SetViewportSize 

_Set the viewport size and update the projection matrix._ 
```C++
inline void AGE::EditorCamera::SetViewportSize (
    float Width,
    float Height
) 
```



This function sets the width and height of the viewport, calculates the aspect ratio from these values, and then updates the projection matrix based on these new dimensions.




**Parameters:**


* `Width` The new width of the viewport. 
* `Height` The new height of the viewport.

Set the viewport size and aspect ratio.


This function sets the width, height, and aspect ratio of the viewport based on the provided parameters. It also calls `UpdateProjection()` to update any projection matrices that depend on these values.




**Parameters:**


* `Width` The new width of the viewport. 
* `Height` The new height of the viewport. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Camera/Public/EditorCamera.h`

