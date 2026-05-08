

# Class AGE::EditorCamera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**EditorCamera**](class_a_g_e_1_1_editor_camera.md)








Inherits the following classes: [AGE::Camera](class_a_g_e_1_1_camera.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**EditorCamera**](#function-editorcamera-13) () = default<br> |
|   | [**EditorCamera**](#function-editorcamera-23) (float FOV, float AspectRatio, float NearClip, float FarClip) <br> |
|   | [**EditorCamera**](#function-editorcamera-33) (float Size, float NearClip, float FarClip) <br> |
|  float | [**GetDistance**](#function-getdistance) () const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetForwardDirection**](#function-getforwarddirection) () const<br> |
|  glm::quat | [**GetOrientation**](#function-getorientation) () const<br> |
|  float | [**GetPitch**](#function-getpitch) () const<br> |
|  const [**Vector3**](struct_a_g_e_1_1_vector3.md) & | [**GetPosition**](#function-getposition) () const<br> |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetRightDirection**](#function-getrightdirection) () const<br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**GetUpDirection**](#function-getupdirection) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewMatrix**](#function-getviewmatrix-12) () <br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewMatrix**](#function-getviewmatrix-22) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewProjMatrix**](#function-getviewprojmatrix-12) () <br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetViewProjMatrix**](#function-getviewprojmatrix-22) () const<br> |
|  float | [**GetYaw**](#function-getyaw) () const<br> |
|  void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & E) <br> |
|  void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|  void | [**SetDistance**](#function-setdistance) (float Distance) <br> |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) <br> |
|  void | [**SetViewportSize**](#function-setviewportsize) (float Width, float Height) <br> |


## Public Functions inherited from AGE::Camera

See [AGE::Camera](class_a_g_e_1_1_camera.md)

| Type | Name |
| ---: | :--- |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-13) () = default<br> |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-23) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Projection) <br> |
|   | [**Camera**](class_a_g_e_1_1_camera.md#function-camera-33) ([**Vector4**](struct_a_g_e_1_1_vector4.md) Eye, [**Vector4**](struct_a_g_e_1_1_vector4.md) At, [**Vector4**](struct_a_g_e_1_1_vector4.md) Up) <br> |
|  const [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](class_a_g_e_1_1_camera.md#function-getconstantbufferdata-12) () const<br> |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](class_a_g_e_1_1_camera.md#function-getconstantbufferdata-22) () <br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](class_a_g_e_1_1_camera.md#function-getprojection-12) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](class_a_g_e_1_1_camera.md#function-getprojection-22) () <br> |
|  ProjectionType | [**GetProjectionType**](class_a_g_e_1_1_camera.md#function-getprojectiontype) () const<br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](class_a_g_e_1_1_camera.md#function-getworldmatrix-12) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](class_a_g_e_1_1_camera.md#function-getworldmatrix-22) () <br> |
| virtual void | [**SetProjectionType**](class_a_g_e_1_1_camera.md#function-setprojectiontype) (ProjectionType Type) <br> |
| virtual  | [**~Camera**](class_a_g_e_1_1_camera.md#function-camera) () <br> |
















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

```C++
AGE::EditorCamera::EditorCamera () = default
```




<hr>



### function EditorCamera [2/3]

```C++
AGE::EditorCamera::EditorCamera (
    float FOV,
    float AspectRatio,
    float NearClip,
    float FarClip
) 
```




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

```C++
inline float AGE::EditorCamera::GetDistance () const
```




<hr>



### function GetForwardDirection 

```C++
Vector3 AGE::EditorCamera::GetForwardDirection () const
```




<hr>



### function GetOrientation 

```C++
glm::quat AGE::EditorCamera::GetOrientation () const
```




<hr>



### function GetPitch 

```C++
inline float AGE::EditorCamera::GetPitch () const
```




<hr>



### function GetPosition 

```C++
inline const Vector3 & AGE::EditorCamera::GetPosition () const
```




<hr>



### function GetProjectionType 

```C++
inline ProjectionType AGE::EditorCamera::GetProjectionType () const
```




<hr>



### function GetRightDirection 

```C++
Vector3 AGE::EditorCamera::GetRightDirection () const
```




<hr>



### function GetUpDirection 

```C++
Vector3 AGE::EditorCamera::GetUpDirection () const
```




<hr>



### function GetViewMatrix [1/2]

```C++
inline Matrix4D AGE::EditorCamera::GetViewMatrix () 
```




<hr>



### function GetViewMatrix [2/2]

```C++
inline const Matrix4D AGE::EditorCamera::GetViewMatrix () const
```




<hr>



### function GetViewProjMatrix [1/2]

```C++
inline Matrix4D AGE::EditorCamera::GetViewProjMatrix () 
```




<hr>



### function GetViewProjMatrix [2/2]

```C++
inline const Matrix4D AGE::EditorCamera::GetViewProjMatrix () const
```




<hr>



### function GetYaw 

```C++
inline float AGE::EditorCamera::GetYaw () const
```




<hr>



### function OnEvent 

```C++
void AGE::EditorCamera::OnEvent (
    Event & E
) 
```




<hr>



### function OnUpdate 

```C++
void AGE::EditorCamera::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function SetDistance 

```C++
inline void AGE::EditorCamera::SetDistance (
    float Distance
) 
```




<hr>



### function SetProjectionType 

```C++
inline virtual void AGE::EditorCamera::SetProjectionType (
    ProjectionType Type
) 
```



Implements [*AGE::Camera::SetProjectionType*](class_a_g_e_1_1_camera.md#function-setprojectiontype)


<hr>



### function SetViewportSize 

```C++
inline void AGE::EditorCamera::SetViewportSize (
    float Width,
    float Height
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Camera/Public/EditorCamera.h`

