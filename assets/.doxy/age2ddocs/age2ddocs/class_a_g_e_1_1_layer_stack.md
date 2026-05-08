

# Class AGE::LayerStack



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**LayerStack**](class_a_g_e_1_1_layer_stack.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  [**Layer**](class_a_g_e_1_1_layer.md) \* | [**GetLayerByName**](#function-getlayerbyname) (const std::string & LayerName) <br> |
|   | [**LayerStack**](#function-layerstack) () <br> |
|  void | [**PopLayer**](#function-poplayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br> |
|  void | [**PopOverlay**](#function-popoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Overlay) <br> |
|  void | [**PushLayer**](#function-pushlayer) ([**Layer**](class_a_g_e_1_1_layer.md) \* Layer) <br> |
|  void | [**PushOverlay**](#function-pushoverlay) ([**Layer**](class_a_g_e_1_1_layer.md) \* Overlay) <br> |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::iterator | [**begin**](#function-begin-12) () <br> |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br> |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::iterator | [**end**](#function-end-12) () <br> |
|  std::vector&lt; [**Layer**](class_a_g_e_1_1_layer.md) \* &gt;::const\_iterator | [**end**](#function-end-22) () const<br> |
|   | [**~LayerStack**](#function-layerstack) () <br> |




























## Public Functions Documentation




### function GetLayerByName 

```C++
Layer * AGE::LayerStack::GetLayerByName (
    const std::string & LayerName
) 
```




<hr>



### function LayerStack 

```C++
AGE::LayerStack::LayerStack () 
```




<hr>



### function PopLayer 

```C++
void AGE::LayerStack::PopLayer (
    Layer * Layer
) 
```




<hr>



### function PopOverlay 

```C++
void AGE::LayerStack::PopOverlay (
    Layer * Overlay
) 
```




<hr>



### function PushLayer 

```C++
void AGE::LayerStack::PushLayer (
    Layer * Layer
) 
```




<hr>



### function PushOverlay 

```C++
void AGE::LayerStack::PushOverlay (
    Layer * Overlay
) 
```




<hr>



### function begin [1/2]

```C++
inline std::vector< Layer * >::iterator AGE::LayerStack::begin () 
```




<hr>



### function begin [2/2]

```C++
inline std::vector< Layer * >::const_iterator AGE::LayerStack::begin () const
```




<hr>



### function end [1/2]

```C++
inline std::vector< Layer * >::iterator AGE::LayerStack::end () 
```




<hr>



### function end [2/2]

```C++
inline std::vector< Layer * >::const_iterator AGE::LayerStack::end () const
```




<hr>



### function ~LayerStack 

```C++
AGE::LayerStack::~LayerStack () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/LayerStack.h`

