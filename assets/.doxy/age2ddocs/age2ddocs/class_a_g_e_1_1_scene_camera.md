

# Class AGE::SceneCamera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**SceneCamera**](class_a_g_e_1_1_scene_camera.md)








Inherits the following classes: [AGE::Camera](class_a_g_e_1_1_camera.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  float | [**GetOrthographicFarClip**](#function-getorthographicfarclip) () const<br> |
|  float | [**GetOrthographicNearClip**](#function-getorthographicnearclip) () const<br> |
|  float | [**GetOrthographicSize**](#function-getorthographicsize) () const<br> |
|  float | [**GetPerspectiveFarClip**](#function-getperspectivefarclip) () const<br> |
|  float | [**GetPerspectiveNearClip**](#function-getperspectivenearclip) () const<br> |
|  float | [**GetPerspectiveVerticalFOV**](#function-getperspectiveverticalfov) () const<br> |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br> |
|   | [**SceneCamera**](#function-scenecamera) () <br> |
|  void | [**SetOrthographic**](#function-setorthographic) (float Size, float NearClip, float FarClip) <br> |
|  void | [**SetOrthographicFarClip**](#function-setorthographicfarclip) (float FarClip) <br> |
|  void | [**SetOrthographicNearClip**](#function-setorthographicnearclip) (float NearClip) <br> |
|  void | [**SetOrthographicSize**](#function-setorthographicsize) (float Size) <br> |
|  void | [**SetPerspective**](#function-setperspective) (float VerticalFOV, float NearClip, float FarClip) <br> |
|  void | [**SetPerspectiveFarClip**](#function-setperspectivefarclip) (float FarClip) <br> |
|  void | [**SetPerspectiveNearClip**](#function-setperspectivenearclip) (float NearClip) <br> |
|  void | [**SetPerspectiveVerticalFOV**](#function-setperspectiveverticalfov) (float VerticalFOV) <br> |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) override<br> |
|  void | [**SetViewportSize**](#function-setviewportsize) (uint32\_t Width, uint32\_t Height) <br> |
| virtual  | [**~SceneCamera**](#function-scenecamera) () = default<br> |


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




### function GetOrthographicFarClip 

```C++
inline float AGE::SceneCamera::GetOrthographicFarClip () const
```




<hr>



### function GetOrthographicNearClip 

```C++
inline float AGE::SceneCamera::GetOrthographicNearClip () const
```




<hr>



### function GetOrthographicSize 

```C++
inline float AGE::SceneCamera::GetOrthographicSize () const
```




<hr>



### function GetPerspectiveFarClip 

```C++
inline float AGE::SceneCamera::GetPerspectiveFarClip () const
```




<hr>



### function GetPerspectiveNearClip 

```C++
inline float AGE::SceneCamera::GetPerspectiveNearClip () const
```




<hr>



### function GetPerspectiveVerticalFOV 

```C++
inline float AGE::SceneCamera::GetPerspectiveVerticalFOV () const
```




<hr>



### function GetProjectionType 

```C++
inline ProjectionType AGE::SceneCamera::GetProjectionType () const
```




<hr>



### function SceneCamera 

```C++
AGE::SceneCamera::SceneCamera () 
```




<hr>



### function SetOrthographic 

```C++
void AGE::SceneCamera::SetOrthographic (
    float Size,
    float NearClip,
    float FarClip
) 
```




<hr>



### function SetOrthographicFarClip 

```C++
inline void AGE::SceneCamera::SetOrthographicFarClip (
    float FarClip
) 
```




<hr>



### function SetOrthographicNearClip 

```C++
inline void AGE::SceneCamera::SetOrthographicNearClip (
    float NearClip
) 
```




<hr>



### function SetOrthographicSize 

```C++
inline void AGE::SceneCamera::SetOrthographicSize (
    float Size
) 
```




<hr>



### function SetPerspective 

```C++
void AGE::SceneCamera::SetPerspective (
    float VerticalFOV,
    float NearClip,
    float FarClip
) 
```




<hr>



### function SetPerspectiveFarClip 

```C++
inline void AGE::SceneCamera::SetPerspectiveFarClip (
    float FarClip
) 
```




<hr>



### function SetPerspectiveNearClip 

```C++
inline void AGE::SceneCamera::SetPerspectiveNearClip (
    float NearClip
) 
```




<hr>



### function SetPerspectiveVerticalFOV 

```C++
inline void AGE::SceneCamera::SetPerspectiveVerticalFOV (
    float VerticalFOV
) 
```




<hr>



### function SetProjectionType 

```C++
inline virtual void AGE::SceneCamera::SetProjectionType (
    ProjectionType Type
) override
```



Implements [*AGE::Camera::SetProjectionType*](class_a_g_e_1_1_camera.md#function-setprojectiontype)


<hr>



### function SetViewportSize 

```C++
void AGE::SceneCamera::SetViewportSize (
    uint32_t Width,
    uint32_t Height
) 
```




<hr>



### function ~SceneCamera 

```C++
virtual AGE::SceneCamera::~SceneCamera () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/SceneCamera.h`

