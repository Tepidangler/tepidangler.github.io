

# Struct AGE::Vector4



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Vector4**](struct_a_g_e_1_1_vector4.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br> |
|  COMMENT | [**\_\_pad1\_\_**](#variable-__pad1__)  <br>_Assigns the values of another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to this one._ |
|  COMMENT | [**\_\_pad2\_\_**](#variable-__pad2__)  <br> |
|  float | [**w**](#variable-w)  <br> |
|  float | [**x**](#variable-x)  <br> |
|  float | [**y**](#variable-y)  <br> |
|  float | [**z**](#variable-z)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**Vector4**](#function-vector4-17) () <br>_Default constructor for the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class. Initializes all components to zero._ |
|   | [**Vector4**](#function-vector4-27) (float a) <br>_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with all components set to the same value._ |
|   | [**Vector4**](#function-vector4-37) (glm::vec4 vec) <br>_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from a glm::vec4._ |
|   | [**Vector4**](#function-vector4-47) (float a, float b, float c, float d) <br>_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object with four components._ |
|   | [**Vector4**](#function-vector4-57) (uint8\_t a, uint8\_t b, uint8\_t c, uint8\_t d) <br>_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from four uint8\_t values, each representing a byte of data. The bytes are converted to float and normalized between 0 and 100._ |
|   | [**Vector4**](#function-vector4-67) (const float \* color) <br>_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from an array of four floats._ |
|   | [**Vector4**](#function-vector4-77) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Other) <br>_Copy constructor for_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class._ |
|  float | [**dot**](#function-dot) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Computes the dot product of this vector with another vector._  |
|  float | [**magnitude**](#function-magnitude) () const<br>_Calculates the magnitude of a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object using the Euclidean distance formula._ |
|  float | [**norm**](#function-norm) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Calculates the magnitude of a four dimensional vector._  |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**normalize**](#function-normalize) () const<br>_Normalizes this vector._  |
|   | [**string**](#function-string) () <br>_Converts the object to a string representation._  |
|   | [**operator uint32\_t**](#function-operator-uint32_t) () <br>_Converts the current color to a uint32\_t representation._  |
|  &lt; doxygen comment &gt; | [**operator uint32\_t \***](#function-operator-uint32_t-*) () <br> |
|  bool | [**operator!=**](#function-operator) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Compares this_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with another for inequality._ |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator\***](#function-operator_1) (float scalar) const<br>_This function returns a new vector that is the result of scaling this vector by a given scalar value._  |
|  void | [**operator\*=**](#function-operator_2) (float scalar) <br>_Multiplies the four components of this vector by a scalar._  |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator+**](#function-operator_3) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Adds another vector to this one._  |
|  void | [**operator+=**](#function-operator_4) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) <br>_This function adds the components of a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to this vector._ |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator-**](#function-operator-) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Subtracts another vector from this one component by component._  |
|  void | [**operator-=**](#function-operator-_1) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) <br>_Subtracts another_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _from this one._ |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) | [**operator/**](#function-operator_5) (float scalar) const<br>_Performs division of the vector by a scalar value._  |
|  void | [**operator/=**](#function-operator_6) (float scalar) <br>_Divides the vector by a scalar value._  |
|  [**Vector4**](struct_a_g_e_1_1_vector4.md) & | [**operator=**](#function-operator_7) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & Other) <br>_Assigns the values of another_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to this one._ |
|  void | [**operator=**](#function-operator_8) ([**Vector3**](struct_a_g_e_1_1_vector3.md) & vec) <br> |
|  bool | [**operator==**](#function-operator_9) (const [**Vector4**](struct_a_g_e_1_1_vector4.md) & vec) const<br>_Compares this_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with another for equality._ |
|  float & | [**operator[]**](#function-operator_10) (int i) <br>_This function returns a reference to the element at index 'i' in an array of float values._  |
|  const float & | [**operator[]**](#function-operator_11) (int i) const<br>_Returns a reference to the element at index 'i' in an array of constant floats._  |
|   | [**~Vector4**](#function-vector4) () = default<br>_Default destructor for the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class._ |




























## Public Attributes Documentation




### variable \_\_pad0\_\_ 

```C++
COMMENT AGE::Vector4::__pad0__;
```




<hr>



### variable \_\_pad1\_\_ 

_Assigns the values of another_ [_**Vector3**_](struct_a_g_e_1_1_vector3.md) _to this one._
```C++
COMMENT AGE::Vector4::__pad1__;
```



This operator overload allows for easy assignment of the x, y and z components from a different [**Vector3**](struct_a_g_e_1_1_vector3.md) object. The w component is always set to 1.0f.




**Parameters:**


* `vec` A reference to the [**Vector3**](struct_a_g_e_1_1_vector3.md) that we want to copy the values from. 




        

<hr>



### variable \_\_pad2\_\_ 

```C++
COMMENT AGE::Vector4::__pad2__;
```




<hr>



### variable w 

```C++
float AGE::Vector4::w;
```




<hr>



### variable x 

```C++
float AGE::Vector4::x;
```




<hr>



### variable y 

```C++
float AGE::Vector4::y;
```




<hr>



### variable z 

```C++
float AGE::Vector4::z;
```




<hr>
## Public Functions Documentation




### function Vector4 [1/7]

_Default constructor for the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class. Initializes all components to zero._
```C++
AGE::Vector4::Vector4 () 
```



This function initializes each component of a [**Vector4**](struct_a_g_e_1_1_vector4.md) object, setting them all to zero. The four components are x, y, z and w. They represent different aspects of the vector such as position, direction or color intensity.




**Returns:**

void


Constructs a [**Vector4**](struct_a_g_e_1_1_vector4.md) object with all components set to zero. 


        

<hr>



### function Vector4 [2/7]

_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with all components set to the same value._
```C++
AGE::Vector4::Vector4 (
    float a
) 
```



This constructor initializes each component of the vector to the provided float value 'a'. The resulting vector will have x, y, z and w equal to 'a'.




**Parameters:**


* `a` The value to initialize all four components of the [**Vector4**](struct_a_g_e_1_1_vector4.md) with.

Constructs a [**Vector4**](struct_a_g_e_1_1_vector4.md) with all components set to the same value.


This constructor initializes each component of the vector to the provided float value. The resulting vector will have x, y, z and w equal to this single value.




**Parameters:**


* `a` The value to initialize all four components of the [**Vector4**](struct_a_g_e_1_1_vector4.md) with. 




        

<hr>



### function Vector4 [3/7]

_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from a glm::vec4._
```C++
AGE::Vector4::Vector4 (
    glm::vec4 vec
) 
```



This constructor takes a glm::vec4 and assigns its x, y, z, w values to the corresponding members of this [**Vector4**](struct_a_g_e_1_1_vector4.md) object.




**Parameters:**


* `vec` The source vector.

Constructs a [**Vector4**](struct_a_g_e_1_1_vector4.md) object from a glm::vec4.


This constructor takes a glm::vec4 and assigns its x, y, z, w values to the corresponding members of this [**Vector4**](struct_a_g_e_1_1_vector4.md) object.




**Parameters:**


* `vec` The input vector. 




        

<hr>



### function Vector4 [4/7]

_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object with four components._
```C++
AGE::Vector4::Vector4 (
    float a,
    float b,
    float c,
    float d
) 
```



This function is used to initialize a [**Vector4**](struct_a_g_e_1_1_vector4.md) object with the given four float values. The first two parameters represent x and y coordinates, while the next two are z and w respectively.




**Parameters:**


* `a` Float value representing the x component of the vector. 
* `b` Float value representing the y component of the vector. 
* `c` Float value representing the z component of the vector. 
* `d` Float value representing the w component of the vector.

Constructs a [**Vector4**](struct_a_g_e_1_1_vector4.md) object with four components.


This function initializes a [**Vector4**](struct_a_g_e_1_1_vector4.md) object with the given four float values, which represent the x, y, z and w coordinates of the vector respectively.




**Parameters:**


* `a` The first component (x) of the vector. 
* `b` The second component (y) of the vector. 
* `c` The third component (z) of the vector. 
* `d` The fourth component (w) of the vector. 




        

<hr>



### function Vector4 [5/7]

_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from four uint8\_t values, each representing a byte of data. The bytes are converted to float and normalized between 0 and 100._
```C++
AGE::Vector4::Vector4 (
    uint8_t a,
    uint8_t b,
    uint8_t c,
    uint8_t d
) 
```





**Parameters:**


* `a` First input byte, represents the x-coordinate. 
* `b` Second input byte, represents the y-coordinate. 
* `c` Third input byte, represents the z-coordinate. 
* `d` Fourth input byte, represents the w-coordinate. 




        

<hr>



### function Vector4 [6/7]

_Constructs a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object from an array of four floats._
```C++
AGE::Vector4::Vector4 (
    const float * color
) 
```



The constructor takes in an array of four floats, which are used to initialize the x, y, z and w members of the [**Vector4**](struct_a_g_e_1_1_vector4.md) object.




**Parameters:**


* `color` An array of four floats representing the initial values for the [**Vector4**](struct_a_g_e_1_1_vector4.md) object.



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) object with its x, y, z and w members set to the corresponding elements in the input array.


Constructs a [**Vector4**](struct_a_g_e_1_1_vector4.md) object from an array of four floats.


This constructor takes in an array of four floats and assigns them to the x, y, z, and w members of the [**Vector4**](struct_a_g_e_1_1_vector4.md) object respectively. The color parameter is expected to be in RGBA format where R (Red), G (Green), B (Blue) and A (Alpha) are float values between 0.0 and 1.0. 

**Parameters:**


* `color` Pointer to an array of four floats representing the RGBA color values. 




        

<hr>



### function Vector4 [7/7]

_Copy constructor for_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class._
```C++
inline AGE::Vector4::Vector4 (
    const Vector4 & Other
) 
```



This function creates a new instance of the [**Vector4**](struct_a_g_e_1_1_vector4.md) class by copying the values from another instance.




**Parameters:**


* `Other` The [**Vector4**](struct_a_g_e_1_1_vector4.md) object to copy from. 




        

<hr>



### function dot 

_Computes the dot product of this vector with another vector._ 
```C++
inline float AGE::Vector4::dot (
    const Vector4 & vec
) const
```



The function takes a constant reference to another [**Vector4**](struct_a_g_e_1_1_vector4.md) object and calculates the dot product by multiplying each corresponding component of both vectors (x, y, z, w) together and summing them up. It then returns the result as a float value.




**Parameters:**


* `vec` The other vector with which this one is to be multiplied. 



**Returns:**

A float representing the dot product of this vector and the input vector.


Computes the dot product of this vector with another [**Vector4**](struct_a_g_e_1_1_vector4.md) object.


The function takes a constant reference to another [**Vector4**](struct_a_g_e_1_1_vector4.md) object and calculates the dot product by multiplying each component of the current [**Vector4**](struct_a_g_e_1_1_vector4.md) object (x, y, z, w) with the corresponding component in the input [**Vector4**](struct_a_g_e_1_1_vector4.md) object. It then returns the result as a float value.




**Parameters:**


* `vec` A const reference to the other [**Vector4**](struct_a_g_e_1_1_vector4.md) object for which the dot product is calculated. 



**Returns:**

The computed dot product of this vector and the provided one. 





        

<hr>



### function magnitude 

_Calculates the magnitude of a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _object using the Euclidean distance formula._
```C++
inline float AGE::Vector4::magnitude () const
```





**Parameters:**


* `None` 



**Returns:**

Returns a float representing the magnitude of the vector. If the vector is (0, 0, 0, 0), returns 0.0. 





        

<hr>



### function norm 

_Calculates the magnitude of a four dimensional vector._ 
```C++
inline float AGE::Vector4::norm (
    const Vector4 & vec
) const
```



This function takes in a constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object and calculates its magnitude by taking the square root of the sum of the squares of each component (x, y, z, w) subtracted from the corresponding components of the input vector. The result is returned as a float.




**Parameters:**


* `vec` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object representing the vector for which we want to calculate the magnitude.



**Returns:**

Returns a float value representing the magnitude of the input vector.


Calculates the magnitude of a four dimensional vector.


This function takes a constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object and calculates its magnitude by applying the Euclidean distance formula on each component of the vector with respect to the origin (0,0,0,0). The result is returned as a float value.




**Parameters:**


* `vec` A constant reference to the [**Vector4**](struct_a_g_e_1_1_vector4.md) object whose magnitude is being calculated. 



**Returns:**

Returns the magnitude of the input vector as a float. 





        

<hr>



### function normalize 

_Normalizes this vector._ 
```C++
Vector4 AGE::Vector4::normalize () const
```



This function scales the vector so that its length (or magnitude) is equal to one, while maintaining its direction. If the vector has a zero length (i.e., it's a zero vector), the result will be another zero vector.




**Returns:**

[**Vector4**](struct_a_g_e_1_1_vector4.md) The normalized version of this vector.


Normalizes this vector.


This function scales the components of the vector so that its length (magnitude) is equal to one, preserving the direction but making it a unit vector. If the vector has zero length (i.e., all elements are zero), the behavior is undefined and may result in division by zero or other unexpected errors.




**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) object representing the normalized version of this vector. 





        

<hr>



### function string 

_Converts the object to a string representation._ 
```C++
inline AGE::Vector4::string () 
```



This function converts the current object into a string format that includes all its properties. The output is in the form "X: &lt;x&gt; Y: &lt;y&gt; Z: &lt;z&gt; W: &lt;w&gt;".




**Returns:**

A std::string containing the formatted representation of the object.


Converts the object to a string representation.


This function converts the current object into its string representation, which includes the values of x, y, z and w. The format is "X: &lt;x&gt; Y: &lt;y&gt; Z: &lt;z&gt; W: &lt;w&gt;".




**Returns:**

A std::string containing the formatted coordinates. 





        

<hr>



### function operator uint32\_t 

_Converts the current color to a uint32\_t representation._ 
```C++
inline AGE::Vector4::operator uint32_t () 
```



This function converts the current color into a 32-bit unsigned integer format, where each byte represents an RGBA component (Red, Green, Blue, Alpha). The conversion is done in such a way that if w &gt; 0, then each of the four bytes will be in the range [0, 255]. If w &lt;= 0, then all components are set to zero.




**Returns:**

A 32-bit unsigned integer representing the current color. 





        

<hr>



### function operator uint32\_t \* 

```C++
inline < doxygen comment > AGE::Vector4::operator uint32_t * () 
```




<hr>



### function operator!= 

_Compares this_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with another for inequality._
```C++
inline bool AGE::Vector4::operator!= (
    const Vector4 & vec
) const
```



This function compares each of the x, y, z and w components of this [**Vector4**](struct_a_g_e_1_1_vector4.md) to those of the provided [**Vector4**](struct_a_g_e_1_1_vector4.md). It returns true if any of these are not equal, false otherwise.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to compare against. 



**Returns:**

True if any component is different, false if all are identical.


Compares this [**Vector4**](struct_a_g_e_1_1_vector4.md) with another for inequality.


This function compares each of the x, y, z and w components of this [**Vector4**](struct_a_g_e_1_1_vector4.md) with those of the provided [**Vector4**](struct_a_g_e_1_1_vector4.md). It returns true if any of these component are not equal, false otherwise.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to compare against. 



**Returns:**

True if any of the x, y, z or w components differ from this [**Vector4**](struct_a_g_e_1_1_vector4.md)'s corresponding components; false otherwise. 





        

<hr>



### function operator\* 

_This function returns a new vector that is the result of scaling this vector by a given scalar value._ 
```C++
inline Vector4 AGE::Vector4::operator* (
    float scalar
) const
```





**Parameters:**


* `scalar` The value to scale each component of the vector by. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the scaled vector.


This function returns a new vector that is the result of scaling this vector by a given scalar.


The resulting vector's x, y, z and w components are each multiplied by the provided scalar.




**Parameters:**


* `scalar` The value to scale the vector by. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) representing the scaled vector. 





        

<hr>



### function operator\*= 

_Multiplies the four components of this vector by a scalar._ 
```C++
inline void AGE::Vector4::operator*= (
    float scalar
) 
```



This function multiplies each component (x, y, z, w) of this vector by the given scalar. The result is stored in-place and does not return a new vector.




**Parameters:**


* `scalar` The value to multiply with.

Multiplies the vector by a scalar value.


This function multiplies each component of the vector (x, y, z, w) by the given scalar value. The result is stored in the same components of the vector.




**Parameters:**


* `scalar` The scalar value to multiply with. 




        

<hr>



### function operator+ 

_Adds another vector to this one._ 
```C++
inline Vector4 AGE::Vector4::operator+ (
    const Vector4 & vec
) const
```



This function adds the x, y and z components of another [**Vector4**](struct_a_g_e_1_1_vector4.md) object to those of this object. The w component is not modified.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) object to add to this one. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) object resulting from the addition operation.


Adds another vector to this one.


This function adds the x, y and z components of another [**Vector4**](struct_a_g_e_1_1_vector4.md) object to those of this one. The w component of the other vector is added directly without modification.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) object to add to this one. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) object with the summed values. 





        

<hr>



### function operator+= 

_This function adds the components of a_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to this vector._
```C++
inline void AGE::Vector4::operator+= (
    const Vector4 & vec
) 
```



The operator+= is used for adding another [**Vector4**](struct_a_g_e_1_1_vector4.md) object's values to the current one. It modifies the current object by adding the x, y, z and w components of the given [**Vector4**](struct_a_g_e_1_1_vector4.md) to the corresponding components of the current object. 

**Parameters:**


* `vec` A const reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object that will be added to this vector.



**Returns:**

void


This function adds the components of another [**Vector4**](struct_a_g_e_1_1_vector4.md) to this one.


The operator += is used to add the x, y, z and w values from a given [**Vector4**](struct_a_g_e_1_1_vector4.md) to the corresponding components in this [**Vector4**](struct_a_g_e_1_1_vector4.md).




**Parameters:**


* `vec` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object whose components will be added to those of this [**Vector4**](struct_a_g_e_1_1_vector4.md).



**Returns:**

void 





        

<hr>



### function operator- 

_Subtracts another vector from this one component by component._ 
```C++
inline Vector4 AGE::Vector4::operator- (
    const Vector4 & vec
) const
```



This function subtracts the corresponding components of the given vector from this vector's components. The result is a new [**Vector4**](struct_a_g_e_1_1_vector4.md) with the differences computed.




**Parameters:**


* `vec` The vector to be subtracted from this one. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) resulting from the component-wise subtraction.


Subtracts another vector from this one component by component.


This function subtracts the corresponding components of the given vector from those of this vector. The result is a new [**Vector4**](struct_a_g_e_1_1_vector4.md) with the differences in its components.




**Parameters:**


* `vec` The vector to be subtracted from this one. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) containing the component-wise difference between this and the input vector. 





        

<hr>



### function operator-= 

_Subtracts another_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _from this one._
```C++
inline void AGE::Vector4::operator-= (
    const Vector4 & vec
) 
```



This function subtracts the x, y, z and w components of the given vector from the corresponding components of this vector.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to be subtracted.



**Returns:**

void


Subtracts another [**Vector4**](struct_a_g_e_1_1_vector4.md) from this one.


This function subtracts the x, y, z and w components of the given vector from the corresponding components of this vector.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to be subtracted. 




        

<hr>



### function operator/ 

_Performs division of the vector by a scalar value._ 
```C++
inline Vector4 AGE::Vector4::operator/ (
    float scalar
) const
```





**Parameters:**


* `scalar` The float value to divide each component of the vector by. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) where each component is the result of dividing the corresponding component of this vector by the given scalar.


Divides the vector by a scalar value.


This function divides each component of the vector by the provided scalar value. It returns a new [**Vector4**](struct_a_g_e_1_1_vector4.md) with divided components.




**Parameters:**


* `scalar` The scalar value to divide the vector by. 



**Returns:**

A new [**Vector4**](struct_a_g_e_1_1_vector4.md) where each component is the corresponding component of this vector divided by the scalar. 





        

<hr>



### function operator/= 

_Divides the vector by a scalar value._ 
```C++
inline void AGE::Vector4::operator/= (
    float scalar
) 
```



This function divides each component of the vector (x, y, z, w) by the given scalar value. It modifies the original vector.




**Parameters:**


* `scalar` The scalar value to divide with.



**Returns:**

void


Divides the vector by a scalar value.


This function divides each component of the vector (x, y, z, w) by the given scalar value. It modifies the original vector.




**Parameters:**


* `scalar` The scalar value to divide with. Must not be zero to avoid division by zero. 




        

<hr>



### function operator= 

_Assigns the values of another_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _to this one._
```C++
inline Vector4 & AGE::Vector4::operator= (
    const Vector4 & Other
) 
```



This operator overload allows for assignment of the values from one [**Vector4**](struct_a_g_e_1_1_vector4.md) instance to another. The vector components (x, y, z, w) are set to match those of the Other parameter.




**Parameters:**


* `Other` A constant reference to a [**Vector4**](struct_a_g_e_1_1_vector4.md) object whose values will be copied into this one. 



**Returns:**

A reference to the modified [**Vector4**](struct_a_g_e_1_1_vector4.md) object for chaining operations. 





        

<hr>



### function operator= 

```C++
inline void AGE::Vector4::operator= (
    Vector3 & vec
) 
```




<hr>



### function operator== 

_Compares this_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _with another for equality._
```C++
inline bool AGE::Vector4::operator== (
    const Vector4 & vec
) const
```



The comparison is done component-wise, i.e., it checks if the x, y, z and w components of both vectors are equal.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to compare against. 



**Returns:**

True if all components are equal, false otherwise.


Compares this [**Vector4**](struct_a_g_e_1_1_vector4.md) with another for equality.


The function compares the x, y, z and w components of this [**Vector4**](struct_a_g_e_1_1_vector4.md) with those of the provided [**Vector4**](struct_a_g_e_1_1_vector4.md). If all four are equal, it returns true; otherwise, false is returned.




**Parameters:**


* `vec` The [**Vector4**](struct_a_g_e_1_1_vector4.md) to compare against.



**Returns:**

True if the vectors are identical in x, y, z and w components; False otherwise. 





        

<hr>



### function operator[] 

_This function returns a reference to the element at index 'i' in an array of float values._ 
```C++
inline float & AGE::Vector4::operator[] (
    int i
) 
```





**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A reference to the float value at position 'i'.


This function returns a reference to the element at index 'i' in an array of floats. 

**Parameters:**


* `i` The index of the element to return. 



**Returns:**

A reference to the float at position 'i'. If 'i' is out of bounds, it will throw an exception. 





        

<hr>



### function operator[] 

_Returns a reference to the element at index 'i' in an array of constant floats._ 
```C++
inline const float & AGE::Vector4::operator[] (
    int i
) const
```



This function returns a constant float reference that can be used for reading but not writing. The returned value is a reference to the i-th element of an internal array, where indices start from 0.




**Parameters:**


* `i` Index of the element in the array. Must be within the range [0, size of array - 1]. 



**Returns:**

Constant float reference to the i-th element of the array. 





        

<hr>



### function ~Vector4 

_Default destructor for the_ [_**Vector4**_](struct_a_g_e_1_1_vector4.md) _class._
```C++
AGE::Vector4::~Vector4 () = default
```



This function is responsible for releasing any resources that were acquired by the [**Vector4**](struct_a_g_e_1_1_vector4.md) object, such as memory or file handles. It does not perform any operations on the actual data stored in the vector.




**Returns:**

void 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Vector4.h`

