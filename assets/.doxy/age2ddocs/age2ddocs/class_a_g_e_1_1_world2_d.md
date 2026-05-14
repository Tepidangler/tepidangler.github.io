

# Class AGE::World2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**World2D**](class_a_g_e_1_1_world2_d.md)








Inherits the following classes: [AGE::World](class_a_g_e_1_1_world.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|  b2BodyId | [**CreateBody**](#function-createbody) (b2BodyDef & Def) <br>_Creates a body in the world._  |
|  b2Polygon | [**CreateBox**](#function-createbox) (float HeightX, float HeightY, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br>_Creates a box polygon with given dimensions and scale._  |
|  b2Capsule | [**CreateCapsule**](#function-createcapsule) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Offset, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale, const float Radius) <br>_Creates a capsule shape with the given parameters._  |
|  b2ShapeId | [**CreateCapsuleShape**](#function-createcapsuleshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Capsule & Capsule) <br>_Creates a capsule shape for the given body._  |
|  b2ShapeId | [**CreatePolygonShape**](#function-createpolygonshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Polygon & Box) <br>_Creates a polygon shape for the given body._  |
|  b2Segment | [**CreateSegment**](#function-createsegment) () <br>_Creates a new segment with default values._  |
|  b2ShapeId | [**CreateSegmentShape**](#function-createsegmentshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Segment & Segment) <br>_Creates a segment shape in the world._  |
| virtual void | [**DestroyWorld**](#function-destroyworld) () override<br>_Destroys the Box2D world object._  |
|  b2BodyId | [**GetBody**](#function-getbody) (const b2ShapeId & ID) <br>_Retrieves the body associated with a given shape id._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetBodyPosition**](#function-getbodyposition) (const b2BodyId & ID) <br>_Gets the position of a body in the world._  |
|  b2Capsule | [**GetCapsule**](#function-getcapsule) (const b2ShapeId & ID) <br>_Retrieves a capsule from the world using its shape id._  |
|  b2Polygon | [**GetPolygon**](#function-getpolygon) (const b2ShapeId & ID) <br>_Retrieves a polygon associated with the given shape id._  |
|  b2QueryFilter & | [**GetQueryFilter**](#function-getqueryfilter) () <br>_Returns a reference to the query filter object used by this class._  |
|  float | [**GetRotationAngle**](#function-getrotationangle) (const b2BodyId & ID) <br>_Get the rotation angle of a body in degrees._  |
|  void \* | [**GetUserData**](#function-getuserdata) (const b2ShapeId & ID) <br>_Retrieves the user data associated with a specific shape id._  |
|  b2WorldId & | [**GetWorld**](#function-getworld) () <br>_Returns a reference to the world object._  |
|  Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; & | [**GetWorldScene**](#function-getworldscene) () <br>_Get the reference to the world scene object._  |
|  b2BodyDef | [**MakeBodyDefinition**](#function-makebodydefinition) (const BodyType & Type, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, bool IsRotationFixed, void \* UserData) <br>_Creates a body definition for the Box2D physics engine._  |
| virtual void | [**MakeDefaultQueryFilter**](#function-makedefaultqueryfilter) () override<br>_Sets the query filter to its default state._  |
|  b2Rot | [**MakeRotation**](#function-makerotation) (float Z) <br>_Creates a rotation object from an angle in radians._  |
|  b2ShapeDef | [**MakeShapeDefinition**](#function-makeshapedefinition) (float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void \* UserData) <br>_Creates a ShapeDefinition for use in Box2D physics engine._  |
| virtual void | [**QueryBoxOverlap**](#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**QueryCapsuleOverlap**](#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**QueryHit**](#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br>_This function is used to perform a ray-casting operation in the 2D world. It takes as input a_ [_**QueryParams**_](struct_a_g_e_1_1_query_params.md) _object that contains information about the point of origin and the location where the ray should be casted, as well as other parameters for the query. The function returns an id representing the result of the hit query._ |
| virtual void | [**QuerySegmentOverlap**](#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) override<br> |
| virtual void | [**Step**](#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) override<br>_Performs a single step of the simulation._  |
|   | [**World2D**](#function-world2d) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br> |
| virtual  | [**~World2D**](#function-world2d) () <br> |


## Public Functions inherited from AGE::World

See [AGE::World](class_a_g_e_1_1_world.md)

| Type | Name |
| ---: | :--- |
|  T \* | [**As**](class_a_g_e_1_1_world.md#function-as-12) () <br>_This function is currently not implemented and will always assert false. It returns a null pointer._  |
|  Wo rld2D \* | [**As**](class_a_g_e_1_1_world.md#function-as-22) () <br>_This function returns a pointer to the derived class '_ [_**World2D**_](class_a_g_e_1_1_world2_d.md) _' from the base class '_[_**World**_](class_a_g_e_1_1_world.md) _'. It is used for polymorphism and dynamic binding. The returned object can be treated as an instance of_[_**World2D**_](class_a_g_e_1_1_world2_d.md) _._ |
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
|  Ref&lt; [**World**](class_a_g_e_1_1_world.md) &gt; | [**Create**](class_a_g_e_1_1_world.md#function-create) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br>_Creates a new instance of the_ [_**World**_](class_a_g_e_1_1_world.md) _class._ |


















































## Public Functions Documentation




### function CreateBody 

_Creates a body in the world._ 
```C++
b2BodyId AGE::World2D::CreateBody (
    b2BodyDef & Def
) 
```



This function creates a new rigid body for simulation. A definition is passed to it specifying properties of the body such as its position, angle, linear velocity, angular velocity etc.




**Parameters:**


* `Def` The definition of the body to be created. 



**Returns:**

BodyId Identifier for the newly created body. 





        

<hr>



### function CreateBox 

_Creates a box polygon with given dimensions and scale._ 
```C++
b2Polygon AGE::World2D::CreateBox (
    float HeightX,
    float HeightY,
    const Vector3 & Scale
) 
```



This function creates a box polygon with the specified height in x-direction (HeightX), y-direction (HeightY) and the provided scale factor for both directions. The resulting Polygon is then returned by the function.




**Parameters:**


* `HeightX` The half width of the box, scaled by Scale.x. 
* `HeightY` The half height of the box, scaled by Scale.y. 
* `Scale` A scaling factor for both directions.



**Returns:**

Polygon The resulting polygon after applying the scale factors to the dimensions. 





        

<hr>



### function CreateCapsule 

_Creates a capsule shape with the given parameters._ 
```C++
b2Capsule AGE::World2D::CreateCapsule (
    const Vector2 & Offset,
    const Vector3 & Scale,
    const float Radius
) 
```



This function creates a capsule shape by setting its center points and radius based on the provided offset, scale, and radius values. The centers are calculated as (Offset.x \* Scale.x, Offset.y \* Scale.y) for both ends of the capsule.




**Parameters:**


* `Offset` The offset to use when calculating the center points. 
* `Scale` The scale to use when calculating the center points and radius. 
* `Radius` The radius of the capsule.



**Returns:**

A b2Capsule object representing a capsule shape with the specified parameters. 





        

<hr>



### function CreateCapsuleShape 

_Creates a capsule shape for the given body._ 
```C++
b2ShapeId AGE::World2D::CreateCapsuleShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Capsule & Capsule
) 
```



This function creates and adds a capsule shape to the specified body with the provided fixture definition and capsule parameters. The function returns an identifier for the newly created shape, which can be used to manipulate or query this shape later on.




**Parameters:**


* `ID` Identifier of the body to add the shape to. 
* `Fixture` Definition of the fixture (e.&lt;｜begin▁of▁sentence｜&gt;cifics like density and restitution) to apply to the shape. 
* `Capsule` Parameters defining the capsule's size and orientation.



**Returns:**

Identifier for the newly created shape. 





        

<hr>



### function CreatePolygonShape 

_Creates a polygon shape for the given body._ 
```C++
b2ShapeId AGE::World2D::CreatePolygonShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Polygon & Box
) 
```



This function creates a polygon shape with the specified definition and box for the body identified by ID. The fixture and box parameters are used to define the properties of the new shape.




**Parameters:**


* `ID` The identifier of the body for which the shape is being created. 
* `Fixture` A reference to the fixture definition that will be applied to the new shape. 
* `Box` A reference to the polygon box that defines the vertices of the new shape.



**Returns:**

Returns a ShapeId representing the newly created shape. 





        

<hr>



### function CreateSegment 

_Creates a new segment with default values._ 
```C++
b2Segment AGE::World2D::CreateSegment () 
```



This function creates and returns a Segment object with its start point at (0,0) and end point at (1,0). The Segment is initialized in the world coordinate system.




**Returns:**

A Segment object with default values. 





        

<hr>



### function CreateSegmentShape 

_Creates a segment shape in the world._ 
```C++
b2ShapeId AGE::World2D::CreateSegmentShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Segment & Segment
) 
```



This function creates a new segment shape within the physics engine and associates it with a body. The segment is defined by two points, forming a line segment.




**Parameters:**


* `ID` The identifier of the body to which the segment shape should be associated. 
* `Fixture` A structure defining the properties of the segment shape. 
* `Segment` A structure specifying the endpoints of the segment.



**Returns:**

Returns a unique identifier for the newly created segment shape. 





        

<hr>



### function DestroyWorld 

_Destroys the Box2D world object._ 
```C++
virtual void AGE::World2D::DestroyWorld () override
```



This function is used to destroy the Box2D world object, which was previously created using World2D::CreateWorld(). It calls b2DestroyWorld() on the m\_World member variable of the class instance.




**Returns:**

void 





        
Implements [*AGE::World::DestroyWorld*](class_a_g_e_1_1_world.md#function-destroyworld)


<hr>



### function GetBody 

_Retrieves the body associated with a given shape id._ 
```C++
b2BodyId AGE::World2D::GetBody (
    const b2ShapeId & ID
) 
```



This function takes in a const reference to an object of type `b2ShapeId`, which represents the unique identifier for a physics shape. It then returns the corresponding `BodyId` representing the body that owns this shape.




**Parameters:**


* `ID` A constant reference to the shape id. 



**Returns:**

The body associated with the given shape id. If no such body exists, an unknown value is returned. 





        

<hr>



### function GetBodyPosition 

_Gets the position of a body in the world._ 
```C++
Vector2 AGE::World2D::GetBodyPosition (
    const b2BodyId & ID
) 
```



This function retrieves the current position of a body within the 2D world using its unique ID. The returned value is a [**Vector2**](struct_a_g_e_1_1_vector2.md) representing the x and y coordinates of the body's position.




**Parameters:**


* `ID` Unique identifier for the body whose position we want to retrieve. 



**Returns:**

A [**Vector2**](struct_a_g_e_1_1_vector2.md) containing the x and y coordinates of the specified body's position. 





        

<hr>



### function GetCapsule 

_Retrieves a capsule from the world using its shape id._ 
```C++
b2Capsule AGE::World2D::GetCapsule (
    const b2ShapeId & ID
) 
```



This function is used to retrieve a capsule object from the world by providing the unique ID of the capsule's shape. The function uses the b2Shape\_GetCapsule() method to get the capsule with the given ID.




**Parameters:**


* `ID` Unique identifier for the capsule shape in the [**World2D**](class_a_g_e_1_1_world2_d.md) object. 



**Returns:**

A Capsule object corresponding to the provided shape id. 





        

<hr>



### function GetPolygon 

_Retrieves a polygon associated with the given shape id._ 
```C++
b2Polygon AGE::World2D::GetPolygon (
    const b2ShapeId & ID
) 
```



This function takes an argument of type `b2ShapeId` and returns a Polygon object. It uses the `b2Shape_GetPolygon()` function to get the polygon based on the provided ID. The returned value is expected to be used for rendering or other geometric operations in the 2D [**World**](class_a_g_e_1_1_world.md).




**Parameters:**


* `ID` A constant reference to an instance of `b2ShapeId`, which represents a unique identifier for a shape. 



**Returns:**

Polygon object representing the polygon associated with the provided shape id. 





        

<hr>



### function GetQueryFilter 

_Returns a reference to the query filter object used by this class._ 
```C++
inline b2QueryFilter & AGE::World2D::GetQueryFilter () 
```





**Returns:**

A reference to the b2QueryFilter object.


Returns a reference to the query filter object used by this class. 

**Returns:**

A reference to the b2QueryFilter object. 





        

<hr>



### function GetRotationAngle 

_Get the rotation angle of a body in degrees._ 
```C++
float AGE::World2D::GetRotationAngle (
    const b2BodyId & ID
) 
```



This function retrieves the rotation angle of a body with a given ID, converting it from radians to degrees using [**Math::Degrees()**](class_a_g_e_1_1_math.md#function-degrees-12). The b2Rot\_GetAngle() and b2Body\_GetRotation() functions are used for this purpose.




**Parameters:**


* `ID` Unique identifier for the body whose rotation angle is being retrieved.



**Returns:**

The rotation angle of the specified body in degrees. 





        

<hr>



### function GetUserData 

_Retrieves the user data associated with a specific shape id._ 
```C++
void * AGE::World2D::GetUserData (
    const b2ShapeId & ID
) 
```



This function retrieves the user data that was previously set using World2D::SetUserData() for a given b2ShapeId. The returned pointer can be used to access any custom data associated with this shape.




**Parameters:**


* `ID` The unique identifier of the shape whose user data is being retrieved. 



**Returns:**

Pointer to the user data, or nullptr if no user data was set for the given shape id. 





        

<hr>



### function GetWorld 

_Returns a reference to the world object._ 
```C++
b2WorldId & AGE::World2D::GetWorld () 
```



This function returns a reference to the world object that is currently being used by the [**World2D**](class_a_g_e_1_1_world2_d.md) class. The returned reference can be used to modify or access the properties of this world object.




**Returns:**

A reference to the current world object. 





        

<hr>



### function GetWorldScene 

_Get the reference to the world scene object._ 
```C++
Ref< Scene > & AGE::World2D::GetWorldScene () 
```



This function returns a reference to the world scene object, which is an instance of the [**Scene**](class_a_g_e_1_1_scene.md) class. The purpose of this function is to provide access to the current state of the world scene for other parts of the program that need it.




**Returns:**

f&lt;Scene&gt;& A reference to the world scene object. 





        

<hr>



### function MakeBodyDefinition 

_Creates a body definition for the Box2D physics engine._ 
```C++
b2BodyDef AGE::World2D::MakeBodyDefinition (
    const BodyType & Type,
    const Vector3 & Translation,
    const Vector3 & Rotation,
    bool IsRotationFixed,
    void * UserData
) 
```



This function creates and returns a b2BodyDef object, which is used to define properties of a rigid body in the Box2D physics engine. The returned BodyDef has its userData set to the provided UserData pointer, its type set based on the given Type parameter, its position set to Translation, and its rotation set to Rotation. It also sets the fixedRotation flag according to IsRotationFixed.




**Parameters:**


* `Type` The type of body to be created. This is used to determine how the body behaves in the physics simulation. 
* `Translation` A [**Vector3**](struct_a_g_e_1_1_vector3.md) specifying the initial position of the body. 
* `Rotation` A [**Vector3**](struct_a_g_e_1_1_vector3.md) specifying the initial rotation of the body, in radians. 
* `IsRotationFixed` A boolean indicating whether the body's rotation should be fixed or not. 
* `UserData` A void pointer to user data that can be associated with the body. This is typically used for game-specific data.



**Returns:**

The created b2BodyDef object, ready to be passed to a Box2D physics engine function to create a new rigid body. 





        

<hr>



### function MakeDefaultQueryFilter 

_Sets the query filter to its default state._ 
```C++
virtual void AGE::World2D::MakeDefaultQueryFilter () override
```



This function resets the internal query filter of the [**World2D**](class_a_g_e_1_1_world2_d.md) object back to its initial, default state. The m\_QueryFilter member variable is set using b2DefaultQueryFilter(), which presumably returns a default query filter for Box2D physics engine.




**Returns:**

void 





        
Implements [*AGE::World::MakeDefaultQueryFilter*](class_a_g_e_1_1_world.md#function-makedefaultqueryfilter)


<hr>



### function MakeRotation 

_Creates a rotation object from an angle in radians._ 
```C++
b2Rot AGE::World2D::MakeRotation (
    float Z
) 
```



This function takes an angle in radians as input and returns a Rotation object representing that angle. The returned Rotation object can be used for various 2D transformations.




**Parameters:**


* `Z` The angle in radians to convert into a rotation object. 



**Returns:**

A Rotation object representing the input angle. 





        

<hr>



### function MakeShapeDefinition 

_Creates a ShapeDefinition for use in Box2D physics engine._ 
```C++
b2ShapeDef AGE::World2D::MakeShapeDefinition (
    float Density,
    float Friction,
    float Restitution,
    bool ShouldGenerateEvents,
    void * UserData
) 
```



This function creates and returns a ShapeDefinition object that can be used to define the properties of a fixture in the Box2D physics engine. The returned object is initialized with default values, which are then overridden by the parameters provided.




**Parameters:**


* `Density` The density of the shape. This value will determine how much mass the shape has. 
* `Friction` A coefficient that determines how much the surface roughness affects the friction between this fixture and another. 
* `Restitution` A factor determining the bounciness of the object when it hits something. 
* `ShouldGenerateEvents` Determines whether contact events should be generated for this shape. 
* `UserData` Pointer to user data that can be associated with this fixture. This is typically used to store custom data about the fixture.



**Returns:**

A ShapeDefinition object initialized with the provided parameters. 





        

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

_This function is used to perform a ray-casting operation in the 2D world. It takes as input a_ [_**QueryParams**_](struct_a_g_e_1_1_query_params.md) _object that contains information about the point of origin and the location where the ray should be casted, as well as other parameters for the query. The function returns an id representing the result of the hit query._
```C++
virtual void AGE::World2D::QueryHit (
    const QueryParams & Params
) override
```





**Parameters:**


* `Params` An instance of [**QueryParams**](struct_a_g_e_1_1_query_params.md) containing all necessary data for the operation. 



**Returns:**

A unique identifier (id) representing the result of the hit query. 





        
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

_Performs a single step of the simulation._ 
```C++
virtual void AGE::World2D::Step (
    TimeStep DeltaTime
) override
```



This function performs one step in the simulation by advancing all bodies and joints in the world according to the specified time step. The number of substeps used is fixed at 4.




**Parameters:**


* `DeltaTime` The duration of the time step. 



**Returns:**

void 





        
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

