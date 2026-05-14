

# Class AGE::OpenGLPipeline



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md)








Inherits the following classes: [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual void | [**Flush2D**](#function-flush2d) () override<br> |
|  void | [**GenerateDefaultTextures**](#function-generatedefaulttextures) () <br>_GenerateDefaultTextures is a function that creates and initializes default textures for the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _object._ |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](#function-getdata) () override<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](#function-getstats) () override<br>_Get the statistics of the OpenGL_ [_**Pipeline**_](class_a_g_e_1_1_pipeline.md) _._ |
| virtual void | [**Init**](#function-init) () override<br> |
| virtual void | [**NextBatch2D**](#function-nextbatch2d) () override<br>_This function is used to start the next batch of 2D rendering. It first flushes any existing 2D data by calling Flush2D(), and then starts a new batch with_ [_**StartBatch2D()**_](class_a_g_e_1_1_open_g_l_pipeline.md#function-startbatch2d) _._ |
|   | [**OpenGLPipeline**](#function-openglpipeline) () <br>[_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _is a class that represents an OpenGL pipeline. It provides methods for setting up and managing the rendering process in an OpenGL context._ |
| virtual void | [**ResetStats**](#function-resetstats) () override<br>_Resets the statistics of the OpenGL pipeline._  |
| virtual void | [**StartBatch2D**](#function-startbatch2d) () override<br>_Resets the buffers for rendering operations in the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _class._ |
|   | [**~OpenGLPipeline**](#function-openglpipeline) () override<br>_Destructor for the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _class._ |


## Public Functions inherited from AGE::Pipeline

See [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_pipeline.md#function-as-12) () <br>_This function is currently not implemented and will always throw an assertion error. It returns a null pointer of type T\*. The purpose of this function is unknown._  |
|  [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) \* | [**As**](class_a_g_e_1_1_pipeline.md#function-as-22) () <br>_This function returns a pointer to the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _object._ |
| virtual void | [**Flush2D**](class_a_g_e_1_1_pipeline.md#function-flush2d) () = 0<br> |
| virtual [**Renderer2DData**](struct_a_g_e_1_1_renderer2_d_data.md) & | [**GetData**](class_a_g_e_1_1_pipeline.md#function-getdata) () = 0<br> |
| virtual [**Statistics**](struct_a_g_e_1_1_statistics.md) & | [**GetStats**](class_a_g_e_1_1_pipeline.md#function-getstats) () = 0<br> |
| virtual void | [**Init**](class_a_g_e_1_1_pipeline.md#function-init) () = 0<br> |
| virtual void | [**NextBatch2D**](class_a_g_e_1_1_pipeline.md#function-nextbatch2d) () = 0<br> |
| virtual void | [**ResetStats**](class_a_g_e_1_1_pipeline.md#function-resetstats) () = 0<br> |
| virtual void | [**StartBatch2D**](class_a_g_e_1_1_pipeline.md#function-startbatch2d) () = 0<br> |
| virtual  | [**~Pipeline**](class_a_g_e_1_1_pipeline.md#function-pipeline) () = default<br>_Virtual destructor for the_ [_**Pipeline**_](class_a_g_e_1_1_pipeline.md) _class._ |




## Public Static Functions inherited from AGE::Pipeline

See [AGE::Pipeline](class_a_g_e_1_1_pipeline.md)

| Type | Name |
| ---: | :--- |
|  Scope&lt; [**Pipeline**](class_a_g_e_1_1_pipeline.md) &gt; | [**Create**](class_a_g_e_1_1_pipeline.md#function-create) () <br>_Creates a new pipeline based on the current_ [_**RendererAPI**_](class_a_g_e_1_1_renderer_a_p_i.md) _._ |


















































## Public Functions Documentation




### function Flush2D 

```C++
virtual void AGE::OpenGLPipeline::Flush2D () override
```



Implements [*AGE::Pipeline::Flush2D*](class_a_g_e_1_1_pipeline.md#function-flush2d)


<hr>



### function GenerateDefaultTextures 

_GenerateDefaultTextures is a function that creates and initializes default textures for the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _object._
```C++
void AGE::OpenGLPipeline::GenerateDefaultTextures () 
```



This function generates a white texture with full alpha channel (0xffffffff) and sets it as the WhiteTexture member of the m\_Data struct. The [**Texture2D::Create()**](class_a_g_e_1_1_texture2_d.md#function-create-15) function is used to create the texture, and the SetData() method is called on the created texture to initialize its data.




**Returns:**

void No return value.


GenerateDefaultTextures is a function that generates default textures for the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) class.


This function creates a white texture and sets it as the default texture data member of the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) object. The white texture is represented by a 32-bit unsigned integer with all its bits set to 1, which corresponds to color (255, 255, 255, 255) in RGBA format.




**Returns:**

void No return value. 





        

<hr>



### function GetData 

```C++
virtual Renderer2DData & AGE::OpenGLPipeline::GetData () override
```



Implements [*AGE::Pipeline::GetData*](class_a_g_e_1_1_pipeline.md#function-getdata)


<hr>



### function GetStats 

_Get the statistics of the OpenGL_ [_**Pipeline**_](class_a_g_e_1_1_pipeline.md) _._
```C++
virtual Statistics & AGE::OpenGLPipeline::GetStats () override
```



This function returns a reference to the statistics object that holds information about the performance and usage of the OpenGL [**Pipeline**](class_a_g_e_1_1_pipeline.md). The returned [**Statistics**](struct_a_g_e_1_1_statistics.md) object can be used for various purposes such as profiling, debugging or optimizing the rendering process.




**Returns:**

A reference to the [**Statistics**](struct_a_g_e_1_1_statistics.md) object.


Get the statistics of the OpenGL [**Pipeline**](class_a_g_e_1_1_pipeline.md).


This function returns a reference to the statistics object that holds information about the performance and usage of the OpenGL pipeline.




**Returns:**

A reference to the [**Statistics**](struct_a_g_e_1_1_statistics.md) object. 





        
Implements [*AGE::Pipeline::GetStats*](class_a_g_e_1_1_pipeline.md#function-getstats)


<hr>



### function Init 

```C++
virtual void AGE::OpenGLPipeline::Init () override
```



Implements [*AGE::Pipeline::Init*](class_a_g_e_1_1_pipeline.md#function-init)


<hr>



### function NextBatch2D 

_This function is used to start the next batch of 2D rendering. It first flushes any existing 2D data by calling Flush2D(), and then starts a new batch with_ [_**StartBatch2D()**_](class_a_g_e_1_1_open_g_l_pipeline.md#function-startbatch2d) _._
```C++
virtual void AGE::OpenGLPipeline::NextBatch2D () override
```





**Returns:**

void


This function is used to prepare for the next batch of 2D rendering. It first flushes any existing 2D data by calling Flush2D(), and then starts a new batch with [**StartBatch2D()**](class_a_g_e_1_1_open_g_l_pipeline.md#function-startbatch2d).




**Returns:**

void 





        
Implements [*AGE::Pipeline::NextBatch2D*](class_a_g_e_1_1_pipeline.md#function-nextbatch2d)


<hr>



### function OpenGLPipeline 

[_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _is a class that represents an OpenGL pipeline. It provides methods for setting up and managing the rendering process in an OpenGL context._
```C++
AGE::OpenGLPipeline::OpenGLPipeline () 
```




<hr>



### function ResetStats 

_Resets the statistics of the OpenGL pipeline._ 
```C++
virtual void AGE::OpenGLPipeline::ResetStats () override
```



This function sets all fields in the [**Statistics**](struct_a_g_e_1_1_statistics.md) structure to zero using memset(). It effectively resets the counters for various statistics tracked by the OpenGL pipeline.




**Returns:**

void


Resets the statistics of the OpenGL pipeline.


This function sets all fields in the [**Statistics**](struct_a_g_e_1_1_statistics.md) structure to zero using memset(). It effectively resets the counters and other statistics that track performance over time.




**Returns:**

void 





        
Implements [*AGE::Pipeline::ResetStats*](class_a_g_e_1_1_pipeline.md#function-resetstats)


<hr>



### function StartBatch2D 

_Resets the buffers for rendering operations in the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _class._
```C++
virtual void AGE::OpenGLPipeline::StartBatch2D () override
```





**Parameters:**


* `None` 



**Returns:**

None 





        
Implements [*AGE::Pipeline::StartBatch2D*](class_a_g_e_1_1_pipeline.md#function-startbatch2d)


<hr>



### function ~OpenGLPipeline 

_Destructor for the_ [_**OpenGLPipeline**_](class_a_g_e_1_1_open_g_l_pipeline.md) _class._
```C++
AGE::OpenGLPipeline::~OpenGLPipeline () override
```



This function is responsible for cleaning up memory that was dynamically allocated during the lifetime of an instance of this class. It deletes four arrays (QuadVertexBufferBase, CircleVertexBufferBase, LineVertexBufferBase, TextVertexBufferBase) and clears a vector (TileVertexBufferBases).




**Returns:**

void


Destructor for the [**OpenGLPipeline**](class_a_g_e_1_1_open_g_l_pipeline.md) class. It is responsible for freeing up memory that was allocated dynamically during its lifetime.


This destructor deletes four arrays (QuadVertexBufferBase, CircleVertexBufferBase, LineVertexBufferBase and TextVertexBufferBase) which were previously allocated using new[]. Additionally, it clears the TileVertexBufferBases vector to free up memory. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Platform/OpenGL/Public/OpenGLPipeline.h`

