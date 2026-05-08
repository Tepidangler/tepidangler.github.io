

# Class AGE::Camera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Camera**](class_a_g_e_1_1_camera.md)










Inherited by the following classes: [AGE::EditorCamera](class_a_g_e_1_1_editor_camera.md),  [AGE::SceneCamera](class_a_g_e_1_1_scene_camera.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Camera**](#function-camera-13) () = default<br> |
|   | [**Camera**](#function-camera-23) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Projection) <br> |
|   | [**Camera**](#function-camera-33) ([**Vector4**](struct_a_g_e_1_1_vector4.md) Eye, [**Vector4**](struct_a_g_e_1_1_vector4.md) At, [**Vector4**](struct_a_g_e_1_1_vector4.md) Up) <br> |
|  const [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](#function-getconstantbufferdata-12) () const<br> |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](#function-getconstantbufferdata-22) () <br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](#function-getprojection-12) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](#function-getprojection-22) () <br> |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br> |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](#function-getworldmatrix-12) () const<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](#function-getworldmatrix-22) () <br> |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) <br> |
| virtual  | [**~Camera**](#function-camera) () <br> |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**m\_ConstantBuffer**](#variable-m_constantbuffer)  <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_Projection**](#variable-m_projection)   = `{ 1.f }`<br> |
|  ProjectionType | [**m\_ProjectionType**](#variable-m_projectiontype)   = `ProjectionType::Orthographic`<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_World**](#variable-m_world)   = `{ 1.f }`<br> |




















## Public Functions Documentation




### function Camera [1/3]

```C++
AGE::Camera::Camera () = default
```




<hr>



### function Camera [2/3]

```C++
inline AGE::Camera::Camera (
    Matrix4D Projection
) 
```




<hr>



### function Camera [3/3]

```C++
inline AGE::Camera::Camera (
    Vector4 Eye,
    Vector4 At,
    Vector4 Up
) 
```




<hr>



### function GetConstantBufferData [1/2]

```C++
inline const ConstantBufferStruct AGE::Camera::GetConstantBufferData () const
```




<hr>



### function GetConstantBufferData [2/2]

```C++
inline ConstantBufferStruct AGE::Camera::GetConstantBufferData () 
```




<hr>



### function GetProjection [1/2]

```C++
inline const Matrix4D & AGE::Camera::GetProjection () const
```




<hr>



### function GetProjection [2/2]

```C++
inline Matrix4D & AGE::Camera::GetProjection () 
```




<hr>



### function GetProjectionType 

```C++
inline ProjectionType AGE::Camera::GetProjectionType () const
```




<hr>



### function GetWorldMatrix [1/2]

```C++
inline const Matrix4D AGE::Camera::GetWorldMatrix () const
```




<hr>



### function GetWorldMatrix [2/2]

```C++
inline Matrix4D AGE::Camera::GetWorldMatrix () 
```




<hr>



### function SetProjectionType 

```C++
inline virtual void AGE::Camera::SetProjectionType (
    ProjectionType Type
) 
```




<hr>



### function ~Camera 

```C++
inline virtual AGE::Camera::~Camera () 
```




<hr>
## Protected Attributes Documentation




### variable m\_ConstantBuffer 

```C++
ConstantBufferStruct AGE::Camera::m_ConstantBuffer;
```




<hr>



### variable m\_Projection 

```C++
Matrix4D AGE::Camera::m_Projection;
```




<hr>



### variable m\_ProjectionType 

```C++
ProjectionType AGE::Camera::m_ProjectionType;
```




<hr>



### variable m\_World 

```C++
Matrix4D AGE::Camera::m_World;
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Camera/Public/Camera.h`

