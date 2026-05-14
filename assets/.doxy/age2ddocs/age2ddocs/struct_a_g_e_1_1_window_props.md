

# Struct AGE::WindowProps



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**WindowProps**](struct_a_g_e_1_1_window_props.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  unsigned int | [**Height**](#variable-height)  <br> |
|  const char \* | [**String**](#variable-string)  <br> |
|  std::string | [**Title**](#variable-title)  <br> |
|  unsigned int | [**Width**](#variable-width)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**WindowProps**](#function-windowprops) (const std::string & T="Alcoy Game Engine Editor", unsigned int W=1280, unsigned int H=720, const char \* S="") <br>_Constructs a_ [_**WindowProps**_](struct_a_g_e_1_1_window_props.md) _object with default values._ |




























## Public Attributes Documentation




### variable Height 

```C++
unsigned int AGE::WindowProps::Height;
```




<hr>



### variable String 

```C++
const char* AGE::WindowProps::String;
```




<hr>



### variable Title 

```C++
std::string AGE::WindowProps::Title;
```




<hr>



### variable Width 

```C++
unsigned int AGE::WindowProps::Width;
```




<hr>
## Public Functions Documentation




### function WindowProps 

_Constructs a_ [_**WindowProps**_](struct_a_g_e_1_1_window_props.md) _object with default values._
```C++
inline AGE::WindowProps::WindowProps (
    const std::string & T="Alcoy Game Engine Editor",
    unsigned int W=1280,
    unsigned int H=720,
    const char * S=""
) 
```



The function initializes the properties of a window, including its title, width, height and string. If no arguments are provided, it uses default values.




**Parameters:**


* `T` A string representing the title of the window (default: "Alcoy Game Engine Editor"). 
* `W` An unsigned integer representing the width of the window in pixels (default: 1280). 
* `H` An unsigned integer representing the height of the window in pixels (default: 720). 
* `S` A C-style string representing additional information about the window (default: "").



**Returns:**

A [**WindowProps**](struct_a_g_e_1_1_window_props.md) object with properties set according to the provided arguments. If no arguments are provided, it uses default values.


Constructs a [**WindowProps**](struct_a_g_e_1_1_window_props.md) object with default values.


The constructor initializes the properties of the window, including its title, width, height and string. If no arguments are provided, it defaults to "Alcoy Game Engine Editor", 1280x720 resolution and an empty string.




**Parameters:**


* `T` Title of the window (default: "Alcoy Game Engine Editor") 
* `W` Width of the window in pixels (default: 1280) 
* `H` Height of the window in pixels (default: 720) 
* `S` String to be displayed on the window (default: "") 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Window.h`

