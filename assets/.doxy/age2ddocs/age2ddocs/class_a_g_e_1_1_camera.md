

# Class AGE::Camera



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Camera**](class_a_g_e_1_1_camera.md)










Inherited by the following classes: [AGE::EditorCamera](class_a_g_e_1_1_editor_camera.md),  [AGE::SceneCamera](class_a_g_e_1_1_scene_camera.md)
















## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br>_Default constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._ |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |
|  COMMENT | [**\_\_pad2\_\_**](#variable-__pad2__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Camera**](#function-camera-13) () = default<br> |
|   | [**Camera**](#function-camera-23) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) Projection) <br> |
|   | [**Camera**](#function-camera-33) ([**Vector4**](struct_a_g_e_1_1_vector4.md) Eye, [**Vector4**](struct_a_g_e_1_1_vector4.md) At, [**Vector4**](struct_a_g_e_1_1_vector4.md) Up) <br>_Constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class that initializes a camera with an eye position, at position and up direction._ |
|  const [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](#function-getconstantbufferdata-12) () const<br>_This function returns the constant buffer data._  |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**GetConstantBufferData**](#function-getconstantbufferdata-22) () <br>_This function returns the constant buffer data._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](#function-getprojection-12) () const<br>_Returns the projection matrix used for rendering._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & | [**GetProjection**](#function-getprojection-22) () <br>_Returns the projection matrix of the camera._  |
|  ProjectionType | [**GetProjectionType**](#function-getprojectiontype) () const<br>_Returns the projection type of this object._  |
|  const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](#function-getworldmatrix-12) () const<br>_Returns the world matrix of the object._  |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**GetWorldMatrix**](#function-getworldmatrix-22) () <br>_Returns the world matrix of the object._  |
| virtual void | [**SetProjectionType**](#function-setprojectiontype) (ProjectionType Type) <br>_Sets the projection type of the object._  |
| virtual  | [**~Camera**](#function-camera) () <br>_Virtual destructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._ |








## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**ConstantBufferStruct**](struct_a_g_e_1_1__constant_buffer_struct.md) | [**m\_ConstantBuffer**](#variable-m_constantbuffer)  <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_Projection**](#variable-m_projection)   = `{ 1.f }`<br> |
|  ProjectionType | [**m\_ProjectionType**](#variable-m_projectiontype)   = `ProjectionType::Orthographic`<br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**m\_World**](#variable-m_world)   = `{ 1.f }`<br> |




















## Public Attributes Documentation




### variable \_\_pad0\_\_ 

_Default constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._
```C++
COMMENT AGE::Camera::__pad0__;
```



This function initializes a new instance of the [**Camera**](class_a_g_e_1_1_camera.md) class with default values. It does not take any parameters and returns nothing. 


        

<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::Camera::__pad1__;
```




<hr>



### variable \_\_pad2\_\_ 

```C++
COMMENT AGE::Camera::__pad2__;
```




<hr>
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

_Constructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class that initializes a camera with an eye position, at position and up direction._
```C++
inline AGE::Camera::Camera (
    Vector4 Eye,
    Vector4 At,
    Vector4 Up
) 
```





**Parameters:**


* `Eye` The eye position of the camera as a [**Vector4**](struct_a_g_e_1_1_vector4.md) object. 
* `At` The at position of the camera as a [**Vector4**](struct_a_g_e_1_1_vector4.md) object. This is usually the point in 3D space that the camera is looking at. 
* `Up` The up direction of the camera as a [**Vector4**](struct_a_g_e_1_1_vector4.md) object. This defines the orientation of the camera.

Constructor for the [**Camera**](class_a_g_e_1_1_camera.md) class. 

**Parameters:**


* `Eye` A [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the eye position in world space coordinates. 
* `At` A [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the point at which to look in world space coordinates. 
* `Up` A [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the up direction in world space coordinates. 




        

<hr>



### function GetConstantBufferData [1/2]

_This function returns the constant buffer data._ 
```C++
inline const ConstantBufferStruct AGE::Camera::GetConstantBufferData () const
```





**Returns:**

A struct of type ConstantBufferStruct containing the constant buffer data.


Retrieves the constant buffer data.


This function returns a copy of the constant buffer data stored in the object. The returned data is a struct that contains all the necessary information for rendering.




**Returns:**

A ConstantBufferStruct containing the constant buffer data. 





        

<hr>



### function GetConstantBufferData [2/2]

_This function returns the constant buffer data._ 
```C++
inline ConstantBufferStruct AGE::Camera::GetConstantBufferData () 
```





**Returns:**

ConstantBufferStruct object containing the constant buffer data.


This function returns the constant buffer data. 

**Returns:**

ConstantBufferStruct object containing the constant buffer data. 





        

<hr>



### function GetProjection [1/2]

_Returns the projection matrix used for rendering._ 
```C++
inline const Matrix4D & AGE::Camera::GetProjection () const
```





**Returns:**

A constant reference to the projection matrix (m\_Projection).


Returns the projection matrix used for rendering. 

**Returns:**

A constant reference to the projection matrix (m\_Projection). 





        

<hr>



### function GetProjection [2/2]

_Returns the projection matrix of the camera._ 
```C++
inline Matrix4D & AGE::Camera::GetProjection () 
```



This function returns a reference to the projection matrix used by the camera for rendering. The returned object can be modified directly, which will affect all subsequent calls to this method and any other methods that use the same projection matrix.




**Returns:**

A reference to the projection matrix.


Returns the projection matrix of the camera. 

**Returns:**

A reference to the projection matrix (m\_Projection). 





        

<hr>



### function GetProjectionType 

_Returns the projection type of this object._ 
```C++
inline ProjectionType AGE::Camera::GetProjectionType () const
```





**Returns:**

The ProjectionType of this object. Possible values are defined in an enumeration.


Returns the projection type of the camera. 

**Returns:**

ProjectionType - The current projection type (ORTHOGRAPHIC, PERSPECTIVE). 





        

<hr>



### function GetWorldMatrix [1/2]

_Returns the world matrix of the object._ 
```C++
inline const Matrix4D AGE::Camera::GetWorldMatrix () const
```



This function returns the current world transformation matrix of the object. It is used to transform the object's vertices from local space to world space.




**Returns:**

The 4x4 world matrix as a [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) object.


Returns the world matrix of the object.


This function returns the current world matrix of the object, which is used for transformations and other calculations in the scene.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The current world matrix of the object. 





        

<hr>



### function GetWorldMatrix [2/2]

_Returns the world matrix of the object._ 
```C++
inline Matrix4D AGE::Camera::GetWorldMatrix () 
```



This function returns the current world matrix of the object, which is used for transformations and other calculations in the scene.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The current world matrix of the object.


Returns the world matrix of the object.


This function returns the current world matrix of the object, which is used for transformations and other calculations in the scene.




**Returns:**

[**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) The current world matrix of the object. 





        

<hr>



### function SetProjectionType 

_Sets the projection type of the object._ 
```C++
inline virtual void AGE::Camera::SetProjectionType (
    ProjectionType Type
) 
```





**Parameters:**


* `Type` The ProjectionType to be set. 



**Returns:**

None


Sets the projection type of the object. 

**Parameters:**


* `Type` The ProjectionType to be set. 




        

<hr>



### function ~Camera 

_Virtual destructor for the_ [_**Camera**_](class_a_g_e_1_1_camera.md) _class._
```C++
inline virtual AGE::Camera::~Camera () 
```



This function is a virtual destructor that cleans up any resources used by an instance of the [**Camera**](class_a_g_e_1_1_camera.md) class. It does not take any parameters and returns nothing.


Virtual destructor for the [**Camera**](class_a_g_e_1_1_camera.md) class.


This function is a virtual destructor that cleans up any resources used by an instance of the [**Camera**](class_a_g_e_1_1_camera.md) class. It does not take any parameters and returns no value. 


        

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

