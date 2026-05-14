

# Class AGE::ButtonComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ButtonComponent**](class_a_g_e_1_1_button_component.md)








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
|   | [**ButtonComponent**](#function-buttoncomponent) (const std::string & Name) <br>_Constructs a_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _with the given name._ |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) override<br>_This function is used to deserialize data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object. It reads an object of type_[_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _using the provided serializer._ |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) override<br>_This function is used to serialize the_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _object._ |
| virtual void | [**DrawContent**](#function-drawcontent) () override<br>_Draws the content of the_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _, including properties like position, rotation, scale and color._ |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) override<br>_This function handles events related to the button component. It dispatches different types of events based on the current state of the button and the event that has occurred._  |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_Updates the_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _based on the provided_[_**TimeStep**_](class_a_g_e_1_1_time_step.md) _._ |
|  void | [**SetOnClickFunc**](#function-setonclickfunc) (const std::function&lt; void()&gt; & func) <br>_Sets the on-click function for this object._  |


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






























## Protected Functions

| Type | Name |
| ---: | :--- |
|  bool | [**IsButtonHovered**](#function-isbuttonhovered) () <br>_Checks if the button is hovered by the mouse cursor._  |


## Protected Functions inherited from AGE::UIComponent

See [AGE::UIComponent](class_a_g_e_1_1_u_i_component.md)

| Type | Name |
| ---: | :--- |
|   | [**UIComponent**](class_a_g_e_1_1_u_i_component.md#function-uicomponent-22) () = default<br>_Default constructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._ |






## Public Functions Documentation




### function ButtonComponent 

_Constructs a_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _with the given name._
```C++
AGE::ButtonComponent::ButtonComponent (
    const std::string & Name
) 
```



This function initializes a new instance of the [**ButtonComponent**](class_a_g_e_1_1_button_component.md) class, setting its name and type. It also sets up an anonymous lambda function as the onClick event handler that logs "Button Clicked!" to the console when invoked. 

**Parameters:**


* `Name` The name for this button component.

Constructs a [**ButtonComponent**](class_a_g_e_1_1_button_component.md) with the given name.


This function initializes a new instance of the [**ButtonComponent**](class_a_g_e_1_1_button_component.md) class, setting its name and type. It also sets up an anonymous lambda function as the onClick event handler that logs "Button Clicked!" to the console when triggered. 

**Parameters:**


* `Name` The name for the button component. 




        

<hr>



### function CallDeserialize 

_This function is used to deserialize data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _object. It reads an object of type_[_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _using the provided serializer._
```C++
inline virtual void AGE::ButtonComponent::CallDeserialize (
    DataReader * Serializer
) override
```





**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that will be used for deserialization.

This function is used to deserialize data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) object. It reads an object of type [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) into the current instance of this class. 

**Parameters:**


* `Serializer` A pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) object that contains the serialized data. 



**Returns:**

None 





        
Implements [*AGE::UIComponent::CallDeserialize*](class_a_g_e_1_1_u_i_component.md#function-calldeserialize)


<hr>



### function CallSerialize 

_This function is used to serialize the_ [_**VerticalBoxComponent**_](class_a_g_e_1_1_vertical_box_component.md) _object._
```C++
inline virtual void AGE::ButtonComponent::CallSerialize (
    DataWriter * Serializer
) override
```





**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object, which provides methods for writing data. 



**Returns:**

void No return value expected.


This function serializes the [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md) object.


The function writes the data of this object into a [**DataWriter**](class_a_g_e_1_1_data_writer.md), which can be used for further processing or storage. It uses the WriteObject method to write the specific type ([**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md)) and the instance of this class (\*this).




**Parameters:**


* `Serializer` A pointer to an instance of [**DataWriter**](class_a_g_e_1_1_data_writer.md) that will handle the serialization process. 




        
Implements [*AGE::UIComponent::CallSerialize*](class_a_g_e_1_1_u_i_component.md#function-callserialize)


<hr>



### function DrawContent 

_Draws the content of the_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _, including properties like position, rotation, scale and color._
```C++
virtual void AGE::ButtonComponent::DrawContent () override
```



This function uses ImGui to draw a series of controls for modifying the [**BoxProperties**](struct_a_g_e_1_1_box_properties.md) of the [**ButtonComponent**](class_a_g_e_1_1_button_component.md). It includes fields for Screen Position, Screen Rotation, Screen Scale and Box Color. The [**DrawVec3Control**](class_a_g_e_1_1_u_i_component.md#function-drawvec3control) is used to handle [**Vector3**](struct_a_g_e_1_1_vector3.md) properties.




**Returns:**

void


Draws the content of the [**ButtonComponent**](class_a_g_e_1_1_button_component.md), including box properties like position, rotation, scale and color.


This function uses ImGui to draw text fields for each property, a vector control for editing position, rotation and scale vectors, and a color edit control for setting the tint color of the box. The `DrawVec3Control` function is used to handle the drawing and input of these properties.




**Returns:**

void 





        
Implements [*AGE::UIComponent::DrawContent*](class_a_g_e_1_1_u_i_component.md#function-drawcontent)


<hr>



### function OnEvent 

_This function handles events related to the button component. It dispatches different types of events based on the current state of the button and the event that has occurred._ 
```C++
virtual void AGE::ButtonComponent::OnEvent (
    Event & Event
) override
```





**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event object which contains information about the event that has occurred.

Handles events related to the button component.


This function processes various types of events such as key presses and mouse clicks, which are dispatched based on certain conditions (like if the button is focused or if it's being hovered over).




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event object that contains information about the event. 




        
Implements [*AGE::UIComponent::OnEvent*](class_a_g_e_1_1_u_i_component.md#function-onevent)


<hr>



### function OnUpdate 

_Updates the_ [_**ButtonComponent**_](class_a_g_e_1_1_button_component.md) _based on the provided_[_**TimeStep**_](class_a_g_e_1_1_time_step.md) _._
```C++
virtual void AGE::ButtonComponent::OnUpdate (
    TimeStep DeltaTime
) override
```



This function updates the [**ButtonComponent**](class_a_g_e_1_1_button_component.md) by calling [**UIComponent**](class_a_g_e_1_1_u_i_component.md)'s OnUpdate method with the given DeltaTime. If the component is visible, it creates a [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object and sets its properties accordingly before passing it to [**Renderer2D::DrawQuad**](class_a_g_e_1_1_renderer2_d.md#function-drawquad-13) for rendering.




**Parameters:**


* `DeltaTime` The time step since the last frame.

Updates the button component based on the provided time step.


This function updates the button component by calling the base class's [**OnUpdate()**](class_a_g_e_1_1_button_component.md#function-onupdate) method, then checks if the component is visible. If it is, a [**QuadProperties**](struct_a_g_e_1_1_quad_properties.md) object is created to hold properties for rendering a quad (like its transform, color etc.). The properties are set based on the button component's box properties and then used with [**Renderer2D::DrawQuad()**](class_a_g_e_1_1_renderer2_d.md#function-drawquad-13) to render the button.




**Parameters:**


* `DeltaTime` The time step since the last frame. 




        
Implements [*AGE::UIComponent::OnUpdate*](class_a_g_e_1_1_u_i_component.md#function-onupdate)


<hr>



### function SetOnClickFunc 

_Sets the on-click function for this object._ 
```C++
inline void AGE::ButtonComponent::SetOnClickFunc (
    const std::function< void()> & func
) 
```



This function sets a new function to be called when the object is clicked. The provided function should take no arguments and return void.




**Parameters:**


* `func` A std::function that will be set as the new click handler. It should have no parameters and return nothing.



**Returns:**

None


Sets the on-click function for this object.


This function sets a new function to be called when the object is clicked. The provided function should take no arguments and return void.




**Parameters:**


* `func` A std::function that will be set as the new click handler. It should have no parameters and return nothing. 




        

<hr>
## Protected Functions Documentation




### function IsButtonHovered 

_Checks if the button is hovered by the mouse cursor._ 
```C++
bool AGE::ButtonComponent::IsButtonHovered () 
```



This function calculates the normalized position of the mouse cursor relative to the window size, and then checks whether this position falls within the bounds defined by the button's dimensions. The bounds are calculated as half the width and height of the button, with the center point being at (m\_Bounds[0].x, m\_Bounds[0].y).




**Returns:**

True if the mouse cursor is hovering over the button, false otherwise.


Checks if the button is hovered by the mouse cursor.


This function calculates the normalized position of the mouse cursor relative to the framebuffer size, then checks if this position lies within the bounds defined by `m_Bounds`. If it does, the function returns true; otherwise, it returns false.




**Returns:**

A boolean value indicating whether or not the button is hovered by the mouse cursor. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Components/Public/ButtonComponent.h`

