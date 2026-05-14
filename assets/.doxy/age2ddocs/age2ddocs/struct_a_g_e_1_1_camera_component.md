

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
|  void | [**Activate**](#function-activate) () <br>_This function is used to activate the object by setting its primary flag to true._  |
|   | [**CameraComponent**](#function-cameracomponent-12) () = default<br>_Default constructor for the_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _class._ |
|   | [**CameraComponent**](#function-cameracomponent-22) (const [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) &) = default<br>_Default copy constructor for the_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _class._ |
|  void | [**Deactivate**](#function-deactivate) () <br>_This function deactivates the object by setting bPrimary to false._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) & Data) <br>_This function deserializes a_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _object from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _instance._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) & Data) <br>_This function serializes a camera component into a data writer object._  |


























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

_This function is used to activate the object by setting its primary flag to true._ 
```C++
inline void AGE::CameraComponent::Activate () 
```





**Returns:**

void 





        

<hr>



### function CameraComponent [1/2]

_Default constructor for the_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _class._
```C++
AGE::CameraComponent::CameraComponent () = default
```




<hr>



### function CameraComponent [2/2]

_Default copy constructor for the_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _class._
```C++
AGE::CameraComponent::CameraComponent (
    const CameraComponent &
) = default
```



This function is used to create a new instance of the [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) class by copying an existing one. It uses the '= default' syntax, which tells the compiler to use its default implementation for this member function.




**Parameters:**


* `other` The [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) object to be copied. 




        

<hr>



### function Deactivate 

_This function deactivates the object by setting bPrimary to false._ 
```C++
inline void AGE::CameraComponent::Deactivate () 
```





**Returns:**

void 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_This function deserializes a_ [_**CameraComponent**_](struct_a_g_e_1_1_camera_component.md) _object from the provided_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _instance._
```C++
static inline void AGE::CameraComponent::Deserialize (
    DataReader * Serializer,
    CameraComponent & Data
) 
```



The function reads data from the serialized format and populates the [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) reference with the corresponding values.




**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides the serialized data. 
* `Data` Reference to a [**CameraComponent**](struct_a_g_e_1_1_camera_component.md) object where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes a camera component into a data writer object._ 
```C++
static inline void AGE::CameraComponent::Serialize (
    DataWriter * Serializer,
    const CameraComponent & Data
) 
```





**Parameters:**


* `Serializer` A pointer to the data writer object where the data will be written. 
* `Data` The camera component that needs to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Scene/Public/Components.h`

