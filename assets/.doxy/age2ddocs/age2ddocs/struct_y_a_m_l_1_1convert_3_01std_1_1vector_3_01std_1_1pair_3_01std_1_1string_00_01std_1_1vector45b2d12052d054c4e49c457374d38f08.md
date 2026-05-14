

# Struct YAML::convert&lt; std::vector&lt; std::pair&lt; std::string, std::vector&lt; uint8\_t &gt; &gt; &gt; &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; std::vector&lt; std::pair&lt; std::string, std::vector&lt; uint8\_t &gt; &gt; &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01std_1_1vector_3_01std_1_1pair_3_01std_1_1string_00_01std_1_1vector45b2d12052d054c4e49c457374d38f08.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, std::vector&lt; std::pair&lt; std::string, std::vector&lt; uint8\_t &gt; &gt; &gt; & rhs) <br>_Decodes a Node object into a vector of pairs._  |
|  Node | [**encode**](#function-encode) (const std::vector&lt; std::pair&lt; std::string, std::vector&lt; uint8\_t &gt; &gt; &gt; & rhs) <br>_Encodes a vector of pairs into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into a vector of pairs._ 
```C++
static inline bool YAML::convert< std::vector< std::pair< std::string, std::vector< uint8_t > > > >::decode (
    const Node & node,
    std::vector< std::pair< std::string, std::vector< uint8_t > > > & rhs
) 
```



This function takes in a const reference to a Node object and a reference to a std::vector of std::pair&lt;std::string, std::vector&lt;uint8\_t&gt;&gt;. It first resizes the output vector based on the size of the input node. Then it checks if the "second" field in the node is a sequence and has more than zero elements. If not, it returns false. Otherwise, it iterates over the node fields, extracting the "first" and "second" values into the output vector.




**Parameters:**


* `node` The Node object to be decoded. 
* `rhs` The std::vector of pairs where the decoded data will be stored.



**Returns:**

True if successful, false otherwise. 





        

<hr>



### function encode 

_Encodes a vector of pairs into a Node object._ 
```C++
static inline Node YAML::convert< std::vector< std::pair< std::string, std::vector< uint8_t > > > >::encode (
    const std::vector< std::pair< std::string, std::vector< uint8_t > > > & rhs
) 
```



This function takes in a vector of pairs, where each pair contains a string and a vector of uint8\_t values. It iterates over the input vector, assigning each pair's first element to the node as its key, and the second element to the node as its value. After processing all pairs, it returns the resulting Node object.




**Parameters:**


* `rhs` The vector of pairs to encode into a Node object. 



**Returns:**

The encoded Node object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

