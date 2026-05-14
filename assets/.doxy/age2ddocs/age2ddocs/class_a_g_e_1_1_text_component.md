

# Class AGE::TextComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**TextComponent**](class_a_g_e_1_1_text_component.md)








Inherits the following classes: [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)






















## Public Attributes

| Type | Name |
| ---: | :--- |
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
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) override<br>_Deserializes the_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) override<br>_This function serializes the_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _object using a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |
| virtual void | [**DrawContent**](#function-drawcontent) () override<br>_Draws a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _with various properties._ |
| virtual void | [**DrawFontSelectionComboBox**](#function-drawfontselectioncombobox) () override<br>_Draws a combo box for selecting the font._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) override<br>_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._ |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_This function updates the text component based on a time step._  |
|   | [**TextComponent**](#function-textcomponent) (const std::string & Name) <br> |


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
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**TextComponent**](class_a_g_e_1_1_text_component.md) & Instance) <br>_Deserialize function for_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**TextComponent**](class_a_g_e_1_1_text_component.md) & Instance) <br>_This function serializes a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


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




### variable m\_StringProperties 

```C++
StringProperties AGE::TextComponent::m_StringProperties;
```




<hr>
## Public Functions Documentation




### function CallDeserialize 

_Deserializes the_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
inline virtual void AGE::TextComponent::CallDeserialize (
    DataReader * Serializer
) override
```



This function reads an instance of [**TextComponent**](class_a_g_e_1_1_text_component.md) from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and assigns it to this object. The exact format in which the data is read depends on how the [**DataReader**](class_a_g_e_1_1_data_reader.md)'s ReadObject method is implemented.




**Parameters:**


* `Serializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data.

Deserializes the [**TextComponent**](class_a_g_e_1_1_text_component.md) from a [**DataReader**](class_a_g_e_1_1_data_reader.md).


This function reads an object of type [**TextComponent**](class_a_g_e_1_1_text_component.md) from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and assigns it to this instance. The exact nature of deserialization is determined by the specific implementation of the [**DataReader**](class_a_g_e_1_1_data_reader.md) class.




**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) that provides the serialized data. 




        
Implements [*AGE::UIComponent::CallDeserialize*](class_a_g_e_1_1_u_i_component.md#function-calldeserialize)


<hr>



### function CallSerialize 

_This function serializes the_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _object using a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
inline virtual void AGE::TextComponent::CallSerialize (
    DataWriter * Serializer
) override
```



The function writes the current instance of the [**TextComponent**](class_a_g_e_1_1_text_component.md) to the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md), which can be used for further processing or storage.




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will handle the writing operation.



**Returns:**

void No return value is expected as this function directly writes data using the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md).


This function serializes the [**TextComponent**](class_a_g_e_1_1_text_component.md) object using a [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that is used for writing data.



**Returns:**

void 





        
Implements [*AGE::UIComponent::CallSerialize*](class_a_g_e_1_1_u_i_component.md#function-callserialize)


<hr>



### function DrawContent 

_Draws a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _with various properties._
```C++
virtual void AGE::TextComponent::DrawContent () override
```



The function displays an interface for editing the text, font size, color, position, and rotation of a [**TextComponent**](class_a_g_e_1_1_text_component.md). It uses ImGui functions to create input fields for these properties.




**Returns:**

void


Draws the content of a [**TextComponent**](class_a_g_e_1_1_text_component.md), including text input fields for properties like Font Name, Font Size and Color, as well as position and rotation controls.


The function first displays "String Properties" using ImGui::Text(). Then it creates an input field for "Text", uses ImGui::InputText() to handle user input. It also includes a combo box for font selection with [**DrawFontSelectionComboBox()**](class_a_g_e_1_1_text_component.md#function-drawfontselectioncombobox). If the selected font's atlas texture name does not match m\_StringProperties.FontName, it updates m\_StringProperties.TextFont accordingly using [**AssetManager::Get()**](class_a_g_e_1_1_asset_manager.md#function-get).GetFont(m\_StringProperties.FontName). It then creates an input field for "Font Size" and a color picker for "Text Color", both handled by ImGui functions respectively. Finally, it draws position and rotation controls with [**DrawVec3Control()**](class_a_g_e_1_1_u_i_component.md#function-drawvec3control) function.




**Returns:**

void 





        
Implements [*AGE::UIComponent::DrawContent*](class_a_g_e_1_1_u_i_component.md#function-drawcontent)


<hr>



### function DrawFontSelectionComboBox 

_Draws a combo box for selecting the font._ 
```C++
virtual void AGE::TextComponent::DrawFontSelectionComboBox () override
```



This function populates a ComboBox with all available fonts from the [**AssetManager**](class_a_g_e_1_1_asset_manager.md). The currently selected font is stored in m\_StringProperties.FontName, which is updated whenever a new font is selected. If no font is currently selected (i.e., m\_StringProperties.FontName is empty), the default font is used as the initial selection.




**Returns:**

void 





        
Implements [*AGE::UIComponent::DrawFontSelectionComboBox*](class_a_g_e_1_1_u_i_component.md#function-drawfontselectioncombobox)


<hr>



### function OnEvent 

_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _._
```C++
virtual void AGE::TextComponent::OnEvent (
    Event & Event
) override
```



This function takes in a reference to an object of type [**Event**](class_a_g_e_1_1_event.md) and processes it accordingly. The exact behavior depends on the specifics of the implementation.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - Reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs processing.

Handles an event of type [**Event**](class_a_g_e_1_1_event.md).


This function takes in a reference to an [**Event**](class_a_g_e_1_1_event.md) object and processes it accordingly. The exact behavior depends on the specifics of the [**Event**](class_a_g_e_1_1_event.md) subclass that is being processed.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - Reference to the [**Event**](class_a_g_e_1_1_event.md) object to be handled. 




        
Implements [*AGE::UIComponent::OnEvent*](class_a_g_e_1_1_u_i_component.md#function-onevent)


<hr>



### function OnUpdate 

_This function updates the text component based on a time step._ 
```C++
virtual void AGE::TextComponent::OnUpdate (
    TimeStep DeltaTime
) override
```



The function checks if the component is visible and if so, it calls Renderer2D::DrawString with the string properties of the component. It's assumed that Renderer2D::DrawString takes care of rendering the string in the correct position on screen.




**Parameters:**


* `DeltaTime` The time step since the last update. This is used to calculate how much time has passed and adjust the animation accordingly.

This function updates the text component based on a time step.


The function checks if the component is visible and then calls [**Renderer2D**](class_a_g_e_1_1_renderer2_d.md)'s DrawString method with m\_StringProperties as an argument. If the component is not visible, no action will be taken.




**Parameters:**


* `DeltaTime` The time step for updating the component. 




        
Implements [*AGE::UIComponent::OnUpdate*](class_a_g_e_1_1_u_i_component.md#function-onupdate)


<hr>



### function TextComponent 

```C++
AGE::TextComponent::TextComponent (
    const std::string & Name
) 
```




<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize function for_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _._
```C++
static inline void AGE::TextComponent::Deserialize (
    DataReader * Serializer,
    TextComponent & Instance
) 
```



This function reads data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object and populates the [**TextComponent**](class_a_g_e_1_1_text_component.md) instance with it. It reads the name of the component, its type, text properties (text, font name, color, font size), and position and rotation values.




**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that provides serialized data. 
* `Instance` Reference to the [**TextComponent**](class_a_g_e_1_1_text_component.md) instance where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::TextComponent::Serialize (
    DataWriter * Serializer,
    const TextComponent & Instance
) 
```



The function writes several properties of the [**TextComponent**](class_a_g_e_1_1_text_component.md) to the [**DataWriter**](class_a_g_e_1_1_data_writer.md), including its name, type, string properties (text, font name), color, font size, and position/rotation.




**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance that will be used for serialization. 
* `Instance` The [**TextComponent**](class_a_g_e_1_1_text_component.md) instance to be serialized.

This function serializes a [**TextComponent**](class_a_g_e_1_1_text_component.md) instance into the provided [**DataWriter**](class_a_g_e_1_1_data_writer.md).




**Parameters:**


* `Serializer` Pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will be used for writing data. 
* `Instance` The [**TextComponent**](class_a_g_e_1_1_text_component.md) instance to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Components/Public/TextComponent.h`

