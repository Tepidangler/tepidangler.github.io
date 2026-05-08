

# Class AGE::World2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**World2D**](class_a_g_e_1_1_world2_d.md)








Inherits the following classes: [AGE::World](class_a_g_e_1_1_world.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  b2BodyId | [**CreateBody**](#function-createbody) (b2BodyDef & Def) <br> |
|  b2Polygon | [**CreateBox**](#function-createbox) (float HeightX, float HeightY, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br> |
|  b2Capsule | [**CreateCapsule**](#function-createcapsule) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Offset, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale, const float Radius) <br> |
|  b2ShapeId | [**CreateCapsuleShape**](#function-createcapsuleshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Capsule & Capsule) <br> |
|  b2ShapeId | [**CreatePolygonShape**](#function-createpolygonshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Polygon & Box) <br> |
|  b2Segment | [**CreateSegment**](#function-createsegment) () <br> |
|  b2ShapeId | [**CreateSegmentShape**](#function-createsegmentshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Segment & Segment) <br> |
| virtual void | [**DestroyWorld**](#function-destroyworld) () override<br> |
|  b2BodyId | [**GetBody**](#function-getbody) (const b2ShapeId & ID) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetBodyPosition**](#function-getbodyposition) (const b2BodyId & ID) <br> |
|  b2Capsule | [**GetCapsule**](#function-getcapsule) (const b2ShapeId & ID) <br> |
|  b2Polygon | [**GetPolygon**](#function-getpolygon) (const b2ShapeId & ID) <br> |
|  b2QueryFilter & | [**GetQueryFilter**](#function-getqueryfilter) () <br> |
|  float | [**GetRotationAngle**](#function-getrotationangle) (const b2BodyId & ID) <br> |
|  void \* | [**GetUserData**](#function-getuserdata) (const b2ShapeId & ID) <br> |
|  b2WorldId & | [**GetWorld**](#function-getworld) () <br> |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; & | [**GetWorldScene**](#function-getworldscene) () <br> |
|  b2BodyDef | [**MakeBodyDefinition**](#function-makebodydefinition) (const BodyType & Type, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, bool IsRotationFixed, void \* UserData) <br> |
| virtual void | [**MakeDefaultQueryFilter**](#function-makedefaultqueryfilter) () override<br> |
|  b2Rot | [**MakeRotation**](#function-makerotation) (float Z) <br> |
|  b2ShapeDef | [**MakeShapeDefinition**](#function-makeshapedefinition) (float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void \* UserData) <br> |
| virtual void | [**QueryBoxOverlap**](#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**QueryCapsuleOverlap**](#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**QueryHit**](#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**QuerySegmentOverlap**](#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**Step**](#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br> |
|   | [**World2D**](#function-world2d) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br> |
| virtual  | [**~World2D**](#function-world2d) () <br> |


## Public Functions inherited from AGE::World

See [AGE::World](class_a_g_e_1_1_world.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_world.md#function-as-12) () <br> |
|  [**World2D**](class_a_g_e_1_1_world2_d.md) \* | [**As**](class_a_g_e_1_1_world.md#function-as-22) () <br> |
| virtual void | [**DestroyWorld**](class_a_g_e_1_1_world.md#function-destroyworld) () = 0<br> |
| virtual void | [**MakeDefaultQueryFilter**](class_a_g_e_1_1_world.md#function-makedefaultqueryfilter) () = 0<br> |
| virtual void | [**QueryBoxOverlap**](class_a_g_e_1_1_world.md#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QueryCapsuleOverlap**](class_a_g_e_1_1_world.md#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QueryHit**](class_a_g_e_1_1_world.md#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**QuerySegmentOverlap**](class_a_g_e_1_1_world.md#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) = 0<br> |
| virtual void | [**Step**](class_a_g_e_1_1_world.md#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) = 0<br> |




## Public Static Functions inherited from AGE::World

See [AGE::World](class_a_g_e_1_1_world.md)

| Type | Name |
| ---: | :--- |
|  Ref&lt; [**World**](class_a_g_e_1_1_world.md) &gt; | [**Create**](class_a_g_e_1_1_world.md#function-create) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br> |


















































## Public Functions Documentation




### function CreateBody 

```C++
b2BodyId AGE::World2D::CreateBody (
    b2BodyDef & Def
) 
```




<hr>



### function CreateBox 

```C++
b2Polygon AGE::World2D::CreateBox (
    float HeightX,
    float HeightY,
    const Vector3 & Scale
) 
```




<hr>



### function CreateCapsule 

```C++
b2Capsule AGE::World2D::CreateCapsule (
    const Vector2 & Offset,
    const Vector3 & Scale,
    const float Radius
) 
```




<hr>



### function CreateCapsuleShape 

```C++
b2ShapeId AGE::World2D::CreateCapsuleShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Capsule & Capsule
) 
```




<hr>



### function CreatePolygonShape 

```C++
b2ShapeId AGE::World2D::CreatePolygonShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Polygon & Box
) 
```




<hr>



### function CreateSegment 

```C++
b2Segment AGE::World2D::CreateSegment () 
```




<hr>



### function CreateSegmentShape 

```C++
b2ShapeId AGE::World2D::CreateSegmentShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Segment & Segment
) 
```




<hr>



### function DestroyWorld 

```C++
virtual void AGE::World2D::DestroyWorld () override
```



Implements [*AGE::World::DestroyWorld*](class_a_g_e_1_1_world.md#function-destroyworld)


<hr>



### function GetBody 

```C++
b2BodyId AGE::World2D::GetBody (
    const b2ShapeId & ID
) 
```




<hr>



### function GetBodyPosition 

```C++
Vector2 AGE::World2D::GetBodyPosition (
    const b2BodyId & ID
) 
```




<hr>



### function GetCapsule 

```C++
b2Capsule AGE::World2D::GetCapsule (
    const b2ShapeId & ID
) 
```




<hr>



### function GetPolygon 

```C++
b2Polygon AGE::World2D::GetPolygon (
    const b2ShapeId & ID
) 
```




<hr>



### function GetQueryFilter 

```C++
inline b2QueryFilter & AGE::World2D::GetQueryFilter () 
```




<hr>



### function GetRotationAngle 

```C++
float AGE::World2D::GetRotationAngle (
    const b2BodyId & ID
) 
```




<hr>



### function GetUserData 

```C++
void * AGE::World2D::GetUserData (
    const b2ShapeId & ID
) 
```




<hr>



### function GetWorld 

```C++
b2WorldId & AGE::World2D::GetWorld () 
```




<hr>



### function GetWorldScene 

```C++
Ref< Scene > & AGE::World2D::GetWorldScene () 
```




<hr>



### function MakeBodyDefinition 

```C++
b2BodyDef AGE::World2D::MakeBodyDefinition (
    const BodyType & Type,
    const Vector3 & Translation,
    const Vector3 & Rotation,
    bool IsRotationFixed,
    void * UserData
) 
```




<hr>



### function MakeDefaultQueryFilter 

```C++
virtual void AGE::World2D::MakeDefaultQueryFilter () override
```



Implements [*AGE::World::MakeDefaultQueryFilter*](class_a_g_e_1_1_world.md#function-makedefaultqueryfilter)


<hr>



### function MakeRotation 

```C++
b2Rot AGE::World2D::MakeRotation (
    float Z
) 
```




<hr>



### function MakeShapeDefinition 

```C++
b2ShapeDef AGE::World2D::MakeShapeDefinition (
    float Density,
    float Friction,
    float Restitution,
    bool ShouldGenerateEvents,
    void * UserData
) 
```




<hr>



### function QueryBoxOverlap 

```C++
virtual void AGE::World2D::QueryBoxOverlap (
    const QueryParams & Params
) override
```



Implements [*AGE::World::QueryBoxOverlap*](class_a_g_e_1_1_world.md#function-queryboxoverlap)


<hr>



### function QueryCapsuleOverlap 

```C++
virtual void AGE::World2D::QueryCapsuleOverlap (
    const QueryParams & Params
) override
```



Implements [*AGE::World::QueryCapsuleOverlap*](class_a_g_e_1_1_world.md#function-querycapsuleoverlap)


<hr>



### function QueryHit 

```C++
virtual void AGE::World2D::QueryHit (
    const QueryParams & Params
) override
```



Implements [*AGE::World::QueryHit*](class_a_g_e_1_1_world.md#function-queryhit)


<hr>



### function QuerySegmentOverlap 

```C++
virtual void AGE::World2D::QuerySegmentOverlap (
    const QueryParams & Params
) override
```



Implements [*AGE::World::QuerySegmentOverlap*](class_a_g_e_1_1_world.md#function-querysegmentoverlap)


<hr>



### function Step 

```C++
virtual void AGE::World2D::Step (
    TimeStep DeltaTime
) override
```



Implements [*AGE::World::Step*](class_a_g_e_1_1_world.md#function-step)


<hr>



### function World2D 

```C++
AGE::World2D::World2D (
    Ref< Scene > scene
) 
```




<hr>



### function ~World2D 

```C++
virtual AGE::World2D::~World2D () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Physics/Public/World2D.h`

