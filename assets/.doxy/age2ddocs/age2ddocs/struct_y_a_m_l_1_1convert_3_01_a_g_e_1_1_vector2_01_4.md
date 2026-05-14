

# Struct YAML::convert&lt; AGE::Vector2 &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::Vector2 &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_vector2_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, [**AGE::Vector2**](struct_a_g_e_1_1_vector2.md) & rhs) <br>_Decodes a Node object into an_ [_**AGE::Vector2**_](struct_a_g_e_1_1_vector2.md) _._ |
|  Node | [**encode**](#function-encode) (const [**AGE::Vector2**](struct_a_g_e_1_1_vector2.md) & rhs) <br>_Encodes a 2D vector into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an_ [_**AGE::Vector2**_](struct_a_g_e_1_1_vector2.md) _._
```C++
static inline bool YAML::convert< AGE::Vector2 >::decode (
    const Node & node,
    AGE::Vector2 & rhs
) 
```



This function attempts to decode the given Node object into an [**AGE::Vector2**](struct_a_g_e_1_1_vector2.md). It checks if the node is a sequence and has exactly two elements, then assigns the first element of the node as x value of the vector and the second one as y value. If the conditions are not met, it returns false.




**Parameters:**


* `node` The Node object to be decoded. 
* `rhs` The [**AGE::Vector2**](struct_a_g_e_1_1_vector2.md) that will store the decoded values. 



**Returns:**

True if the decoding was successful, False otherwise. 





        

<hr>



### function encode 

_Encodes a 2D vector into a Node object._ 
```C++
static inline Node YAML::convert< AGE::Vector2 >::encode (
    const AGE::Vector2 & rhs
) 
```



This function takes in a const reference to an [**AGE::Vector2**](struct_a_g_e_1_1_vector2.md) and encodes it into a Node object by pushing the x and y coordinates of the Vector2 onto the Node. The encoded Node is then returned.




**Parameters:**


* `rhs` The 2D vector to be encoded. 



**Returns:**

The encoded Node containing the x and y coordinates of the input Vector2. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

