

# Struct YAML::convert&lt; AGE::Ref&lt; AGE::AudioSource &gt; &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::Ref&lt; AGE::AudioSource &gt; &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_ref_3_01_a_g_e_1_1_audio_source_01_4_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, AGE::Ref&lt; [**AGE::AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & rhs) <br>_Decodes a Node object into an AGE::Ref&lt;AGE::AudioSource&gt;._  |
|  Node | [**encode**](#function-encode) (const AGE::Ref&lt; [**AGE::AudioSource**](class_a_g_e_1_1_audio_source.md) &gt; & rhs) <br>_Encodes an audio source into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an AGE::Ref&lt;AGE::AudioSource&gt;._ 
```C++
static inline bool YAML::convert< AGE::Ref< AGE::AudioSource > >::decode (
    const Node & node,
    AGE::Ref< AGE::AudioSource > & rhs
) 
```



This function takes in a const reference to a Node object and attempts to decode it into an instance of AGE::Ref&lt;AGE::AudioSource&gt;. If the node is not a sequence or if it's empty, the function returns false indicating failure. Otherwise, it sets rhs to the first element in the Node object and returns true.




**Parameters:**


* `node` The input Node object to be decoded. 
* `rhs` The output AGE::Ref&lt;AGE::AudioSource&gt; instance where the decoded data will be stored. 



**Returns:**

True if successful, false otherwise. 





        

<hr>



### function encode 

_Encodes an audio source into a Node object._ 
```C++
static inline Node YAML::convert< AGE::Ref< AGE::AudioSource > >::encode (
    const AGE::Ref< AGE::AudioSource > & rhs
) 
```



This function takes in a reference to an AudioSource and encodes it into a Node object. The encoded data is then pushed back onto the Node object.




**Parameters:**


* `rhs` A reference to an AudioSource that needs to be encoded. 



**Returns:**

Returns a Node object containing the encoded audio source. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

