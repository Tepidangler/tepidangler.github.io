

# Class AGE::UIImageComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md)








Inherits the following classes: [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::string | [**m\_CurrentTexture**](#variable-m_currenttexture)  <br> |
|  Ref&lt; [**Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; | [**m\_Image**](#variable-m_image)  <br> |
|  [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) | [**m\_Properties**](#variable-m_properties)   = `{}`<br> |
|  std::vector&lt; std::string &gt; | [**m\_TextureNames**](#variable-m_texturenames)  <br> |


## Public Attributes inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) | [**m\_CompProperties**](class_a_g_e_1_1_u_i_component.md#variable-m_compproperties)  <br> |
|  std::string | [**m\_Name**](class_a_g_e_1_1_u_i_component.md#variable-m_name)   = `""`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) override<br>_This function is used to call the deserialization process on a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._ |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) override<br>_This function is used to serialize data using a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |
| virtual void | [**DrawContent**](#function-drawcontent) () override<br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) override<br>_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._ |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_This function updates the image component._  |
|   | [**UIImageComponent**](#function-uiimagecomponent) (const std::string & Name) <br>_Constructs an instance of_ [_**UIImageComponent**_](class_a_g_e_1_1_u_i_image_component.md) _with the given name and initializes it._ |
| virtual  | [**~UIImageComponent**](#function-uiimagecomponent) () = default<br>_Virtual destructor for the_ [_**UIImageComponent**_](class_a_g_e_1_1_u_i_image_component.md) _class._ |


## Public Functions inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_u_i_component.md#function-as-13) () <br> |
|  [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) \* | [**As**](class_a_g_e_1_1_u_i_component.md#function-as-23) () <br>_This function is used to cast the current object to_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _type._ |
|  [**TextComponent**](class_a_g_e_1_1_text_component.md) \* | [**As**](class_a_g_e_1_1_u_i_component.md#function-as-33) () <br>_This function is used to cast the current object to a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _type._ |
| virtual void | [**CallDeserialize**](class_a_g_e_1_1_u_i_component.md#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) = 0<br> |
| virtual void | [**CallSerialize**](class_a_g_e_1_1_u_i_component.md#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) = 0<br> |
| virtual void | [**DrawContent**](class_a_g_e_1_1_u_i_component.md#function-drawcontent) () = 0<br> |
| virtual void | [**DrawFontSelectionComboBox**](class_a_g_e_1_1_u_i_component.md#function-drawfontselectioncombobox) () <br>_This function is responsible for drawing the font selection combo box on the screen._  |
|  std::string & | [**GetName**](class_a_g_e_1_1_u_i_component.md#function-getname) () <br>_Gets the name of the object._  |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) & | [**GetProperties**](class_a_g_e_1_1_u_i_component.md#function-getproperties) () <br>_Returns a reference to the UI properties object._  |
|  UIComponentType::Value | [**GetType**](class_a_g_e_1_1_u_i_component.md#function-gettype) () <br>_This function returns the type of the UI component._  |
| virtual void | [**OnEvent**](class_a_g_e_1_1_u_i_component.md#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) = 0<br>_Handles an event by dispatching it to the appropriate handler._  |
| virtual void | [**OnUpdate**](class_a_g_e_1_1_u_i_component.md#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|   | [**UIComponent**](class_a_g_e_1_1_u_i_component.md#function-uicomponent-12) (const std::string & Name) <br>_Constructs a_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _with the given name._ |
| virtual  | [**~UIComponent**](class_a_g_e_1_1_u_i_component.md#function-uicomponent) () = default<br>_Virtual destructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._ |




## Public Static Functions inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UIComponent**](class_a_g_e_1_1_u_i_component.md) &gt; | [**Create**](class_a_g_e_1_1_u_i_component.md#function-create) (const std::string & Name, [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) Type) <br>_Creates a new instance of a UI component based on the provided type._  |
|  void | [**DrawVec3Control**](class_a_g_e_1_1_u_i_component.md#function-drawvec3control) (const std::string & Label, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, float ResetValue=0.f, float ColumnWidth=100.f) <br>_Draws a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _control with draggable sliders._ |












## Protected Attributes inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) | [**m\_Type**](class_a_g_e_1_1_u_i_component.md#variable-m_type)   = `UIComponentType::TextComponent`<br> |
































## Protected Functions inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|   | [**UIComponent**](class_a_g_e_1_1_u_i_component.md#function-uicomponent-22) () = default<br>_Default constructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._ |






## Public Attributes Documentation




### variable m\_CurrentTexture 

```C++
std::string AGE::UIImageComponent::m_CurrentTexture;
```




<hr>



### variable m\_Image 

```C++
Ref<Texture2D> AGE::UIImageComponent::m_Image;
```




<hr>



### variable m\_Properties 

```C++
QuadProperties AGE::UIImageComponent::m_Properties;
```




<hr>



### variable m\_TextureNames 

```C++
std::vector<std::string> AGE::UIImageComponent::m_TextureNames;
```




<hr>
## Public Functions Documentation




### function CallDeserialize 

_This function is used to call the deserialization process on a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._
```C++
inline virtual void AGE::UIImageComponent::CallDeserialize (
    DataReader * Serializer
) override
```



The function takes in a pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object as its parameter. It does not return anything, so it's void type.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object that will be used for the deserialization process.

This function is used to call the deserialization process on a [**DataReader**](class_a_g_e_1_1_data_reader.md) object. The exact behavior of this function depends on its implementation in the derived class, as it's marked as 'override'.




**Parameters:**


* `Serializer` A pointer to an instance of [**DataReader**](class_a_g_e_1_1_data_reader.md) that will be used for deserialization. 




        
Implements [*AGE::UIComponent::CallDeserialize*](class_a_g_e_1_1_u_i_component.md#function-calldeserialize)


<hr>



### function CallSerialize 

_This function is used to serialize data using a_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
inline virtual void AGE::UIImageComponent::CallSerialize (
    DataWriter * Serializer
) override
```



The function takes in a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object as its parameter. It does not return anything, so the return type should be void.




**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will handle the serialization process.

This function is used to serialize data using a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object.


The function takes in one parameter, a pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object which is responsible for writing the serialized data. It does not return anything as it's an override of the base class method and doesn't need any post-processing after serialization.




**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be used to write the serialized data. 




        
Implements [*AGE::UIComponent::CallSerialize*](class_a_g_e_1_1_u_i_component.md#function-callserialize)


<hr>



### function DrawContent 

```C++
virtual void AGE::UIImageComponent::DrawContent () override
```



Implements [*AGE::UIComponent::DrawContent*](class_a_g_e_1_1_u_i_component.md#function-drawcontent)


<hr>



### function OnEvent 

_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._
```C++
virtual void AGE::UIImageComponent::OnEvent (
    Event & Event
) override
```



This function is responsible for handling events dispatched by the system. It takes in a reference to an [**Event**](class_a_g_e_1_1_event.md) object and processes it accordingly. The exact behavior depends on the specifics of the [**Event**](class_a_g_e_1_1_event.md) subclass that is being handled.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - A reference to the event to be processed.

This function is used to handle events in the [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md) class.


The function takes an [**Event**](class_a_g_e_1_1_event.md) object as a parameter and processes it according to its type.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - An instance of the [**Event**](class_a_g_e_1_1_event.md) class that represents the event to be processed.



**Returns:**

void 





        
Implements [*AGE::UIComponent::OnEvent*](class_a_g_e_1_1_u_i_component.md#function-onevent)


<hr>



### function OnUpdate 

_This function updates the image component._ 
```C++
virtual void AGE::UIImageComponent::OnUpdate (
    TimeStep DeltaTime
) override
```



The function takes a [**TimeStep**](class_a_g_e_1_1_time_step.md) parameter representing the time elapsed since the last frame. It uses this value to update the image and its properties.




**Parameters:**


* `DeltaTime` - A [**TimeStep**](class_a_g_e_1_1_time_step.md) object representing the time elapsed since the last frame.



**Returns:**

void


This function updates the image component.


The function takes in a [**TimeStep**](class_a_g_e_1_1_time_step.md) parameter representing the delta time since the last frame. It then uses this value to update the properties of the image component, such as its position or scale. Finally, it renders the updated image using [**Renderer2D::DrawQuad()**](class_a_g_e_1_1_renderer2_d.md#function-drawquad-13).




**Parameters:**


* `DeltaTime` The time elapsed since the last frame in seconds. 




        
Implements [*AGE::UIComponent::OnUpdate*](class_a_g_e_1_1_u_i_component.md#function-onupdate)


<hr>



### function UIImageComponent 

_Constructs an instance of_ [_**UIImageComponent**_](class_a_g_e_1_1_u_i_image_component.md) _with the given name and initializes it._
```C++
AGE::UIImageComponent::UIImageComponent (
    const std::string & Name
) 
```



This constructor creates a new [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md) with the provided name, sets its type to ImageComponent, retrieves all textures from the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s asset registry, stores their names in m\_TextureNames, and finally creates an instance of [**Texture2D**](class_a_g_e_1_1_texture2_d.md) using default parameters.




**Parameters:**


* `Name` The name for this [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md).

Constructs an instance of [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md) with the given name and initializes it with a default texture.


The constructor creates an unordered map of textures from the [**AssetManager**](class_a_g_e_1_1_asset_manager.md)'s asset registry using GetTextures() method. It then iterates over this map, pushing each texture's name into m\_TextureNames vector. Finally, it creates a new [**Texture2D**](class_a_g_e_1_1_texture2_d.md) instance with default specifications and assigns it to m\_Image.




**Parameters:**


* `Name` The name of the [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md) instance. 




        

<hr>



### function ~UIImageComponent 

_Virtual destructor for the_ [_**UIImageComponent**_](class_a_g_e_1_1_u_i_image_component.md) _class._
```C++
virtual AGE::UIImageComponent::~UIImageComponent () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not take any parameters and returns no value.


Virtual destructor for the [**UIImageComponent**](class_a_g_e_1_1_u_i_image_component.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Components/Public/UiImageComponent.h`

