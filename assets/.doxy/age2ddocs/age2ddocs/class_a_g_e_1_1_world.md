

# Class AGE::World



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**World**](class_a_g_e_1_1_world.md)










Inherited by the following classes: [AGE::World2D](class_a_g_e_1_1_world2_d.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](#function-as-12) () <br>_This function is currently not implemented and will always assert false. It returns a null pointer._  |
|  Wo rld2D \* | [**As**](#function-as-22) () <br>_This function returns a pointer to the derived class '_ [_**World2D**_](class_a_g_e_1_1_world2_d.md) _' from the base class '_[_**World**_](class_a_g_e_1_1_world.md) _'. It is used for polymorphism and dynamic binding. The returned object can be treated as an instance of_[_**World2D**_](class_a_g_e_1_1_world2_d.md) _._ |
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
|  Ref&lt; [**World**](class_a_g_e_1_1_world.md) &gt; | [**Create**](#function-create) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br>_Creates a new instance of the_ [_**World**_](class_a_g_e_1_1_world.md) _class._ |


























## Public Functions Documentation




### function As [1/2]

_This function is currently not implemented and will always assert false. It returns a null pointer._ 
```C++
template<typename T>
T * AGE::World::As () 
```





**Returns:**

nullptr Always.


This function is currently not implemented and will always assert false. It returns a null pointer.




**Returns:**

nullptr Always. 





        

<hr>



### function As [2/2]

_This function returns a pointer to the derived class '_ [_**World2D**_](class_a_g_e_1_1_world2_d.md) _' from the base class '_[_**World**_](class_a_g_e_1_1_world.md) _'. It is used for polymorphism and dynamic binding. The returned object can be treated as an instance of_[_**World2D**_](class_a_g_e_1_1_world2_d.md) _._
```C++
template<>
Wo rld2D * AGE::World::As () 
```





**Returns:**

A pointer to the derived class '[**World2D**](class_a_g_e_1_1_world2_d.md)'. 





        

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

_Creates a new instance of the_ [_**World**_](class_a_g_e_1_1_world.md) _class._
```C++
static Ref< World > AGE::World::Create (
    Ref< Scene > scene
) 
```



This function creates and returns a new instance of the [**World**](class_a_g_e_1_1_world.md) class, which is specialized for handling 2D scenes. The scene parameter specifies the [**Scene**](class_a_g_e_1_1_scene.md) that this world will be associated with.




**Parameters:**


* `scene` A reference to the [**Scene**](class_a_g_e_1_1_scene.md) object that this world will be associated with. 



**Returns:**

A reference to the newly created [**World**](class_a_g_e_1_1_world.md) instance.


Creates a new instance of the [**World**](class_a_g_e_1_1_world.md) class.


This function creates and returns a new instance of the [**World**](class_a_g_e_1_1_world.md) class, which is specialized for handling 2D scenes. The scene parameter specifies the [**Scene**](class_a_g_e_1_1_scene.md) that this world will be associated with.




**Parameters:**


* `scene` A reference to the [**Scene**](class_a_g_e_1_1_scene.md) object that this world will be associated with. 



**Returns:**

A reference to the newly created [**World**](class_a_g_e_1_1_world.md) instance. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Physics/Public/World.h`

