

# Struct AGE::AGEFunction

**template &lt;typename R, typename E&gt;**



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  std::vector&lt; rttr::variant &gt; | [**Args**](#variable-args)  <br> |
|  E \* | [**Entt**](#variable-entt)  <br> |
|  uint64\_t | [**EnttID**](#variable-enttid)  <br> |
|  uint64\_t | [**RefID**](#variable-refid)  <br> |
|  Ref&lt; R &gt; | [**Reference**](#variable-reference)  <br> |
|  std::string | [**Val**](#variable-val)  <br> |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br> |
|  bool | [**bIsUtilFunction**](#variable-bisutilfunction)   = `false`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGEFunction**](#function-agefunction-13) () = default<br>_Default constructor for the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _class._ |
|   | [**AGEFunction**](#function-agefunction-23) (const std::string & Exec, std::vector&lt; rttr::variant &gt; Arguments, E \* Value=nullptr, Ref&lt; R &gt; & Ptr=nullptr) <br>_Constructs an instance of the class with given parameters._  |
|   | [**AGEFunction**](#function-agefunction-33) (const [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) &) = default<br> |
|  rttr::variant | [**Execute**](#function-execute) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime=0.f) <br>_Executes the function stored in Reference with optional delta time as input._  |
| virtual  | [**~AGEFunction**](#function-agefunction) () = default<br>_Virtual destructor for the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Serializer, [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) & Data) <br>_Deserialize function data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _into an_[_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _object._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) & Data) <br>_This function serializes the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._ |






















## Protected Functions

| Type | Name |
| ---: | :--- |
|  rttr::variant | [**Function**](#function-function) (Ref&lt; R &gt; & Ptr, [**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime=0.f) <br>_This function is used to execute a method on an entity. It can be either a utility function or a normal method of the entity's class._  |




## Public Attributes Documentation




### variable Args 

```C++
std::vector<rttr::variant> AGE::AGEFunction< R, E >::Args;
```




<hr>



### variable Entt 

```C++
E* AGE::AGEFunction< R, E >::Entt;
```




<hr>



### variable EnttID 

```C++
uint64_t AGE::AGEFunction< R, E >::EnttID;
```




<hr>



### variable RefID 

```C++
uint64_t AGE::AGEFunction< R, E >::RefID;
```




<hr>



### variable Reference 

```C++
Ref<R> AGE::AGEFunction< R, E >::Reference;
```




<hr>



### variable Val 

```C++
std::string AGE::AGEFunction< R, E >::Val;
```




<hr>



### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::AGEFunction< R, E >::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

```C++
COMMENT AGE::AGEFunction< R, E >::__pad1__;
```




<hr>



### variable bIsUtilFunction 

```C++
bool AGE::AGEFunction< R, E >::bIsUtilFunction;
```




<hr>
## Public Functions Documentation




### function AGEFunction [1/3]

_Default constructor for the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _class._
```C++
AGE::AGEFunction::AGEFunction () = default
```



Default constructor for the AGE class.


This function initializes an instance of the AGE class with its default values. It is used to create a new object without any specific initialization.




**Returns:**

void 





        

<hr>



### function AGEFunction [2/3]

_Constructs an instance of the class with given parameters._ 
```C++
inline AGE::AGEFunction::AGEFunction (
    const std::string & Exec,
    std::vector< rttr::variant > Arguments,
    E * Value=nullptr,
    Ref< R > & Ptr=nullptr
) 
```





**Parameters:**


* `Exec` A string parameter that is used for some purpose, but not specified in this comment. 
* `Arguments` A vector of rttr::variant objects which are used to perform various operations. 
* `Value` Pointer to an E object, default value is nullptr. 
* `Ptr` Reference to a R object, default value is nullptr.

Constructs an instance of the class with given parameters. 

**Parameters:**


* `Exec` The string to be stored in the object. 
* `Arguments` A vector of rttr::variant objects to be stored in the object. 
* `Value` Pointer to an E object, which is copied into the object if not null. Defaults to nullptr. 
* `Ptr` Reference to a R object, which can be used to access and modify the object. Defaults to nullptr. 




        

<hr>



### function AGEFunction [3/3]

```C++
AGE::AGEFunction::AGEFunction (
    const AGEFunction &
) = default
```




<hr>



### function Execute 

_Executes the function stored in Reference with optional delta time as input._ 
```C++
inline rttr::variant AGE::AGEFunction::Execute (
    TimeStep DeltaTime=0.f
) 
```



The function will be executed based on whether a reference to an object is present and if DeltaTime &gt; 0. If only Reference is provided, it assumes that no additional parameters are required for execution.




**Parameters:**


* `DeltaTime` Optional parameter representing time elapsed since the last frame. Defaults to 0.f. 



**Returns:**

The return value of the function stored in Reference.


Executes the function stored in Reference with an optional delta time as parameter.


The function to be executed is determined by the state of Reference. If it's not null, then either Function(Reference) or Function(Reference, DeltaTime) will be called depending on whether DeltaTime &gt; 0. If Reference is null and DeltaTime &gt; 0, then Function(nullptr, DeltaTime) is called.




**Parameters:**


* `DeltaTime` The time step to pass into the function (optional). 



**Returns:**

rttr::variant The return value of the executed function. 





        

<hr>



### function ~AGEFunction 

_Virtual destructor for the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _class._
```C++
virtual AGE::AGEFunction::~AGEFunction () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not take any parameters and returns void.


Virtual destructor for the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) class.


This function is responsible for freeing any resources that were allocated by the object during its lifetime. It does not take any parameters and returns void. 


        

<hr>
## Public Static Functions Documentation




### function Deserialize 

_Deserialize function data from a_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _into an_[_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _object._
```C++
static inline void AGE::AGEFunction::Deserialize (
    DataReader * Serializer,
    AGEFunction & Data
) 
```



This function reads raw data from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and populates an [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object with it. The function checks if 'HasEntt' is true, in which case it also reads an EnttID. It then reads a string value for 'Val'. 

**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides raw data. 
* `Data` Reference to the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object where the deserialized data will be stored.



**Returns:**

void


Deserializes data from a [**DataReader**](class_a_g_e_1_1_data_reader.md) into an [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object.


This function reads raw data from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and populates an [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object with it. The function checks if 'HasEntt' is true, in which case it also reads an EnttID. It then reads a string value for 'Val'. 

**Parameters:**


* `Serializer` Pointer to the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides raw data. 
* `Data` Reference to the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object where the deserialized data will be stored.



**Returns:**

void 





        

<hr>



### function Serialize 

_This function serializes the_ [_**AGEFunction**_](struct_a_g_e_1_1_a_g_e_function.md) _data into a_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _object._
```C++
static inline void AGE::AGEFunction::Serialize (
    DataWriter * Serializer,
    const AGEFunction & Data
) 
```



The function writes the RefID, bIsUtilFunction and Entt status of the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) to the [**DataWriter**](class_a_g_e_1_1_data_writer.md). If the Entt is present, it also writes the EnttID. It then writes the Val string of the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md).




**Parameters:**


* `Serializer` Pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where serialized data will be written into. 
* `Data` Reference to an [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object that needs to be serialized.



**Returns:**

void


This function serializes the [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) data into a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object.


The function writes the RefID, bIsUtilFunction flag, and Entt status to the Serializer. If an Entt exists, it also writes the EnttID. Finally, it writes the Val string.




**Parameters:**


* `Serializer` Pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object where serialized data will be written. 
* `Data` Reference to an [**AGEFunction**](struct_a_g_e_1_1_a_g_e_function.md) object that contains the data to be serialized.



**Returns:**

void 





        

<hr>
## Protected Functions Documentation




### function Function 

_This function is used to execute a method on an entity. It can be either a utility function or a normal method of the entity's class._ 
```C++
inline rttr::variant AGE::AGEFunction::Function (
    Ref< R > & Ptr,
    TimeStep DeltaTime=0.f
) 
```





**Parameters:**


* `Ptr` Reference to the entity. If it's not valid, the function will return without doing anything. 
* `DeltaTime` The time step for the update. Default is 0.f.



**Returns:**

Returns a variant containing the result of the method execution if successful, or an invalid variant otherwise.


This function is used to perform some operation on a given entity. It can be either an update function or any other type of function depending on the input parameters and conditions.




**Parameters:**


* `Ptr` A reference to an object of class R. 
* `DeltaTime` The time elapsed since the last frame, default is 0.f. 



**Returns:**

rttr::variant Returns a variant that contains the result of the operation performed on the entity. If no valid operation was performed, it returns an empty variant. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/Functions.h`

