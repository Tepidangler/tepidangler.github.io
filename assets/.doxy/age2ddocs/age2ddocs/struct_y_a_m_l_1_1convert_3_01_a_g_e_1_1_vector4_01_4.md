

# Struct YAML::convert&lt; AGE::Vector4 &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::Vector4 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector4_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, [**AGE::Vector4**](struct_a_g_e_1_1_vector4.md) & rhs) <br>_Decodes a Node object into an_ [_**AGE::Vector4**_](struct_a_g_e_1_1_vector4.md) _._ |
|  Node | [**encode**](#function-encode) (const [**AGE::Vector4**](struct_a_g_e_1_1_vector4.md) & rhs) <br>_Encodes a Vector4 into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an_ [_**AGE::Vector4**_](struct_a_g_e_1_1_vector4.md) _._
```C++
static inline bool YAML::convert< AGE::Vector4 >::decode (
    const Node & node,
    AGE::Vector4 & rhs
) 
```



This function takes in a const reference to a Node object and a reference to an [**AGE::Vector4**](struct_a_g_e_1_1_vector4.md). It checks if the node is a sequence and has exactly four elements. If it does, it assigns the first three elements of the node (interpreted as floats) to x, y, and z properties of the Vector4 respectively, and the fourth element to w property. The function returns true if the decoding was successful, false otherwise. 


        

<hr>



### function encode 

_Encodes a Vector4 into a Node object._ 
```C++
static inline Node YAML::convert< AGE::Vector4 >::encode (
    const AGE::Vector4 & rhs
) 
```



This function takes in a const reference to an [**AGE::Vector4**](struct_a_g_e_1_1_vector4.md) and encodes it into a Node object by pushing the x, y, z, and w values of the vector onto the node.




**Parameters:**


* `rhs` The input Vector4 to be encoded. 



**Returns:**

Returns a Node object containing the encoded data from the input Vector4. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

