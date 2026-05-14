

# Class AGE::TextBoxComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md)








Inherits the following classes: [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**BoxProperties**](struct_a_g_e_1_1_box_properties.md) | [**m\_BoxProperties**](#variable-m_boxproperties)  <br> |
|  [**StringProperties**](struct_a_g_e_1_1_string_properties.md) | [**m\_StringProperties**](#variable-m_stringproperties)  <br> |


## Public Attributes inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) | [**m\_CompProperties**](class_a_g_e_1_1_u_i_component.md#variable-m_compproperties)  <br> |
|  std::string | [**m\_Name**](class_a_g_e_1_1_u_i_component.md#variable-m_name)   = `""`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) override<br>_Deserializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) override<br>_This function serializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _object using a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |
| virtual void | [**DrawContent**](#function-drawcontent) () override<br>_Draws the content of the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _, including text properties, font selection, color editing, and positioning controls._ |
| virtual void | [**DrawFontSelectionComboBox**](#function-drawfontselectioncombobox) () override<br>_This function is responsible for drawing the font selection combo box on the screen._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) override<br>_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._ |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_Updates the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _based on a time step._ |
|   | [**TextBoxComponent**](#function-textboxcomponent) (const std::string & Name) <br>_Constructs a_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _with the given name and sets default properties._ |


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


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) & Instance) <br>_Deserializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _instance from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) & Instance) <br>_Serializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _instance into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |


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




### variable m\_BoxProperties 

```C++
BoxProperties AGE::TextBoxComponent::m_BoxProperties;
```




<hr>



### variable m\_StringProperties 

```C++
StringProperties AGE::TextBoxComponent::m_StringProperties;
```




<hr>
## Public Functions Documentation




### function CallDeserialize 

_Deserializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
inline virtual void AGE::TextBoxComponent::CallDeserialize (
    DataReader * Serializer
) override
```



This function reads an instance of [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and assigns it to this object. The exact format in which the data is read depends on how the [**DataReader**](class_a_g_e_1_1_data_reader.md)'s ReadObject method is implemented.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data.

This function is used to deserialize a [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md).




**Parameters:**


* `Serializer` A pointer to an instance of [**DataReader**](class_a_g_e_1_1_data_reader.md), which provides the serialized data. 



**Returns:**

void No return value as it directly modifies the state of the current object ([**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md)). 





        
Implements [*AGE::UIComponent::CallDeserialize*](class_a_g_e_1_1_u_i_component.md#function-calldeserialize)


<hr>



### function CallSerialize 

_This function serializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _object using a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
inline virtual void AGE::TextBoxComponent::CallSerialize (
    DataWriter * Serializer
) override
```





**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that is used for writing data.

This function serializes the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance where the object will be written. 




        
Implements [*AGE::UIComponent::CallSerialize*](class_a_g_e_1_1_u_i_component.md#function-callserialize)


<hr>



### function DrawContent 

_Draws the content of the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _, including text properties, font selection, color editing, and positioning controls._
```C++
virtual void AGE::TextBoxComponent::DrawContent () override
```



This function uses ImGui to draw a series of UI elements for configuring the text properties of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md). It includes inputs for text string, font selection, color editing, and positioning controls. The function updates the m\_StringProperties member variable accordingly based on user input.




**Returns:**

void 





        
Implements [*AGE::UIComponent::DrawContent*](class_a_g_e_1_1_u_i_component.md#function-drawcontent)


<hr>



### function DrawFontSelectionComboBox 

_This function is responsible for drawing the font selection combo box on the screen._ 
```C++
virtual void AGE::TextBoxComponent::DrawFontSelectionComboBox () override
```





**Returns:**

None


This function is responsible for drawing the font selection combo box on the screen.


The function does not take any parameters and returns no value. It directly interacts with the UI to display the font selection combo box. 


        
Implements [*AGE::UIComponent::DrawFontSelectionComboBox*](class_a_g_e_1_1_u_i_component.md#function-drawfontselectioncombobox)


<hr>



### function OnEvent 

_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._
```C++
virtual void AGE::TextBoxComponent::OnEvent (
    Event & Event
) override
```



This function takes in a reference to an [**Event**](class_a_g_e_1_1_event.md) object and processes it according to its type. The exact behavior depends on the specific implementation of this class.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - A reference to the [**Event**](class_a_g_e_1_1_event.md) that needs to be processed.

Handles an event of type [**Event**](class_a_g_e_1_1_event.md).


This function takes in a reference to an [**Event**](class_a_g_e_1_1_event.md) object and processes it according to its type. The exact behavior depends on the specific implementation of this class, which is not specified here.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) A reference to the [**Event**](class_a_g_e_1_1_event.md) that needs to be processed. 




        
Implements [*AGE::UIComponent::OnEvent*](class_a_g_e_1_1_u_i_component.md#function-onevent)


<hr>



### function OnUpdate 

_Updates the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _based on a time step._
```C++
virtual void AGE::TextBoxComponent::OnUpdate (
    TimeStep DeltaTime
) override
```



This function updates the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) by checking if it is visible. If it is, it sets up properties for a quad and string to be drawn. The quad's transform, color, and other properties are set according to the component's box properties. Then, it calls [**Renderer2D::DrawQuad**](class_a_g_e_1_1_renderer2_d.md#function-drawquad-13) with these properties and Renderer2D::DrawString with the string properties of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md).




**Parameters:**


* `DeltaTime` The time step for updating the component.

Updates the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) based on the provided [**TimeStep**](class_a_g_e_1_1_time_step.md).


This function updates the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) by checking if it is visible. If it is, it creates a [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object and sets its properties such as Transform, Color etc., then calls [**Renderer2D::DrawQuad()**](class_a_g_e_1_1_renderer2_d.md#function-drawquad-13) with this [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) to render the quad. It also renders a string using Renderer2D::DrawString().




**Parameters:**


* `DeltaTime` The time step for the update operation. 




        
Implements [*AGE::UIComponent::OnUpdate*](class_a_g_e_1_1_u_i_component.md#function-onupdate)


<hr>



### function TextBoxComponent 

_Constructs a_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _with the given name and sets default properties._
```C++
AGE::TextBoxComponent::TextBoxComponent (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The name of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md). 



**Returns:**

None


Constructs a [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) with the given name and sets default properties. 

**Parameters:**


* `Name` The name of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md). 




        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _instance from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object._
```C++
static inline void AGE::TextBoxComponent::Deserialize (
    DataReader * Serializer,
    TextBoxComponent & Instance
) 
```



This function reads various properties of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) instance, including its name, type, string properties (text, font name, color and size), and position and rotation data. It uses the provided Serializer to read these values.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides the serialized data. 
* `Instance` The [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) instance to be deserialized. 




        

<hr>



### function Serialize 

_Serializes the_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _instance into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::TextBoxComponent::Serialize (
    DataWriter * Serializer,
    const TextBoxComponent & Instance
) 
```



This function writes various properties of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md), including its name, type, string properties (text, font name, color and size), and position and rotation data.




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance where serialization will be performed. 
* `Instance` The [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) instance that needs to be serialized.



**Returns:**

void


This function serializes the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) instance into a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object.


The function writes various properties of the [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), such as its name, type, string properties (text, font name, color and size), and position and rotation data.




**Parameters:**


* `Serializer` Pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where serialized data will be written into. 
* `Instance` The [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) instance that needs to be serialized.



**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Components/Public/TextBoxComponent.h`

