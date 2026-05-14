

# Class AGE::Reverse

**template &lt;typename T&gt;**



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Reverse**](class_a_g_e_1_1_reverse.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Reverse**](#function-reverse) (T & iterable) <br>_Constructs a new instance of the_ [_**Reverse**_](class_a_g_e_1_1_reverse.md) _class with an iterable object._ |
|  auto | [**begin**](#function-begin) () const<br>_Returns a reverse iterator pointing to the last element of the container (i.e., its reverse beginning)._  |
|  auto | [**end**](#function-end) () const<br>_Returns a reverse iterator pointing to the theoretical element past the last element of the sequence._  |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Reverse< T >::__pad0__;
```




<hr>
## Public Functions Documentation




### function Reverse 

_Constructs a new instance of the_ [_**Reverse**_](class_a_g_e_1_1_reverse.md) _class with an iterable object._
```C++
inline explicit AGE::Reverse::Reverse (
    T & iterable
) 
```





**Parameters:**


* `iterable` A reference to the iterable object that will be reversed.

Constructs a new instance of the [**Reverse**](class_a_g_e_1_1_reverse.md) class with the provided iterable object. 

**Parameters:**


* `iterable` The reference to an iterable object (like vector, list etc.) that needs to be reversed. 




        

<hr>



### function begin 

_Returns a reverse iterator pointing to the last element of the container (i.e., its reverse beginning)._ 
```C++
inline auto AGE::Reverse::begin () const
```





**Returns:**

A reverse iterator which points to the end of the sequence of numbers in the container.


Returns a reverse iterator pointing to the last element of the container (i.e., its reverse beginning). 

**Returns:**

A reverse iterator which points to the end of the sequence of numbers in the container. 





        

<hr>



### function end 

_Returns a reverse iterator pointing to the theoretical element past the last element of the sequence._ 
```C++
inline auto AGE::Reverse::end () const
```





**Returns:**

A reverse iterator that points to the theoretical element past the last element of the sequence. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Core.h`

