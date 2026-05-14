

# Struct AGE::UIComponentType



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md)






















## Public Types

| Type | Name |
| ---: | :--- |
| enum uint16\_t | [**Value**](#enum-value)  <br> |




## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  std::string & | [**ToString**](#function-tostring-14) () <br>_Returns a reference to the object's name string._  |
|  std::string | [**ToString**](#function-tostring-24) () const<br>_This function returns the name of an object as a string._  |
|  std::string | [**ToString**](#function-tostring-34) (Value Val) <br>_Converts a Value enum to its corresponding string representation._  |
|  std::string | [**ToString**](#function-tostring-44) (Value Val) const<br>_Converts an enumeration value to its corresponding string representation._  |
|  Value | [**ToValue**](#function-tovalue-12) () <br>_Returns the Value object stored in the function._  |
|  Value | [**ToValue**](#function-tovalue-22) () const<br>_This function returns the Value object 'value'._  |
|   | [**UIComponentType**](#function-uicomponenttype-12) () = default<br>_Default constructor for the_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _class._ |
|   | [**UIComponentType**](#function-uicomponenttype-22) (Value Val) <br> |
|  constexpr | [**operator Value**](#function-operator-value) () const<br>_Returns the current value of the object._  |
|   | [**operator bool**](#function-operator-bool) () const<br> |
|   | [**string**](#function-string) () const<br>_Converts the object to a string representation of its name._  |
|  bool | [**operator!=**](#function-operator) ([**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) a) const<br>_Compares the current_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _instance with another one for inequality._ |
|  std::string | [**operator()**](#function-operator_1) (Value Val) const<br>_Converts a Value to its string representation._  |
|  bool | [**operator==**](#function-operator_2) ([**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) a) const<br>_Compares the current_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _with another one for equality._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) & Instance) <br>_Deserialize function for the_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _class._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) & Instance) <br>_This function serializes a_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























## Public Types Documentation




### enum Value 

```C++
enum AGE::UIComponentType::Value {
    TextComponent,
    TextBoxComponent,
    HorizontalBoxComponent,
    VerticalBoxComponent,
    ButtonComponent,
    ImageComponent
};
```




<hr>
## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::UIComponentType::__pad0__;
```




<hr>
## Public Functions Documentation




### function ToString [1/4]

_Returns a reference to the object's name string._ 
```C++
inline std::string & AGE::UIComponentType::ToString () 
```



This function returns a reference to the internal `Name` member variable of the class instance. It is used for getting and setting the value of the name attribute.




**Returns:**

A reference to the Name string. 





        

<hr>



### function ToString [2/4]

_This function returns the name of an object as a string._ 
```C++
inline std::string AGE::UIComponentType::ToString () const
```





**Returns:**

std::string The name of the object. 





        

<hr>



### function ToString [3/4]

_Converts a Value enum to its corresponding string representation._ 
```C++
inline std::string AGE::UIComponentType::ToString (
    Value Val
) 
```



This function takes in a Value enum and returns the string equivalent of it. The possible values are "TextComponent", "TextBoxComponent", "HorizontalBoxComponent", "VerticalBoxComponent", "ButtonComponent" and "ImageComponent". If the input is not one of these, an empty string is returned.




**Parameters:**


* `Val` Value enum to be converted. 



**Returns:**

String representation of the Value enum. 





        

<hr>



### function ToString [4/4]

_Converts an enumeration value to its corresponding string representation._ 
```C++
inline std::string AGE::UIComponentType::ToString (
    Value Val
) const
```



This function takes as input an enumerated type Value and returns a string that corresponds to the enum value. The possible values of the enum are [**TextComponent**](class_a_g_e_1_1_text_component.md), [**TextBoxComponent**](class_a_g_e_1_1_text_box_component.md), [**HorizontalBoxComponent**](class_a_g_e_1_1_horizontal_box_component.md), [**VerticalBoxComponent**](class_a_g_e_1_1_vertical_box_component.md), [**ButtonComponent**](class_a_g_e_1_1_button_component.md), and ImageComponent. If the input is not one of these values, the function will return an empty string.




**Parameters:**


* `Val` An enumerated type Value to be converted into a string. 



**Returns:**

A string representation of the enum value. Returns an empty string if the input is not recognized. 





        

<hr>



### function ToValue [1/2]

_Returns the Value object stored in the function._ 
```C++
inline Value AGE::UIComponentType::ToValue () 
```



This function is used to return the 'value' variable of type Value that was previously set elsewhere in the code. It does not take any parameters and returns a single Value object.




**Returns:**

The Value object stored in the function. 





        

<hr>



### function ToValue [2/2]

_This function returns the Value object 'value'._ 
```C++
inline Value AGE::UIComponentType::ToValue () const
```





**Returns:**

The Value object that is being returned by this function. 





        

<hr>



### function UIComponentType [1/2]

_Default constructor for the_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _class._
```C++
AGE::UIComponentType::UIComponentType () = default
```




<hr>



### function UIComponentType [2/2]

```C++
inline AGE::UIComponentType::UIComponentType (
    Value Val
) 
```




<hr>



### function operator Value 

_Returns the current value of the object._ 
```C++
inline constexpr AGE::UIComponentType::operator Value () const
```



This function returns the stored value in a constant expression. It is used to get the current value of the object without modifying it.




**Returns:**

The current value of the object as a Value type. 





        

<hr>



### function operator bool 

```C++
explicit AGE::UIComponentType::operator bool () const
```




<hr>



### function string 

_Converts the object to a string representation of its name._ 
```C++
inline AGE::UIComponentType::string () const
```



This function returns the `Name` member variable as a string. It is used for converting an object into a string format.




**Returns:**

std::string The name of the object. 





        

<hr>



### function operator!= 

_Compares the current_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _instance with another one for inequality._
```C++
inline bool AGE::UIComponentType::operator!= (
    UIComponentType a
) const
```



This function compares the 'value' member of this instance with that of the provided [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) instance. It returns true if they are not equal, and false otherwise.




**Parameters:**


* `a` The [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) instance to compare with. 



**Returns:**

True if the values are not equal, false otherwise. 





        

<hr>



### function operator() 

_Converts a Value to its string representation._ 
```C++
inline std::string AGE::UIComponentType::operator() (
    Value Val
) const
```



This function takes in a Value and returns its string representation using the [**ToString()**](struct_a_g_e_1_1_u_i_component_type.md#function-tostring-14) function.




**Parameters:**


* `Val` The Value to be converted to a string. 



**Returns:**

A string representing the input Value. 





        

<hr>



### function operator== 

_Compares the current_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _with another one for equality._
```C++
inline bool AGE::UIComponentType::operator== (
    UIComponentType a
) const
```



This function compares the 'value' member of this instance with that of the provided [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) object. It returns true if they are equal, and false otherwise.




**Parameters:**


* `a` The [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) to compare against.



**Returns:**

True if the current [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) is equal to the input one, False otherwise. 





        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize function for the_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _class._
```C++
static inline void AGE::UIComponentType::Deserialize (
    DataReader * Serializer,
    UIComponentType & Instance
) 
```



This function reads a string and a Value from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) instance, which are expected to be populated with data in some way (like reading from a file or network). The read values are then used to set the Name and value properties of the passed-in [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) instance.




**Parameters:**


* `Serializer` A pointer to an initialized [**DataReader**](class_a_g_e_1_1_data_reader.md) instance. 
* `Instance` An uninitialized [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) instance that will be populated with data from the Serializer.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes a_ [_**UIComponentType**_](struct_a_g_e_1_1_u_i_component_type.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::UIComponentType::Serialize (
    DataWriter * Serializer,
    const UIComponentType & Instance
) 
```



The function writes the name of the component and its value to the writer, which can be used for further processing or storage.




**Parameters:**


* `Serializer` Pointer to an object that implements the [**DataWriter**](class_a_g_e_1_1_data_writer.md) interface. This is where the serialized data will be written. 
* `Instance` The [**UIComponentType**](struct_a_g_e_1_1_u_i_component_type.md) instance to be serialized. Contains the name and value of the component.



**Returns:**

None 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/UI/Public/UIStructs.h`

