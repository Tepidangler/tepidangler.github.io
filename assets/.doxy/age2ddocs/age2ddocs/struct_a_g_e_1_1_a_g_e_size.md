

# Struct AGE::AGESize



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  int32\_t | [**Height**](#variable-height)  <br> |
|  int32\_t | [**Width**](#variable-width)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**AGESize**](#function-agesize-12) () = default<br>_Default constructor for the_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _class._ |
|   | [**AGESize**](#function-agesize-22) (int32\_t width, int32\_t height) <br>_Constructs an instance of_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _with the specified width and height._ |
|   | [**~AGESize**](#function-agesize) () = default<br>_Default destructor for the_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _class._ |




























## Public Attributes Documentation




### variable Height 

```C++
int32_t AGE::AGESize::Height;
```




<hr>



### variable Width 

```C++
int32_t AGE::AGESize::Width;
```




<hr>
## Public Functions Documentation




### function AGESize [1/2]

_Default constructor for the_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _class._
```C++
AGE::AGESize::AGESize () = default
```




<hr>



### function AGESize [2/2]

_Constructs an instance of_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _with the specified width and height._
```C++
inline AGE::AGESize::AGESize (
    int32_t width,
    int32_t height
) 
```





**Parameters:**


* `width` The width to be set for this [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) object. 
* `height` The height to be set for this [**AGESize**](struct_a_g_e_1_1_a_g_e_size.md) object. 




        

<hr>



### function ~AGESize 

_Default destructor for the_ [_**AGESize**_](struct_a_g_e_1_1_a_g_e_size.md) _class._
```C++
AGE::AGESize::~AGESize () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It's a good practice to provide a default destructor in your classes to ensure proper cleanup when objects are destroyed.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Structs/Public/DataStructures.h`

