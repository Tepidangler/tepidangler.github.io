

# Class AGE::VerticalBoxComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md)








Inherits the following classes: [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)
























## Public Attributes inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) | [**m\_CompProperties**](class_a_g_e_1_1_u_i_component.md#variable-m_compproperties)  <br> |
|  std::string | [**m\_Name**](class_a_g_e_1_1_u_i_component.md#variable-m_name)   = `""`<br> |






























## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) override<br>_This function is used to deserialize data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object. It reads an object of type_[_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _using the provided serializer._ |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) override<br>_This function serializes the_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _object._ |
| virtual void | [**DrawContent**](#function-drawcontent) () override<br>_Draw the content of this component in a vertical layout._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) override<br>_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _by updating the component's state accordingly._ |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_This function updates the component based on a time step._  |
|   | [**VerticalBoxComponent**](#function-verticalboxcomponent) (const std::string & Name) <br>_Constructs a_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _with the given name._ |


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






## Public Functions Documentation




### function CallDeserialize 

_This function is used to deserialize data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object. It reads an object of type_[_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _using the provided serializer._
```C++
inline virtual void AGE::VerticalBoxComponent::CallDeserialize (
    DataReader * Serializer
) override
```





**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that will be used for deserialization.

This function is used to deserialize data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object. It reads an object of type [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) into the current instance of the class.




**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains the serialized data. 




        
Implements [*AGE::UIComponent::CallDeserialize*](class_a_g_e_1_1_u_i_component.md#function-calldeserialize)


<hr>



### function CallSerialize 

_This function serializes the_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _object._
```C++
inline virtual void AGE::VerticalBoxComponent::CallSerialize (
    DataWriter * Serializer
) override
```



The function writes the current state of the [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) object to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance, which can be used for further processing or storage.




**Parameters:**


* `Serializer` A pointer to the [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance that will handle the serialization process.



**Returns:**

void No return value is expected as this function only writes data and does not return any result.


This function is used to serialize the [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) object.




**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object, which provides methods for writing data.



**Returns:**

None 





        
Implements [*AGE::UIComponent::CallSerialize*](class_a_g_e_1_1_u_i_component.md#function-callserialize)


<hr>



### function DrawContent 

_Draw the content of this component in a vertical layout._ 
```C++
virtual void AGE::VerticalBoxComponent::DrawContent () override
```



This function is responsible for drawing the content of the component in a vertical layout, which means that it will draw all its child components one after another vertically. It does not handle any specific styling or positioning of these child components. These are handled by their respective Draw methods.




**Returns:**

void


Draw the content of this component in a vertical layout.


This function draws the content of this component in a vertical layout, which means that all child components are drawn one after another vertically. The exact behavior depends on the specific implementation of the [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) class and its subclasses.




**Returns:**

void 





        
Implements [*AGE::UIComponent::DrawContent*](class_a_g_e_1_1_u_i_component.md#function-drawcontent)


<hr>



### function OnEvent 

_Handles an event of type_ [_**Event**_](class_a_g_e_1_1_event.md) _by updating the component's state accordingly._
```C++
virtual void AGE::VerticalBoxComponent::OnEvent (
    Event & Event
) override
```



This function takes in a reference to an [**Event**](class_a_g_e_1_1_event.md) object and processes it based on its type. The exact behavior depends on the specific implementation of this class, which is not specified here.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) A reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs to be processed.

Handles an event of type [**Event**](class_a_g_e_1_1_event.md).


This function is responsible for processing the incoming events and updating the state of the [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) accordingly.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event to be processed. 




        
Implements [*AGE::UIComponent::OnEvent*](class_a_g_e_1_1_u_i_component.md#function-onevent)


<hr>



### function OnUpdate 

_This function updates the component based on a time step._ 
```C++
virtual void AGE::VerticalBoxComponent::OnUpdate (
    TimeStep DeltaTime
) override
```



The function first calls the base class's [**OnUpdate()**](class_a_g_e_1_1_vertical_box_component.md#function-onupdate) method with the provided delta time, which allows for any necessary cleanup or other tasks to be performed before the update process begins. It then continues with its own specific update logic.




**Parameters:**


* `DeltaTime` - A [**TimeStep**](class_a_g_e_1_1_time_step.md) object representing the amount of time that has passed since the last frame.

This function updates the component based on a time step.


The function first calls the OnUpdate method of its base class, [**UIComponent**](class_a_g_e_1_1_u_i_component.md), to handle any general updates that might be necessary. Then it performs any specific updates related to this [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) itself.




**Parameters:**


* `DeltaTime` The amount of time that has passed since the last update. 




        
Implements [*AGE::UIComponent::OnUpdate*](class_a_g_e_1_1_u_i_component.md#function-onupdate)


<hr>



### function VerticalBoxComponent 

_Constructs a_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _with the given name._
```C++
AGE::VerticalBoxComponent::VerticalBoxComponent (
    const std::string & Name
) 
```



This function initializes a new instance of [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) with the provided name and sets its type to VerticalBoxComponentType.




**Parameters:**


* `Name` The name for this component.

Constructs a [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) with the given name.


This constructor initializes the component's name and type to represent a vertical box component. The name of the component is set by the parameter 'Name'.




**Parameters:**


* `Name` A string representing the name of the component. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Components/Public/VerticalBoxComponent.h`

