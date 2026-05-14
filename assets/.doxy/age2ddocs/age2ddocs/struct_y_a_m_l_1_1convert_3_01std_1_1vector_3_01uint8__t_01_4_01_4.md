

# Struct YAML::convert&lt; std::vector&lt; uint8\_t &gt; &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; std::vector&lt; uint8\_t &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01std_1_1vector_3_01uint8__t_01_4_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, std::vector&lt; uint8\_t &gt; & rhs) <br>_Decodes a Node object into an std::vector of uint8\_t values._  |
|  Node | [**encode**](#function-encode) (const std::vector&lt; uint8\_t &gt; & rhs) <br>_Encodes a vector of uint8\_t into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an std::vector of uint8\_t values._ 
```C++
static inline bool YAML::convert< std::vector< uint8_t > >::decode (
    const Node & node,
    std::vector< uint8_t > & rhs
) 
```



This function takes in a const reference to a Node object and a reference to an std::vector of unsigned char (uint8\_t). It checks if the node is a sequence and its size is greater than zero, returning false otherwise. If the check passes, it resizes the vector to match the size of the node and populates it with uint8\_t values obtained by converting each string element in the Node object to an unsigned char. It then returns true indicating successful decoding.




**Parameters:**


* `node` The input Node object to be decoded. 
* `rhs` The output vector of uint8\_t values.



**Returns:**

True if the function successfully decodes the Node, false otherwise. 





        

<hr>



### function encode 

_Encodes a vector of uint8\_t into a Node object._ 
```C++
static inline Node YAML::convert< std::vector< uint8_t > >::encode (
    const std::vector< uint8_t > & rhs
) 
```



This function takes an input vector of uint8\_t and encodes it into a Node object by assigning each element of the vector to a corresponding index in the Node object. The encoding is done using a for loop, where each element from the input vector is assigned to a position in the Node object.




**Parameters:**


* `rhs` A const reference to an std::vector&lt;uint8\_t&gt; that needs to be encoded into a Node object. 



**Returns:**

Returns a Node object which contains the encoded data from the input vector. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

