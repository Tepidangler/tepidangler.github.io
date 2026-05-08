

# Class AGE::OpenGLPipeline



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md)








Inherits the following classes: [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Flush2D**](#function-flush2d) () override<br> |
|  void | [**GenerateDefaultTextures**](#function-generatedefaulttextures) () <br> |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](#function-getdata) () override<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](#function-getstats) () override<br> |
| virtual void | [**Init**](#function-init) () override<br> |
| virtual void | [**NextBatch2D**](#function-nextbatch2d) () override<br> |
|   | [**OpenGLPipeline**](#function-openglpipeline) () <br> |
| virtual void | [**ResetStats**](#function-resetstats) () override<br> |
| virtual void | [**StartBatch2D**](#function-startbatch2d) () override<br> |
|   | [**~OpenGLPipeline**](#function-openglpipeline) () override<br> |


## Public Functions inherited from AGE::Pipeline

See [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_pipeline.md#function-as-12) () <br> |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**As**](class_a_g_e_1_1_pipeline.md#function-as-22) () <br> |
| virtual void | [**Flush2D**](class_a_g_e_1_1_pipeline.md#function-flush2d) () = 0<br> |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](class_a_g_e_1_1_pipeline.md#function-getdata) () = 0<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](class_a_g_e_1_1_pipeline.md#function-getstats) () = 0<br> |
| virtual void | [**Init**](class_a_g_e_1_1_pipeline.md#function-init) () = 0<br> |
| virtual void | [**NextBatch2D**](class_a_g_e_1_1_pipeline.md#function-nextbatch2d) () = 0<br> |
| virtual void | [**ResetStats**](class_a_g_e_1_1_pipeline.md#function-resetstats) () = 0<br> |
| virtual void | [**StartBatch2D**](class_a_g_e_1_1_pipeline.md#function-startbatch2d) () = 0<br> |
| virtual  | [**~Pipeline**](class_a_g_e_1_1_pipeline.md#function-pipeline) () = default<br> |




## Public Static Functions inherited from AGE::Pipeline

See [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**Pipeline**](class_a_g_e_1_1_pipeline.md) &gt; | [**Create**](class_a_g_e_1_1_pipeline.md#function-create) () <br> |


















































## Public Functions Documentation




### function Flush2D 

```C++
virtual void AGE::OpenGLPipeline::Flush2D () override
```



Implements [*AGE::Pipeline::Flush2D*](class_a_g_e_1_1_pipeline.md#function-flush2d)


<hr>



### function GenerateDefaultTextures 

```C++
void AGE::OpenGLPipeline::GenerateDefaultTextures () 
```




<hr>



### function GetData 

```C++
virtual Renderer2DData & AGE::OpenGLPipeline::GetData () override
```



Implements [*AGE::Pipeline::GetData*](class_a_g_e_1_1_pipeline.md#function-getdata)


<hr>



### function GetStats 

```C++
virtual Statistics & AGE::OpenGLPipeline::GetStats () override
```



Implements [*AGE::Pipeline::GetStats*](class_a_g_e_1_1_pipeline.md#function-getstats)


<hr>



### function Init 

```C++
virtual void AGE::OpenGLPipeline::Init () override
```



Implements [*AGE::Pipeline::Init*](class_a_g_e_1_1_pipeline.md#function-init)


<hr>



### function NextBatch2D 

```C++
virtual void AGE::OpenGLPipeline::NextBatch2D () override
```



Implements [*AGE::Pipeline::NextBatch2D*](class_a_g_e_1_1_pipeline.md#function-nextbatch2d)


<hr>



### function OpenGLPipeline 

```C++
AGE::OpenGLPipeline::OpenGLPipeline () 
```




<hr>



### function ResetStats 

```C++
virtual void AGE::OpenGLPipeline::ResetStats () override
```



Implements [*AGE::Pipeline::ResetStats*](class_a_g_e_1_1_pipeline.md#function-resetstats)


<hr>



### function StartBatch2D 

```C++
virtual void AGE::OpenGLPipeline::StartBatch2D () override
```



Implements [*AGE::Pipeline::StartBatch2D*](class_a_g_e_1_1_pipeline.md#function-startbatch2d)


<hr>



### function ~OpenGLPipeline 

```C++
AGE::OpenGLPipeline::~OpenGLPipeline () override
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLPipeline.h`

