

# Class AGE::LayerStack



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**LayerStack**](class_a_g_e_1_1_layer_stack.md)



_A class for managing layers in a stack-like structure._ [More...](#detailed-description)

* `#include <LayerStack.h>`





















## Public Attributes

| Type | Name |
| ---: | :--- |
|  COMMENT | [**\_\_pad0\_\_**](#variable-__pad0__)  <br>_Returns an iterator pointing to the beginning of the Layers vector._  |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Layer**](class_a_g_e_1_1_layer.md) \* | [**GetLayerByName**](#function-getlayerbyname) (const std::string & LayerName) <br>_This function is used to get a layer by its name._  |
|   | [**LayerStack**](#function-layerstack) () <br>[_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _is a class that manages layers in a stack-like structure. It provides methods for pushing, popping and managing the layers._ |
|  void | [**PopLayer**](#function-poplayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br>_This function is used to remove a layer from the_ [_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _. It calls the OnDetach() method of the provided layer, then it searches for that layer in the m\_Layers vector and removes it if found. The index where this layer was inserted into the stack is also decremented by one._ |
|  void | [**PopOverlay**](#function-popoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Overlay) <br>_This function is used to remove an overlay from the layer stack._  |
|  void | [**PushLayer**](#function-pushlayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br>_Pushes a layer onto the stack at the specified position._  |
|  void | [**PushOverlay**](#function-pushoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Overlay) <br>_Pushes an overlay layer onto the stack._  |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::iterator | [**begin**](#function-begin-12) () <br> |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br>_Returns a constant iterator pointing to the beginning of the layers vector._  |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::iterator | [**end**](#function-end-12) () <br>_Returns an iterator pointing to the theoretical element that follows the last element of the vector._  |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::const\_iterator | [**end**](#function-end-22) () const<br>_Returns a constant iterator pointing to the past-the-end element of the layer vector._  |
|   | [**~LayerStack**](#function-layerstack) () <br>_Destructor for the_ [_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _class. This function is responsible for deleting all layers in the stack, freeing up memory that was previously allocated to them. It uses a range-based for loop to iterate over each layer and deletes it using the delete keyword._ |




























## Detailed Description


The [**LayerStack**](class_a_g_e_1_1_layer_stack.md) class provides methods to push, pop and get layers by name. It also supports iteration over the layers using iterators. 


    
## Public Attributes Documentation




### variable \_\_pad0\_\_ 

_Returns an iterator pointing to the beginning of the Layers vector._ 
```C++
COMMENT AGE::LayerStack::__pad0__;
```





**Returns:**

An iterator pointing to the start of the Layers vector. If no layers exist, returns an iterator equal to [**end()**](class_a_g_e_1_1_layer_stack.md#function-end-12). 





        

<hr>
## Public Functions Documentation




### function GetLayerByName 

_This function is used to get a layer by its name._ 
```C++
Layer * AGE::LayerStack::GetLayerByName (
    const std::string & LayerName
) 
```



The function iterates over the layers in the stack and returns the first one whose name matches the input string. If no such layer exists, it returns nullptr.




**Parameters:**


* `LayerName` A const reference to a std::string representing the name of the layer we are looking for. 



**Returns:**

Pointer to [**Layer**](class_a_g_e_1_1_layer.md) if found, otherwise nullptr.


This function is used to get a layer by its name. 

**Parameters:**


* `LayerName` The name of the layer that we want to find. 



**Returns:**

Returns a pointer to the found layer if it exists, otherwise returns nullptr. 





        

<hr>



### function LayerStack 

[_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _is a class that manages layers in a stack-like structure. It provides methods for pushing, popping and managing the layers._
```C++
AGE::LayerStack::LayerStack () 
```



[**LayerStack**](class_a_g_e_1_1_layer_stack.md) is a class that manages layers in a stack-like structure. It provides methods for pushing, popping and managing layers. 


        

<hr>



### function PopLayer 

_This function is used to remove a layer from the_ [_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _. It calls the OnDetach() method of the provided layer, then it searches for that layer in the m\_Layers vector and removes it if found. The index where this layer was inserted into the stack is also decremented by one._
```C++
void AGE::LayerStack::PopLayer (
    Layer * Layer
) 
```





**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the layer that needs to be removed from the stack.

Pop a layer from the stack and detach it.


This function removes a specified [**Layer**](class_a_g_e_1_1_layer.md) object from the [**LayerStack**](class_a_g_e_1_1_layer_stack.md) by calling its OnDetach() method, then erases it from the m\_Layers vector. The index of insertion is also decremented to reflect this removal. 

**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the layer that needs to be removed. 




        

<hr>



### function PopOverlay 

_This function is used to remove an overlay from the layer stack._ 
```C++
void AGE::LayerStack::PopOverlay (
    Layer * Overlay
) 
```





**Parameters:**


* `Overlay` Pointer to the [**Layer**](class_a_g_e_1_1_layer.md) object that needs to be removed.



**Returns:**

void


This function is used to remove an overlay from the layer stack.




**Parameters:**


* `Overlay` Pointer to the [**Layer**](class_a_g_e_1_1_layer.md) object that needs to be removed.



**Returns:**

void No return value. 





        

<hr>



### function PushLayer 

_Pushes a layer onto the stack at the specified position._ 
```C++
void AGE::LayerStack::PushLayer (
    Layer * Layer
) 
```



This function inserts a new layer into the [**LayerStack**](class_a_g_e_1_1_layer_stack.md) at the specified index, effectively pushing it to the top of the rendering order. The layer is inserted before all existing layers. If no index is provided, it defaults to the end of the stack (top).




**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the layer that should be pushed onto the stack.



**Returns:**

void No return value.


Pushes a layer onto the stack at the specified index.


This function inserts a new layer into the [**LayerStack**](class_a_g_e_1_1_layer_stack.md) at the position indicated by m\_LayerInsertIndex. The layer is inserted before all existing layers with lower indices, and its index in the stack increases by one.




**Parameters:**


* [**Layer**](class_a_g_e_1_1_layer.md) Pointer to the layer that will be pushed onto the stack. 



**Returns:**

void No return value. 





        

<hr>



### function PushOverlay 

_Pushes an overlay layer onto the stack._ 
```C++
void AGE::LayerStack::PushOverlay (
    Layer * Overlay
) 
```



This function adds a new layer to the top of the [**LayerStack**](class_a_g_e_1_1_layer_stack.md), making it visible and interactive. The layer is added at the end of the m\_Layers vector, so it will be rendered on top of all other layers.




**Parameters:**


* `Overlay` Pointer to the overlay layer that should be pushed onto the stack. 



**Returns:**

void No return value.


Pushes an overlay layer onto the stack.


This function adds a new layer to the top of the [**LayerStack**](class_a_g_e_1_1_layer_stack.md), making it visible and interactive. The layer is added at the end of the m\_Layers vector, so it will be rendered on top of all other layers.




**Parameters:**


* `Overlay` Pointer to the overlay layer that should be pushed onto the stack. 




        

<hr>



### function begin [1/2]

```C++
inline std::vector< Layer * >::iterator AGE::LayerStack::begin () 
```




<hr>



### function begin [2/2]

_Returns a constant iterator pointing to the beginning of the layers vector._ 
```C++
inline std::vector< Layer * >::const_iterator AGE::LayerStack::begin () const
```





**Returns:**

A constant iterator to the start of the layers vector.


Returns a constant iterator pointing to the beginning of the layers vector. 

**Returns:**

A constant iterator pointing to the first element in the layers vector, or end if the layers vector is empty. 





        

<hr>



### function end [1/2]

_Returns an iterator pointing to the theoretical element that follows the last element of the vector._ 
```C++
inline std::vector< Layer * >::iterator AGE::LayerStack::end () 
```





**Returns:**

An iterator to the theoretical element following the last element of the vector.


Returns an iterator pointing to the theoretical element past the last element of the container. 

**Returns:**

An iterator to the theoretical element past the end of the sequence of elements in the container. 





        

<hr>



### function end [2/2]

_Returns a constant iterator pointing to the past-the-end element of the layer vector._ 
```C++
inline std::vector< Layer * >::const_iterator AGE::LayerStack::end () const
```



This function returns a constant iterator that points to one position past the last element in the layer vector. It is used to indicate the end of the sequence of elements in the container, similar to how std::vector's member functions cend() return an iterator pointing to the past-the-end element.




**Returns:**

A constant iterator pointing to the past-the-end element.


Returns a constant iterator pointing to the past-the-end element of the layers vector. 

**Returns:**

A constant iterator pointing to the past-the-end element in the layers vector. 





        

<hr>



### function ~LayerStack 

_Destructor for the_ [_**LayerStack**_](class_a_g_e_1_1_layer_stack.md) _class. This function is responsible for deleting all layers in the stack, freeing up memory that was previously allocated to them. It uses a range-based for loop to iterate over each layer and deletes it using the delete keyword._
```C++
AGE::LayerStack::~LayerStack () 
```



Destructor for the [**LayerStack**](class_a_g_e_1_1_layer_stack.md) class. This function is responsible for deleting all layers in the stack when an instance of the class is destroyed. It uses a range-based for loop to iterate over each layer and deletes it using 'delete'. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/LayerStack.h`

