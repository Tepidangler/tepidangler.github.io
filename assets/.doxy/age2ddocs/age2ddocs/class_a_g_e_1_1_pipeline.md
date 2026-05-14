

# Class AGE::Pipeline



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Pipeline**](class_a_g_e_1_1_pipeline.md)










Inherited by the following classes: [AGE::OpenGLPipeline](class_a_g_e_1_1_open_g_l_pipeline.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br>_This function is currently not implemented and will always throw an assertion error. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**As**](#function-as-22) () <br>_This function returns a pointer to the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _object._ |
| virtual void | [**Flush2D**](#function-flush2d) () = 0<br> |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](#function-getdata) () = 0<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](#function-getstats) () = 0<br> |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual void | [**NextBatch2D**](#function-nextbatch2d) () = 0<br> |
| virtual void | [**ResetStats**](#function-resetstats) () = 0<br> |
| virtual void | [**StartBatch2D**](#function-startbatch2d) () = 0<br> |
| virtual  | [**~Pipeline**](#function-pipeline) () = default<br>_Virtual destructor for the_ [_**Pipeline**_](class_a_g_e_1_1_pipeline.md) _class._ |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**Pipeline**](class_a_g_e_1_1_pipeline.md) &gt; | [**Create**](#function-create) () <br>_Creates a new pipeline based on the current_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._ |


























## Public Functions Documentation




### function As [1/2]

_This function is currently not implemented and will always throw an assertion error. It returns a null pointer of type T\*. The purpose of this function is unknown._ 
```C++
template<typename T>
T * AGE::Pipeline::As () 
```





**Returns:**

A null pointer of type T\*


This function is currently not implemented and will always throw an assertion error. It returns a null pointer of type T\*. The purpose of this function is unknown.




**Returns:**

A null pointer of type T\* 





        

<hr>



### function As [2/2]

_This function returns a pointer to the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _object._
```C++
template<>
OpenGLPipeline * AGE::Pipeline::As () 
```



The function is used to cast the current instance of [**Pipeline**](class_a_g_e_1_1_pipeline.md) to an [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) type. It does this by returning 'this' as a void pointer, then casting it back to an [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) pointer. This allows for polymorphism in OpenGL operations where different types of objects can respond differently to the same function calls.




**Returns:**

A pointer to the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object. If no such object exists, returns nullptr.


This function returns a pointer to an [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object.


The function is used to convert the current object into an [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) type. It does this by returning 'this' casted as an OpenGLPipeline\*.




**Returns:**

An instance of [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md). 





        

<hr>



### function Flush2D 

```C++
virtual void AGE::Pipeline::Flush2D () = 0
```




<hr>



### function GetData 

```C++
virtual Renderer2DData & AGE::Pipeline::GetData () = 0
```




<hr>



### function GetStats 

```C++
virtual Statistics & AGE::Pipeline::GetStats () = 0
```




<hr>



### function Init 

```C++
virtual void AGE::Pipeline::Init () = 0
```




<hr>



### function NextBatch2D 

```C++
virtual void AGE::Pipeline::NextBatch2D () = 0
```




<hr>



### function ResetStats 

```C++
virtual void AGE::Pipeline::ResetStats () = 0
```




<hr>



### function StartBatch2D 

```C++
virtual void AGE::Pipeline::StartBatch2D () = 0
```




<hr>



### function ~Pipeline 

_Virtual destructor for the_ [_**Pipeline**_](class_a_g_e_1_1_pipeline.md) _class._
```C++
virtual AGE::Pipeline::~Pipeline () = default
```



This function is responsible for releasing any resources that were acquired by the object during its lifetime. It does not return anything and thus, it has a void return type.


Virtual destructor for the [**Pipeline**](class_a_g_e_1_1_pipeline.md) class.


This function is responsible for releasing any resources that were acquired by the pipeline during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>
## Public Static Functions Documentation




### function Create 

_Creates a new pipeline based on the current_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._
```C++
static Scope< Pipeline > AGE::Pipeline::Create () 
```



This function creates and returns a new [**Pipeline**](class_a_g_e_1_1_pipeline.md) object that is specific to the currently used [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md). The type of [**Pipeline**](class_a_g_e_1_1_pipeline.md) created depends on which API is in use at the time this function is called. If no valid [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is detected, nullptr is returned.




**Returns:**

Scope&lt;Pipeline&gt; A new pipeline or nullptr if no valid [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) was found.


Creates a new [**Pipeline**](class_a_g_e_1_1_pipeline.md) instance based on the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md).


This function checks the currently set [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) and creates an appropriate pipeline for it. If the API is not recognized, nullptr is returned.




**Returns:**

Scope&lt;Pipeline&gt; A smart pointer to a new [**Pipeline**](class_a_g_e_1_1_pipeline.md) instance or nullptr if the current [**RendererAPI**](class_a_g_e_1_1_renderer_a_p_i.md) is unrecognized. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Pipeline.h`

