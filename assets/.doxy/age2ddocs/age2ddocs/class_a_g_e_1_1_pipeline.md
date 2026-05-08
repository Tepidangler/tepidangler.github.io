

# Class AGE::Pipeline



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Pipeline**](class_a_g_e_1_1_pipeline.md)










Inherited by the following classes: [AGE::OpenGLPipeline](class_a_g_e_1_1_open_g_l_pipeline.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br> |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**As**](#function-as-22) () <br> |
| virtual void | [**Flush2D**](#function-flush2d) () = 0<br> |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](#function-getdata) () = 0<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](#function-getstats) () = 0<br> |
| virtual void | [**Init**](#function-init) () = 0<br> |
| virtual void | [**NextBatch2D**](#function-nextbatch2d) () = 0<br> |
| virtual void | [**ResetStats**](#function-resetstats) () = 0<br> |
| virtual void | [**StartBatch2D**](#function-startbatch2d) () = 0<br> |
| virtual  | [**~Pipeline**](#function-pipeline) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**Pipeline**](class_a_g_e_1_1_pipeline.md) &gt; | [**Create**](#function-create) () <br> |


























## Public Functions Documentation




### function As [1/2]

```C++
template<typename T>
T * AGE::Pipeline::As () 
```




<hr>



### function As [2/2]

```C++
template<>
OpenGLPipeline * AGE::Pipeline::As () 
```




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

```C++
virtual AGE::Pipeline::~Pipeline () = default
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Scope< Pipeline > AGE::Pipeline::Create () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Render/Public/Pipeline.h`

