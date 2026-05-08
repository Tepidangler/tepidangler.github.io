

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
|  [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md) \* | [**As**](#function-as-23) () <br> |
|  [**TextComponent**](class_a_g_e_1_1_text_component.md) \* | [**As**](#function-as-33) () <br> |
| virtual void | [**CallDeserialize**](#function-calldeserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer) = 0<br> |
| virtual void | [**CallSerialize**](#function-callserialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer) = 0<br> |
| virtual void | [**DrawContent**](#function-drawcontent) () = 0<br> |
| virtual void | [**DrawFontSelectionComboBox**](#function-drawfontselectioncombobox) () <br> |
|  std::string & | [**GetName**](#function-getname) () <br> |
|  [**UIProperties**](struct_a_g_e_1_1_u_i_properties.md) & | [**GetProperties**](#function-getproperties) () <br> |
|  UIComponentType::Value | [**GetType**](#function-gettype) () <br> |
| virtual void | [**OnEvent**](#function-onevent) ([**Event**](class_a_g_e_1_1_event.md) & Event) = 0<br> |
| virtual void | [**OnUpdate**](#function-onupdate) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|   | [**UIComponent**](#function-uicomponent-12) (const std::string & Name) <br> |
| virtual  | [**~UIComponent**](#function-uicomponent) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**UIComponent**](class_a_g_e_1_1_u_i_component.md) &gt; | [**Create**](#function-create) (const std::string & Name, [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) Type) <br> |
|  void | [**DrawVec3Control**](#function-drawvec3control) (const std::string & Label, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Values, float ResetValue=0.f, float ColumnWidth=100.f) <br> |






## Protected Attributes

| Type | Name |
| ---: | :--- |
|  [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) | [**m\_Type**](#variable-m_type)   = `UIComponentType::TextComponent`<br> |
















## Protected Functions

| Type | Name |
| ---: | :--- |
|   | [**UIComponent**](#function-uicomponent-22) () = default<br> |




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

```C++
template<>
TextBoxComponent * AGE::UIComponent::As () 
```




<hr>



### function As [3/3]

```C++
template<>
TextComponent * AGE::UIComponent::As () 
```




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

```C++
inline virtual void AGE::UIComponent::DrawFontSelectionComboBox () 
```




<hr>



### function GetName 

```C++
inline std::string & AGE::UIComponent::GetName () 
```




<hr>



### function GetProperties 

```C++
inline UIProperties & AGE::UIComponent::GetProperties () 
```




<hr>



### function GetType 

```C++
inline UIComponentType::Value AGE::UIComponent::GetType () 
```




<hr>



### function OnEvent 

```C++
virtual void AGE::UIComponent::OnEvent (
    Event & Event
) = 0
```




<hr>



### function OnUpdate 

```C++
inline virtual void AGE::UIComponent::OnUpdate (
    TimeStep DeltaTime
) 
```




<hr>



### function UIComponent [1/2]

```C++
AGE::UIComponent::UIComponent (
    const std::string & Name
) 
```




<hr>



### function ~UIComponent 

```C++
virtual AGE::UIComponent::~UIComponent () = default
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< UIComponent > AGE::UIComponent::Create (
    const std::string & Name,
    UIComponentType Type
) 
```




<hr>



### function DrawVec3Control 

```C++
static void AGE::UIComponent::DrawVec3Control (
    const std::string & Label,
    Vector3 & Values,
    float ResetValue=0.f,
    float ColumnWidth=100.f
) 
```




<hr>
## Protected Attributes Documentation




### variable m\_Type 

```C++
UIComponentType AGE::UIComponent::m_Type;
```




<hr>
## Protected Functions Documentation




### function UIComponent [2/2]

```C++
AGE::UIComponent::UIComponent () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/UiComponent.h`

