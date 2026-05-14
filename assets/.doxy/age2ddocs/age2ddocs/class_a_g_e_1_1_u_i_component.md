

# Class AGE::UIComponent



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UIComponent**](class_a_g_e_1_1_u_i_component.md)










Inherited by the following classes: [AGE::ButtonComponent](class_a_g_e_1_1_button_component.md),  [AGE::HorizontalBoxComponent](class_a_g_e_1_1_horizontal_box_component.md),  [AGE::TextBoxComponent](class_a_g_e_1_1_text_box_component.md),  [AGE::TextComponent](class_a_g_e_1_1_text_component.md),  [AGE::UIImageComponent](class_a_g_e_1_1_u_i_image_component.md),  [AGE::VerticalBoxComponent](class_a_g_e_1_1_vertical_box_component.md)
















## Public Attributes

| Type | Name |
| ---: | :--- |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) | [**m\_CompProperties**](#variable-m_compproperties)  <br> |
|  std::string | [**m\_Name**](#variable-m_name)   = `""`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-13) () <br> |
|  [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) \* | [**As**](#function-as-23) () <br>_This function is used to cast the current object to_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _type._ |
|  [**TextComponent**](class_a_g_e_1_1_text_component.md) \* | [**As**](#function-as-33) () <br>_This function is used to cast the current object to a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _type._ |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) = 0<br> |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) = 0<br> |
| virtual void | [**DrawContent**](#function-drawcontent) () = 0<br> |
| virtual void | [**DrawFontSelectionComboBox**](#function-drawfontselectioncombobox) () <br>_This function is responsible for drawing the font selection combo box on the screen._  |
|  std::string & | [**GetName**](#function-getname) () <br>_Gets the name of the object._  |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) & | [**GetProperties**](#function-getproperties) () <br>_Returns a reference to the UI properties object._  |
|  UIComponentType::Value | [**GetType**](#function-gettype) () <br>_This function returns the type of the UI component._  |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) = 0<br>_Handles an event by dispatching it to the appropriate handler._  |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|   | [**UIComponent**](#function-uicomponent-12) (const std::string & Name) <br>_Constructs a_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _with the given name._ |
| virtual  | [**~UIComponent**](#function-uicomponent) () = default<br>_Virtual destructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UIComponent**](class_a_g_e_1_1_u_i_component.md) &gt; | [**Create**](#function-create) (const std::string & Name, [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) Type) <br>_Creates a new instance of a UI component based on the provided type._  |
|  void | [**DrawVec3Control**](#function-drawvec3control) (const std::string & Label, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, float ResetValue=0.f, float ColumnWidth=100.f) <br>_Draws a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _control with draggable sliders._ |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) | [**m\_Type**](#variable-m_type)   = `UIComponentType::TextComponent`<br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**UIComponent**](#function-uicomponent-22) () = default<br>_Default constructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._ |




## Public Attributes Documentation




### variable m\_CompProperties 

```C++
&AGE::UIComponent::OnUpdate & AGE::UIComponent::m_CompProperties;
```




<hr>



### variable m\_Name 

```C++
std::string AGE::UIComponent::m_Name;
```




<hr>
## Public Functions Documentation




### function As [1/3]

```C++
template<typename T>
T * AGE::UIComponent::As () 
```




<hr>



### function As [2/3]

_This function is used to cast the current object to_ [_**TextBoxComponent**_](class_a_g_e_1_1_text_box_component.md) _type._
```C++
template<>
TextBoxComponent * AGE::UIComponent::As () 
```





**Returns:**

TextBoxComponent\* Returns a pointer to this object, but with its type as [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md).


This function is used to cast the current object to [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) type. 

**Returns:**

Returns a pointer of type [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), which points to this object if it can be safely casted to that type. If not, returns nullptr. 





        

<hr>



### function As [3/3]

_This function is used to cast the current object to a_ [_**TextComponent**_](class_a_g_e_1_1_text_component.md) _type._
```C++
template<>
TextComponent * AGE::UIComponent::As () 
```





**Returns:**

A pointer of type [**TextComponent**](class_a_g_e_1_1_text_component.md) that points to this instance of [**UIComponent**](class_a_g_e_1_1_u_i_component.md). If the casting fails, it will return nullptr.


This function is used to cast the current object to a [**TextComponent**](class_a_g_e_1_1_text_component.md) type.




**Returns:**

A pointer of type [**TextComponent**](class_a_g_e_1_1_text_component.md) that points to this object. If the casting fails, it will return nullptr. 





        

<hr>



### function CallDeserialize 

```C++
virtual void AGE::UIComponent::CallDeserialize (
    DataReader * Serializer
) = 0
```




<hr>



### function CallSerialize 

```C++
virtual void AGE::UIComponent::CallSerialize (
    DataWriter * Serializer
) = 0
```




<hr>



### function DrawContent 

```C++
virtual void AGE::UIComponent::DrawContent () = 0
```




<hr>



### function DrawFontSelectionComboBox 

_This function is responsible for drawing the font selection combo box on the screen._ 
```C++
inline virtual void AGE::UIComponent::DrawFontSelectionComboBox () 
```





**Returns:**

None


This function is responsible for drawing the font selection combo box on the screen.


The function does not take any parameters and returns no value. It directly interacts with the UI to display the font selection combo box. 


        

<hr>



### function GetName 

_Gets the name of the object._ 
```C++
inline std::string & AGE::UIComponent::GetName () 
```



This function returns a reference to the internal string that holds the name of the object. The caller can modify this string, and the changes will be reflected in the object's state.




**Returns:**

A reference to the internal string holding the name.


Gets the name of the object.


This function returns a reference to the internal string that holds the name of the object. The caller can modify this string, and the changes will be reflected in the object's state.




**Returns:**

A reference to the internal string holding the name. 





        

<hr>



### function GetProperties 

_Returns a reference to the UI properties object._ 
```C++
inline UIProperties & AGE::UIComponent::GetProperties () 
```



This function returns a reference to an object of type [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md), which holds all the properties related to the user interface. These properties can be used for customizing the appearance and behavior of different UI elements.




**Returns:**

A reference to the [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) object.


Gets the UI properties associated with this component. 

**Returns:**

A reference to the [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) object for this component. 





        

<hr>



### function GetType 

_This function returns the type of the UI component._ 
```C++
inline UIComponentType::Value AGE::UIComponent::GetType () 
```





**Returns:**

The type of the UI component as an enumerated value.


This function returns the type of the UI component. 

**Returns:**

The type of the UI component as an enumeration value. 





        

<hr>



### function OnEvent 

_Handles an event by dispatching it to the appropriate handler._ 
```C++
virtual void AGE::UIComponent::OnEvent (
    Event & Event
) = 0
```



This function takes in an [**Event**](class_a_g_e_1_1_event.md) object and dispatches it to the appropriate handler based on its type. The [**EventDispatcher**](class_a_g_e_1_1_event_dispatcher.md) class is used for this purpose.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) - Reference to the [**Event**](class_a_g_e_1_1_event.md) object that needs to be handled.

This function is used to handle events in the [**UIComponent**](class_a_g_e_1_1_u_i_component.md) class.




**Parameters:**


* [**Event**](class_a_g_e_1_1_event.md) The event object that needs to be handled by the [**UIComponent**](class_a_g_e_1_1_u_i_component.md). 




        

<hr>



### function OnUpdate 

```C++
inline virtual void AGE::UIComponent::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function UIComponent [1/2]

_Constructs a_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _with the given name._
```C++
AGE::UIComponent::UIComponent (
    const std::string & Name
) 
```





**Parameters:**


* `Name` The name of the component.

Constructs a [**UIComponent**](class_a_g_e_1_1_u_i_component.md) with the given name. 

**Parameters:**


* `Name` The name of the component. 




        

<hr>



### function ~UIComponent 

_Virtual destructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._
```C++
virtual AGE::UIComponent::~UIComponent () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not return anything and has no parameters.


Virtual destructor for the [**UIComponent**](class_a_g_e_1_1_u_i_component.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new instance of a UI component based on the provided type._ 
```C++
static Ref< UIComponent > AGE::UIComponent::Create (
    const std::string & Name,
    UIComponentType Type
) 
```



This function creates and returns a reference to a newly created [**UIComponent**](class_a_g_e_1_1_u_i_component.md), which can be one of several types such as [**TextComponent**](class_a_g_e_1_1_text_component.md), [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), [**HorizontalBoxComponent**](class_a_g_e_1_1_horizontal_box_component.md), [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md), [**ButtonComponent**](class_a_g_e_1_1_button_component.md) or ImageComponent. The specific type is determined by the 'Type' parameter. If an unsupported type is provided, it asserts false and returns nullptr.




**Parameters:**


* `Name` The name of the UI component to be created. 
* `Type` The type of the UI component to be created. This can be one of the following: [**TextComponent**](class_a_g_e_1_1_text_component.md), [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), [**HorizontalBoxComponent**](class_a_g_e_1_1_horizontal_box_component.md), [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md), [**ButtonComponent**](class_a_g_e_1_1_button_component.md) or ImageComponent.



**Returns:**

A reference to a newly created [**UIComponent**](class_a_g_e_1_1_u_i_component.md) instance. If an unsupported 'Type' is provided, it returns nullptr.


Creates a new instance of a UI component based on the provided type.


This function creates and returns a reference to a newly created [**UIComponent**](class_a_g_e_1_1_u_i_component.md), which can be one of several types such as [**TextComponent**](class_a_g_e_1_1_text_component.md), [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), [**HorizontalBoxComponent**](class_a_g_e_1_1_horizontal_box_component.md), [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md), [**ButtonComponent**](class_a_g_e_1_1_button_component.md) or ImageComponent. The specific type is determined by the 'Type' parameter. If an unsupported type is provided, it asserts false and returns nullptr.




**Parameters:**


* `Name` The name of the UI component to be created. 
* `Type` The type of the UI component to be created. This can be one of the following: [**TextComponent**](class_a_g_e_1_1_text_component.md), [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), [**HorizontalBoxComponent**](class_a_g_e_1_1_horizontal_box_component.md), [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md), [**ButtonComponent**](class_a_g_e_1_1_button_component.md) or ImageComponent.



**Returns:**

A reference to a newly created [**UIComponent**](class_a_g_e_1_1_u_i_component.md) instance. If an unsupported 'Type' is provided, it returns nullptr. 





        

<hr>



### function DrawVec3Control 

_Draws a_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _control with draggable sliders._
```C++
static void AGE::UIComponent::DrawVec3Control (
    const std::string & Label,
    Vector3 & Values,
    float ResetValue=0.f,
    float ColumnWidth=100.f
) 
```



This function creates an ImGui UI component that allows the user to modify three float values (x, y, z) through draggable sliders. The labels and initial values are provided as parameters.




**Parameters:**


* `Label` A string label for this control. 
* `Values` A reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object representing the current x, y, and z values. This function will modify these values when the user interacts with the sliders. 
* `ResetValue` The value to reset each individual component of the vector to when the corresponding button is clicked. 
* `ColumnWidth` The width of the column in which this control should be displayed.

Draws a 3D vector control with draggable sliders for X, Y and Z values.


This function is used to create an ImGui UI component that allows the user to manipulate three-dimensional vectors (X, Y, Z). The labels, initial vector values, reset value, and column width are all parameters of this function.




**Parameters:**


* `Label` A string representing the label for the control. 
* `Values` A reference to a [**Vector3**](struct_a_g_e_1_1_vector3.md) object that holds the current X, Y, and Z values. 
* `ResetValue` The value to which each component (X, Y, Z) of the vector will be reset when its corresponding button is clicked. 
* `ColumnWidth` The width of the column in which the control will be displayed.



**Returns:**

void 





        

<hr>
## Protected Attributes Documentation




### variable m\_Type 

```C++
UIComponentType AGE::UIComponent::m_Type;
```




<hr>
## Protected Functions Documentation




### function UIComponent [2/2]

_Default constructor for the_ [_**UIComponent**_](class_a_g_e_1_1_u_i_component.md) _class._
```C++
AGE::UIComponent::UIComponent () = default
```



This function initializes a new instance of the [**UIComponent**](class_a_g_e_1_1_u_i_component.md) class with default values. It does not take any parameters and returns nothing. The behavior is undefined if this function is called on an already initialized object.


Default constructor for the [**UIComponent**](class_a_g_e_1_1_u_i_component.md) class. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/UiComponent.h`

