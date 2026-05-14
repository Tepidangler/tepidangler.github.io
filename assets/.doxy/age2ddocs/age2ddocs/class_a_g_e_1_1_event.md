

# Class AGE::Event



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Event**](class_a_g_e_1_1_event.md)



_Abstract base class for an event._ [More...](#detailed-description)

* `#include <Event.h>`





Inherited by the following classes: [AGE::AppRenderEvent](class_a_g_e_1_1_app_render_event.md),  [AGE::AppTickEvent](class_a_g_e_1_1_app_tick_event.md),  [AGE::AppUpdateEvent](class_a_g_e_1_1_app_update_event.md),  [AGE::FramebufferResizeEvent](class_a_g_e_1_1_framebuffer_resize_event.md),  [AGE::InputEvent](class_a_g_e_1_1_input_event.md),  [AGE::KeyEvent](class_a_g_e_1_1_key_event.md),  [AGE::MouseEvent](class_a_g_e_1_1_mouse_event.md),  [AGE::ProjectCreatedEvent](class_a_g_e_1_1_project_created_event.md),  [AGE::ProjectLoadedEvent](class_a_g_e_1_1_project_loaded_event.md),  [AGE::RenderUIEvent](class_a_g_e_1_1_render_u_i_event.md),  [AGE::RendererChangeEvent](class_a_g_e_1_1_renderer_change_event.md),  [AGE::SceneEvent](class_a_g_e_1_1_scene_event.md),  [AGE::StringCopyEvent](class_a_g_e_1_1_string_copy_event.md),  [AGE::StringPasteEvent](class_a_g_e_1_1_string_paste_event.md),  [AGE::WidgetActivatedEvent](class_a_g_e_1_1_widget_activated_event.md),  [AGE::WidgetConstructedEvent](class_a_g_e_1_1_widget_constructed_event.md),  [AGE::WidgetDeactivatedEvent](class_a_g_e_1_1_widget_deactivated_event.md),  [AGE::WindowCloseEvent](class_a_g_e_1_1_window_close_event.md),  [AGE::WindowFocusEvent](class_a_g_e_1_1_window_focus_event.md),  [AGE::WindowLostFocusEvent](class_a_g_e_1_1_window_lost_focus_event.md),  [AGE::WindowMovedEvent](class_a_g_e_1_1_window_moved_event.md),  [AGE::WindowResizeEvent](class_a_g_e_1_1_window_resize_event.md)
















## Public Attributes

| Type | Name |
| ---: | :--- |
|  bool | [**Handled**](#variable-handled)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
| virtual int | [**GetCategoryFlags**](#function-getcategoryflags) () const = 0<br> |
| virtual EventType | [**GetEventType**](#function-geteventtype) () const = 0<br> |
| virtual const char \* | [**GetName**](#function-getname) () const = 0<br> |
|  bool | [**IsInCategory**](#function-isincategory) (EventCategory Category) <br>_Checks if an event is in a specific category._  |
| virtual std::string | [**ToString**](#function-tostring) () const<br>_Returns a string representation of the object._  |




























## Detailed Description


This is the abstract base class that represents a generic event in the system. It provides methods to get information about the type of the event, its category flags and whether it has been handled or not.


Represents an event in the system.


This class represents a generic event that can be handled by various components of the system. It provides methods to get information about the type, category and name of the event. The ToString method returns the name of the event as default implementation but subclasses may override it with more meaningful representation. 


    
## Public Attributes Documentation




### variable Handled 

```C++
bool AGE::Event::Handled;
```




<hr>
## Public Functions Documentation




### function GetCategoryFlags 

```C++
virtual int AGE::Event::GetCategoryFlags () const = 0
```




<hr>



### function GetEventType 

```C++
virtual EventType AGE::Event::GetEventType () const = 0
```




<hr>



### function GetName 

```C++
virtual const char * AGE::Event::GetName () const = 0
```




<hr>



### function IsInCategory 

_Checks if an event is in a specific category._ 
```C++
inline bool AGE::Event::IsInCategory (
    EventCategory Category
) 
```



This function checks whether the provided EventCategory is set within the categories that are currently active. The comparison is done by bitwise AND operation with GetCategoryFlags() and Category.




**Parameters:**


* `Category` - The category to check against. 



**Returns:**

True if the event is in the specified category, false otherwise.


Checks if an event is in a specific category.


This function checks whether the given EventCategory (bitmask) is set within the result of GetCategoryFlags(). It uses bitwise AND operation to compare the Category flag with all flags.




**Parameters:**


* `Category` The category to check against. 



**Returns:**

True if the event is in the specified category, false otherwise. 





        

<hr>



### function ToString 

_Returns a string representation of the object._ 
```C++
inline virtual std::string AGE::Event::ToString () const
```



This function returns a string that represents the current object's state. It does this by calling the `GetName` method and returning its result.




**Returns:**

A string representing the current object's name.


Converts the object into a string representation.


This function returns a string that represents the current object's name. It uses the `GetName` method to get the name of the object.




**Returns:**

A string representing the current object's name. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Events/Public/Event.h`

