

# Struct YAML::convert&lt; AGE::Vector3 &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::Vector3 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector3_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) & rhs) <br>_Decodes a Node object into an_ [_**AGE::Vector3**_](struct_a_g_e_1_1_vector3.md) _object._ |
|  Node | [**encode**](#function-encode) (const [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) & rhs) <br>_Encodes a Vector3 object into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an_ [_**AGE::Vector3**_](struct_a_g_e_1_1_vector3.md) _object._
```C++
static inline bool YAML::convert< AGE::Vector3 >::decode (
    const Node & node,
    AGE::Vector3 & rhs
) 
```



This function takes in a const reference to a Node object and a reference to an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) object. It checks if the Node is a sequence (i.e., it contains elements) and has exactly three elements. If these conditions are met, it assigns the first element of the Node to rhs.x, the second to rhs.y, and the third to rhs.z. The function returns true if all operations were successful, false otherwise.




**Parameters:**


* `node` A const reference to a Node object that should be decoded into an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) object. 
* `rhs` A reference to an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) object where the result of the decoding will be stored.



**Returns:**

Returns true if successful, false otherwise. 





        

<hr>



### function encode 

_Encodes a Vector3 object into a Node object._ 
```C++
static inline Node YAML::convert< AGE::Vector3 >::encode (
    const AGE::Vector3 & rhs
) 
```



This function takes in a const reference to an [**AGE::Vector3**](struct_a_g_e_1_1_vector3.md) object and encodes it into a Node object by pushing the x, y, and z values of the vector onto the node. The encoded Node is then returned. 

**Parameters:**


* `rhs` The Vector3 object to be encoded. 



**Returns:**

The encoded Node object containing the x, y, and z values from the input Vector3. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

