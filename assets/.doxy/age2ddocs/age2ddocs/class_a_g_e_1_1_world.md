

# Class AGE::World



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**World**](class_a_g_e_1_1_world.md)










Inherited by the following classes: [AGE::World2D](class_a_g_e_1_1_world2_d.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br> |
|  [**World2D**](class_a_g_e_1_1_world2_d.md) \* | [**As**](#function-as-22) () <br> |
| virtual void | [**DestroyWorld**](#function-destroyworld) () = 0<br> |
| virtual void | [**MakeDefaultQueryFilter**](#function-makedefaultqueryfilter) () = 0<br> |
| virtual void | [**QueryBoxOverlap**](#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QueryCapsuleOverlap**](#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QueryHit**](#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QuerySegmentOverlap**](#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**Step**](#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) = 0<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**World**](class_a_g_e_1_1_world.md) &gt; | [**Create**](#function-create) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br> |


























## Public Functions Documentation




### function As [1/2]

```C++
template<typename T>
T * AGE::World::As () 
```




<hr>



### function As [2/2]

```C++
template<>
World2D * AGE::World::As () 
```




<hr>



### function DestroyWorld 

```C++
virtual void AGE::World::DestroyWorld () = 0
```




<hr>



### function MakeDefaultQueryFilter 

```C++
virtual void AGE::World::MakeDefaultQueryFilter () = 0
```




<hr>



### function QueryBoxOverlap 

```C++
virtual void AGE::World::QueryBoxOverlap (
    const QueryParams & Params
) = 0
```




<hr>



### function QueryCapsuleOverlap 

```C++
virtual void AGE::World::QueryCapsuleOverlap (
    const QueryParams & Params
) = 0
```




<hr>



### function QueryHit 

```C++
virtual void AGE::World::QueryHit (
    const QueryParams & Params
) = 0
```




<hr>



### function QuerySegmentOverlap 

```C++
virtual void AGE::World::QuerySegmentOverlap (
    const QueryParams & Params
) = 0
```




<hr>



### function Step 

```C++
virtual void AGE::World::Step (
    TimeStep DeltaTime
) = 0
```




<hr>
## Public Static Functions Documentation




### function Create 

```C++
static Ref< World > AGE::World::Create (
    Ref< Scene > scene
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Physics/Public/World.h`

