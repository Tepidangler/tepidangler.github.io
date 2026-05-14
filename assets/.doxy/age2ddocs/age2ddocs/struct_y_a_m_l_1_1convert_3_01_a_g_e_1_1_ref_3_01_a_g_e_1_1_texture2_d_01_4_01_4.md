

# Struct YAML::convert&lt; AGE::Ref&lt; AGE::Texture2D &gt; &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::Ref&lt; AGE::Texture2D &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_ref_3_01_a_g_e_1_1_texture2_d_01_4_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, AGE::Ref&lt; [**AGE::Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & rhs) <br>_Decodes a Node object into an AGE::Ref&lt;AGE::Texture2D&gt;._  |
|  Node | [**encode**](#function-encode) (const AGE::Ref&lt; [**AGE::Texture2D**](class_a_g_e_1_1_texture2_d.md) &gt; & rhs) <br>_Encodes a texture into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an AGE::Ref&lt;AGE::Texture2D&gt;._ 
```C++
static inline bool YAML::convert< AGE::Ref< AGE::Texture2D > >::decode (
    const Node & node,
    AGE::Ref< AGE::Texture2D > & rhs
) 
```



This function checks if the input node is a sequence and has exactly one element. If it does, it attempts to convert that single element into an AGE::Ref&lt;AGE::Texture2D&gt; and assigns it to rhs. The function returns true on success and false otherwise.




**Parameters:**


* `node` The Node object to decode. 
* `rhs` The AGE::Ref&lt;AGE::Texture2D&gt; to store the result in. 



**Returns:**

True if the decoding was successful, false otherwise. 





        

<hr>



### function encode 

_Encodes a texture into a Node object._ 
```C++
static inline Node YAML::convert< AGE::Ref< AGE::Texture2D > >::encode (
    const AGE::Ref< AGE::Texture2D > & rhs
) 
```



This function takes a reference to an [**AGE::Texture2D**](class_a_g_e_1_1_texture2_d.md) object and encodes it into a Node object. The encoded data is then pushed back onto the node.




**Parameters:**


* `rhs` Reference to the Texture2D object to be encoded. 



**Returns:**

Encoded texture as a Node object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

