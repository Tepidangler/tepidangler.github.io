

# Struct AGE::ApplicationCommandLineArgs



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**ApplicationCommandLineArgs**](struct_a_g_e_1_1_application_command_line_args.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  char \*\* | [**Args**](#variable-args)   = `nullptr`<br> |
|  int | [**Count**](#variable-count)   = `0`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  const char \* | [**operator[]**](#function-operator) (int index) const<br>_This function returns the argument at a given index._  |




























## Public Attributes Documentation




### variable Args 

```C++
char** AGE::ApplicationCommandLineArgs::Args;
```




<hr>



### variable Count 

```C++
int AGE::ApplicationCommandLineArgs::Count;
```




<hr>
## Public Functions Documentation




### function operator[] 

_This function returns the argument at a given index._ 
```C++
inline const char * AGE::ApplicationCommandLineArgs::operator[] (
    int index
) const
```



The function takes an integer as input and checks if it is within the valid range of indices for the array. If the index is out of bounds, it logs an error message and returns nullptr. Otherwise, it returns the argument at the specified index.




**Parameters:**


* `index` The zero-based index of the argument to be returned. 



**Returns:**

A pointer to a constant character string representing the argument at the given index. If the index is out of bounds, this function will return nullptr.


This function returns the argument at a given index.




**Parameters:**


* `index` The zero-based index of the argument to return. 



**Returns:**

A pointer to the argument, or nullptr if the index is out of range. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/App.h`

