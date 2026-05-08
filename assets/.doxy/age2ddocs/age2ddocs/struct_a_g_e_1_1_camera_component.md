

# Struct AGE::CameraComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**CameraComponent**](struct_a_g_e_1_1_camera_component.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**SceneCamera**](class_a_g_e_1_1_scene_camera.md) | [**Cam**](#variable-cam)  <br> |
|  bool | [**bFixedAspectRatio**](#variable-bfixedaspectratio)   = `false`<br> |
|  bool | [**bPrimary**](#variable-bprimary)   = `true`<br> |
|  bool | [**bRecording**](#variable-brecording)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Activate**](#function-activate) () <br> |
|   | [**CameraComponent**](#function-cameracomponent-12) () = default<br> |
|   | [**CameraComponent**](#function-cameracomponent-22) (const [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) &) = default<br> |
|  void | [**Deactivate**](#function-deactivate) () <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) & Data) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) & Data) <br> |


























## Public Attributes Documentation




### variable Cam 

```C++
SceneCamera AGE::CameraComponent::Cam;
```




<hr>



### variable bFixedAspectRatio 

```C++
bool AGE::CameraComponent::bFixedAspectRatio;
```




<hr>



### variable bPrimary 

```C++
bool AGE::CameraComponent::bPrimary;
```




<hr>



### variable bRecording 

```C++
bool AGE::CameraComponent::bRecording;
```




<hr>
## Public Functions Documentation




### function Activate 

```C++
inline void AGE::CameraComponent::Activate () 
```




<hr>



### function CameraComponent [1/2]

```C++
AGE::CameraComponent::CameraComponent () = default
```




<hr>



### function CameraComponent [2/2]

```C++
AGE::CameraComponent::CameraComponent (
    const CameraComponent &
) = default
```




<hr>



### function Deactivate 

```C++
inline void AGE::CameraComponent::Deactivate () 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

```C++
static inline void AGE::CameraComponent::Deserialize (
    DataReader * Serializer,
    CameraComponent & Data
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::CameraComponent::Serialize (
    DataWriter * Serializer,
    const CameraComponent & Data
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

