

# Class AGE::Physics2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Physics2D**](class_a_g_e_1_1_physics2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  b2BodyId | [**CreateBody**](#function-createbody) (b2BodyDef & Def) <br> |
|  b2Polygon | [**CreateBox**](#function-createbox) (float HeightX, float HeightY, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br> |
|  b2Capsule | [**CreateCapsule**](#function-createcapsule) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Offset, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale, const float Radius) <br> |
|  b2ShapeId | [**CreateCapsuleShape**](#function-createcapsuleshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Capsule & Capsule) <br> |
|  bool | [**CreateNewPhysicsWorld**](#function-createnewphysicsworld) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br> |
|  b2ShapeId | [**CreatePolygonShape**](#function-createpolygonshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Polygon & Box) <br> |
|  b2Segment | [**CreateSegment**](#function-createsegment) () <br> |
|  b2ShapeId | [**CreateSegmentShape**](#function-createsegmentshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Segment & Segment) <br> |
|  void | [**DestroyWorld**](#function-destroyworld) () <br> |
|  b2BodyId | [**GetBody**](#function-getbody) (const b2ShapeId & ID) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetBodyPosition**](#function-getbodyposition) (const b2BodyId & ID) <br> |
|  b2Capsule | [**GetCapsule**](#function-getcapsule) (const b2ShapeId & ID) <br> |
|  b2Polygon | [**GetPolygon**](#function-getpolygon) (const b2ShapeId & ID) <br> |
|  float | [**GetRotationAngle**](#function-getrotationangle) (const b2BodyId & ID) <br> |
|  void \* | [**GetUserData**](#function-getuserdata) (const b2ShapeId & ID) <br> |
|  Ref&lt; [**World**](class_a_g_e_1_1_world.md) &gt; & | [**GetWorld**](#function-getworld) () <br> |
|  b2BodyDef | [**MakeBodyDefinition**](#function-makebodydefinition) (const BodyType & Type, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, bool IsRotationFixed, void \* UserData) <br> |
|  b2Rot | [**MakeRotation**](#function-makerotation) (float Z) <br> |
|  b2ShapeDef | [**MakeShapeDefinition**](#function-makeshapedefinition) (float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void \* UserData) <br> |
|   | [**Physics2D**](#function-physics2d) () = default<br> |
|  void | [**QueryBoxOverlap**](#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br> |
|  void | [**QueryCapsuleOverlap**](#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br> |
|  bool | [**QueryHit**](#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br> |
|  void | [**QuerySegmentOverlap**](#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br> |
|  void | [**Step**](#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br> |
|   | [**~Physics2D**](#function-physics2d) () = default<br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  T | [**GetShapeFromID**](#function-getshapefromid) (b2ShapeId ID) <br> |


























## Public Functions Documentation




### function CreateBody 

```C++
b2BodyId AGE::Physics2D::CreateBody (
    b2BodyDef & Def
) 
```




<hr>



### function CreateBox 

```C++
b2Polygon AGE::Physics2D::CreateBox (
    float HeightX,
    float HeightY,
    const Vector3 & Scale
) 
```




<hr>



### function CreateCapsule 

```C++
b2Capsule AGE::Physics2D::CreateCapsule (
    const Vector2 & Offset,
    const Vector3 & Scale,
    const float Radius
) 
```




<hr>



### function CreateCapsuleShape 

```C++
b2ShapeId AGE::Physics2D::CreateCapsuleShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Capsule & Capsule
) 
```




<hr>



### function CreateNewPhysicsWorld 

```C++
bool AGE::Physics2D::CreateNewPhysicsWorld (
    Ref< Scene > scene
) 
```




<hr>



### function CreatePolygonShape 

```C++
b2ShapeId AGE::Physics2D::CreatePolygonShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Polygon & Box
) 
```




<hr>



### function CreateSegment 

```C++
b2Segment AGE::Physics2D::CreateSegment () 
```




<hr>



### function CreateSegmentShape 

```C++
b2ShapeId AGE::Physics2D::CreateSegmentShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Segment & Segment
) 
```




<hr>



### function DestroyWorld 

```C++
void AGE::Physics2D::DestroyWorld () 
```




<hr>



### function GetBody 

```C++
b2BodyId AGE::Physics2D::GetBody (
    const b2ShapeId & ID
) 
```




<hr>



### function GetBodyPosition 

```C++
Vector2 AGE::Physics2D::GetBodyPosition (
    const b2BodyId & ID
) 
```




<hr>



### function GetCapsule 

```C++
b2Capsule AGE::Physics2D::GetCapsule (
    const b2ShapeId & ID
) 
```




<hr>



### function GetPolygon 

```C++
b2Polygon AGE::Physics2D::GetPolygon (
    const b2ShapeId & ID
) 
```




<hr>



### function GetRotationAngle 

```C++
float AGE::Physics2D::GetRotationAngle (
    const b2BodyId & ID
) 
```




<hr>



### function GetUserData 

```C++
void * AGE::Physics2D::GetUserData (
    const b2ShapeId & ID
) 
```




<hr>



### function GetWorld 

```C++
inline Ref< World > & AGE::Physics2D::GetWorld () 
```




<hr>



### function MakeBodyDefinition 

```C++
b2BodyDef AGE::Physics2D::MakeBodyDefinition (
    const BodyType & Type,
    const Vector3 & Translation,
    const Vector3 & Rotation,
    bool IsRotationFixed,
    void * UserData
) 
```




<hr>



### function MakeRotation 

```C++
b2Rot AGE::Physics2D::MakeRotation (
    float Z
) 
```




<hr>



### function MakeShapeDefinition 

```C++
b2ShapeDef AGE::Physics2D::MakeShapeDefinition (
    float Density,
    float Friction,
    float Restitution,
    bool ShouldGenerateEvents,
    void * UserData
) 
```




<hr>



### function Physics2D 

```C++
AGE::Physics2D::Physics2D () = default
```




<hr>



### function QueryBoxOverlap 

```C++
void AGE::Physics2D::QueryBoxOverlap (
    const QueryParams & Params
) 
```




<hr>



### function QueryCapsuleOverlap 

```C++
void AGE::Physics2D::QueryCapsuleOverlap (
    const QueryParams & Params
) 
```




<hr>



### function QueryHit 

```C++
bool AGE::Physics2D::QueryHit (
    const QueryParams & Params
) 
```




<hr>



### function QuerySegmentOverlap 

```C++
void AGE::Physics2D::QuerySegmentOverlap (
    const QueryParams & Params
) 
```




<hr>



### function Step 

```C++
void AGE::Physics2D::Step (
    TimeStep DeltaTime
) 
```




<hr>



### function ~Physics2D 

```C++
AGE::Physics2D::~Physics2D () = default
```




<hr>
## Public Static Functions Documentation




### function GetShapeFromID 

```C++
template<typename T>
static inline T AGE::Physics2D::GetShapeFromID (
    b2ShapeId ID
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Physics/Public/Physics2D.h`

