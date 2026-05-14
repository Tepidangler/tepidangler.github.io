

# Struct YAML::convert&lt; AGE::AnimationSpecification &gt;

**template &lt;&gt;**



[**ClassList**](annotated.md) **>** [**YAML**](namespace_y_a_m_l.md) **>** [**convert&lt; AGE::AnimationSpecification &gt;**](struct_y_a_m_l_1_1convert_3_01_a_g_e_1_1_animation_specification_01_4.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  bool | [**decode**](#function-decode) (const Node & node, [**AGE::AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) & rhs) <br>_Decodes a Node object into an AnimationSpecification object._  |
|  Node | [**encode**](#function-encode) (const [**AGE::AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) & rhs) <br>_Encodes an AnimationSpecification object into a Node object._  |


























## Public Static Functions Documentation




### function decode 

_Decodes a Node object into an AnimationSpecification object._ 
```C++
static inline bool YAML::convert< AGE::AnimationSpecification >::decode (
    const Node & node,
    AGE::AnimationSpecification & rhs
) 
```



This function takes in a const reference to a Node object and a reference to an [**AGE::AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) object. It checks if the Node is a sequence and if it has any elements. If these conditions are not met, it returns false. Otherwise, it populates the AnimationSpecification with data from the Node. The function then returns true.




**Parameters:**


* `node` The const reference to the Node object to be decoded. 
* `rhs` The reference to the [**AGE::AnimationSpecification**](struct_a_g_e_1_1_animation_specification.md) object that will hold the decoded data.



**Returns:**

Returns true if the Node was successfully decoded, false otherwise. 





        

<hr>



### function encode 

_Encodes an AnimationSpecification object into a Node object._ 
```C++
static inline Node YAML::convert< AGE::AnimationSpecification >::encode (
    const AGE::AnimationSpecification & rhs
) 
```



This function takes an instance of the AnimationSpecification class and encodes it into a Node object, which is then returned by the function. The encoding process involves pushing back several properties of the AnimationSpecification object onto the Node object in specific order: Name, NumberOfFrames, MovementStatus (cast to int), Width, Height, TextureFilePath, and bIsReadyToLoad.




**Parameters:**


* `rhs` The AnimationSpecification object to be encoded. 



**Returns:**

A Node object containing the encoded data from the AnimationSpecification object. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Utils/Private/Serializers.cpp`

