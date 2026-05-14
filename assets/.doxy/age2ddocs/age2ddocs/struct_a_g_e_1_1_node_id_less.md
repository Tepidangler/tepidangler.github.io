

# Struct AGE::NodeIdLess



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**NodeIdLess**](struct_a_g_e_1_1_node_id_less.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  bool | [**operator()**](#function-operator) (const ax::NodeEditor::NodeId & lhs, const ax::NodeEditor::NodeId rhs) const<br>_Compares two NodeIds for less than comparison._  |




























## Public Functions Documentation




### function operator() 

_Compares two NodeIds for less than comparison._ 
```C++
inline bool AGE::NodeIdLess::operator() (
    const ax::NodeEditor::NodeId & lhs,
    const ax::NodeEditor::NodeId rhs
) const
```



This function compares the underlying pointers of two NodeId objects and returns true if the pointer of lhs is less than that of rhs, otherwise it returns false.




**Parameters:**


* `lhs` The first NodeId to compare. 
* `rhs` The second NodeId to compare. 



**Returns:**

True if the pointer of lhs is less than that of rhs, False otherwise.


Compares two NodeIds for less than comparison.


This function compares the underlying pointers of two NodeId objects and returns true if the left hand side is less than the right hand side, otherwise it returns false.




**Parameters:**


* `lhs` The first NodeId to compare. 
* `rhs` The second NodeId to compare. 



**Returns:**

True if lhs &lt; rhs, False otherwise. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/VisualScripting/Public/VisualScriptingStructs.h`

