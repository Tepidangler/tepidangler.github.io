

# Class AGE::GraphicsContext



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md)










Inherited by the following classes: [AGE::OpenGLContext](class_a_g_e_1_1_open_g_l_context.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br>_This function is a placeholder for future use. It currently always asserts false and returns null._  |
|  [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) \* | [**As**](#function-as-22) () <br>_This function returns a pointer to the OpenGL context associated with this instance of_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _._ |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual void | [**SwapBuffers**](#function-swapbuffers) () = 0<br> |
| virtual  | [**~GraphicsContext**](#function-graphicscontext) () <br>_Virtual destructor for the_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) &gt; | [**Create**](#function-create) (void \* Window) <br>_Creates a graphics context based on the current renderer API._  |


























## Public Functions Documentation




### function As [1/2]

_This function is a placeholder for future use. It currently always asserts false and returns null._ 
```C++
template<typename T>
T * AGE::GraphicsContext::As () 
```





**Parameters:**


* `None` 



**Returns:**

T\* Returns nullptr.


This function is currently not implemented and will always throw an assertion. It returns a pointer of type T\*, which in this case is unknown to the documentation. The function does not take any parameters. In future, it should be implemented to cast the [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) instance to another derived class if possible. 

**Returns:**

A nullptr as per current implementation. 





        

<hr>



### function As [2/2]

_This function returns a pointer to the OpenGL context associated with this instance of_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _._
```C++
template<>
OpenGLContext * AGE::GraphicsContext::As () 
```





**Returns:**

Pointer to an [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md) object, or nullptr if no such context exists.


This function returns a pointer to the OpenGL context associated with this [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) object. 

**Returns:**

A pointer to an [**OpenGLContext**](class_a_g_e_1_1_open_g_l_context.md), or nullptr if no such context exists. 





        

<hr>



### function Init 

```C++
virtual void AGE::GraphicsContext::Init () = 0
```




<hr>



### function SwapBuffers 

```C++
virtual void AGE::GraphicsContext::SwapBuffers () = 0
```




<hr>



### function ~GraphicsContext 

_Virtual destructor for the_ [_**GraphicsContext**_](class_a_g_e_1_1_graphics_context.md) _class._
```C++
inline virtual AGE::GraphicsContext::~GraphicsContext () 
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or GPU handles. It does not return anything and thus has an empty return type (void).


Virtual destructor for the [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or graphics contexts. It does not return anything and thus has an empty return type (void). 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a graphics context based on the current renderer API._ 
```C++
static Scope< GraphicsContext > AGE::GraphicsContext::Create (
    void * Window
) 
```



This function creates and returns a Scope of [**GraphicsContext**](class_a_g_e_1_1_graphics_context.md) which is initialized according to the currently set [**Renderer**](class_a_g_e_1_1_renderer.md) API. If no valid API is set, it asserts false and returns nullptr. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/GraphicsContext.h`

