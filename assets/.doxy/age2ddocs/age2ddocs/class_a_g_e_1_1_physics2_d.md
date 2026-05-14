

# Class AGE::Physics2D



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Physics2D**](class_a_g_e_1_1_physics2_d.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  b2BodyId | [**CreateBody**](#function-createbody) (b2BodyDef & Def) <br>_Creates a body in the physics world._  |
|  b2Polygon | [**CreateBox**](#function-createbox) (float HeightX, float HeightY, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br>_Creates a box shape with the given dimensions and scale._  |
|  b2Capsule | [**CreateCapsule**](#function-createcapsule) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & Offset, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale, const float Radius) <br>_Creates a capsule shape with the given parameters._  |
|  b2ShapeId | [**CreateCapsuleShape**](#function-createcapsuleshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Capsule & Capsule) <br>_Creates a capsule shape in the physics world._  |
|  bool | [**CreateNewPhysicsWorld**](#function-createnewphysicsworld) (Ref&lt; [**Scene**](class_a_g_e_1_1_scene.md) &gt; scene) <br>_Creates a new physics world for the given scene._  |
|  b2ShapeId | [**CreatePolygonShape**](#function-createpolygonshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Polygon & Box) <br>_Creates a polygon shape for the given body with the specified fixture and box._  |
|  b2Segment | [**CreateSegment**](#function-createsegment) () <br>_Creates a segment in the physics world._  |
|  b2ShapeId | [**CreateSegmentShape**](#function-createsegmentshape) (const b2BodyId & ID, const b2ShapeDef & Fixture, const b2Segment & Segment) <br>_Creates a segment shape with the given parameters._  |
|  void | [**DestroyWorld**](#function-destroyworld) () <br>_Destroys the physics world._  |
|  b2BodyId | [**GetBody**](#function-getbody) (const b2ShapeId & ID) <br>_Retrieves a body from the physics world using its shape id._  |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**GetBodyPosition**](#function-getbodyposition) (const b2BodyId & ID) <br>_Get the position of a body in the 2D physics world._  |
|  b2Capsule | [**GetCapsule**](#function-getcapsule) (const b2ShapeId & ID) <br>_Retrieves a capsule with the given shape id._  |
|  b2Polygon | [**GetPolygon**](#function-getpolygon) (const b2ShapeId & ID) <br>_Retrieves a polygon from the physics world using its shape id._  |
|  float | [**GetRotationAngle**](#function-getrotationangle) (const b2BodyId & ID) <br>_This function returns the rotation angle of a body with a given id._  |
|  st atic T | [**GetShapeFromID**](#function-getshapefromid) (b2ShapeId ID) <br>_Retrieves a shape from its ID._  |
|  void \* | [**GetUserData**](#function-getuserdata) (const b2ShapeId & ID) <br>_Retrieves the user data associated with a given shape id._  |
|  Re f&lt; [**World**](class_a_g_e_1_1_world.md) &gt; & | [**GetWorld**](#function-getworld) () <br>_Returns a reference to the_ [_**World**_](class_a_g_e_1_1_world.md) _object._ |
|  b2BodyDef | [**MakeBodyDefinition**](#function-makebodydefinition) (const BodyType & Type, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, bool IsRotationFixed, void \* UserData) <br>_Creates a body definition for the physics world._  |
|  b2Rot | [**MakeRotation**](#function-makerotation) (float Z) <br>_Creates a rotation object based on the given angle in radians._  |
|  b2ShapeDef | [**MakeShapeDefinition**](#function-makeshapedefinition) (float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void \* UserData) <br>_Creates a shape definition with the given parameters._  |
|  void | [**QueryBoxOverlap**](#function-queryboxoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br>_This function is used to perform a box overlap query in the physics world._  |
|  void | [**QueryCapsuleOverlap**](#function-querycapsuleoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br>_This function is used to query for overlapping between a capsule and the physics world._  |
|  bool | [**QueryHit**](#function-queryhit) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br>_This function is used to query for a hit in the physics simulation._  |
|  void | [**QuerySegmentOverlap**](#function-querysegmentoverlap) (const [**QueryParams**](struct_a_g_e_1_1_query_params.md) & Params) <br>_This function is used to query for overlapping segments in the physics world._  |
|  void | [**Step**](#function-step) ([**TimeStep**](class_a_g_e_1_1_time_step.md) DeltaTime) <br>_This function steps the physics simulation by a given time step._  |
|  ~P | [**hysics2D**](#function-hysics2d) () = default<br>_Default constructor for the_ [_**Physics2D**_](class_a_g_e_1_1_physics2_d.md) _class._ |
|  Ph | [**ysics2D**](#function-ysics2d) () = default<br>_Default constructor for the ysics2D class._  |




























## Public Functions Documentation




### function CreateBody 

_Creates a body in the physics world._ 
```C++
b2BodyId AGE::Physics2D::CreateBody (
    b2BodyDef & Def
) 
```



This function creates a new body within the physics simulation based on the provided definition. The body is added to the physics world and its ID is returned.




**Parameters:**


* `Def` A reference to the b2BodyDef that defines the properties of the new body. 



**Returns:**

The unique identifier (b2BodyId) for the newly created body. 





        

<hr>



### function CreateBox 

_Creates a box shape with the given dimensions and scale._ 
```C++
b2Polygon AGE::Physics2D::CreateBox (
    float HeightX,
    float HeightY,
    const Vector3 & Scale
) 
```



This function creates a box shape with the specified height in X and Y directions and applies the provided scale to it. The resulting b2Polygon is then returned by the function.




**Parameters:**


* `HeightX` The horizontal extent of the box. 
* `HeightY` The vertical extent of the box. 
* `Scale` The scaling factor for the box shape.



**Returns:**

A b2Polygon representing the created box shape. 





        

<hr>



### function CreateCapsule 

_Creates a capsule shape with the given parameters._ 
```C++
b2Capsule AGE::Physics2D::CreateCapsule (
    const Vector2 & Offset,
    const Vector3 & Scale,
    const float Radius
) 
```



This function creates and returns a capsule shape using the provided offset, scale, and radius values. The capsule is created in the context of the current world.




**Parameters:**


* `Offset` A [**Vector2**](struct_a_g_e_1_1_vector2.md) specifying the position of the capsule. 
* `Scale` A [**Vector3**](struct_a_g_e_1_1_vector3.md) specifying the scaling factors for the capsule. 
* `Radius` The float value representing the radius of the capsule.



**Returns:**

b2Capsule The newly created capsule shape. 





        

<hr>



### function CreateCapsuleShape 

_Creates a capsule shape in the physics world._ 
```C++
b2ShapeId AGE::Physics2D::CreateCapsuleShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Capsule & Capsule
) 
```



This function creates a capsule shape with the given parameters and adds it to the specified body. The ID of the body is passed as an argument, along with the fixture definition and the dimensions of the capsule.




**Parameters:**


* `ID` The identifier for the body in which the capsule will be added. 
* `Fixture` A structure containing the properties of the fixture to be applied to the shape. 
* `Capsule` A structure containing the dimensions of the capsule (half-height, radius).



**Returns:**

The identifier for the newly created capsule shape. 





        

<hr>



### function CreateNewPhysicsWorld 

_Creates a new physics world for the given scene._ 
```C++
bool AGE::Physics2D::CreateNewPhysicsWorld (
    Ref< Scene > scene
) 
```



This function creates a new physics world and assigns it to the member variable `m_World`. It returns true if the creation was successful, false otherwise.




**Parameters:**


* `scene` The scene for which to create the physics world. 



**Returns:**

True if the creation was successful, false otherwise. 





        

<hr>



### function CreatePolygonShape 

_Creates a polygon shape for the given body with the specified fixture and box._ 
```C++
b2ShapeId AGE::Physics2D::CreatePolygonShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Polygon & Box
) 
```



This function creates a polygon shape for the given body using the provided fixture definition and box. The resulting shape is then returned by the function.




**Parameters:**


* `ID` The identifier of the body to create the shape for. 
* `Fixture` The fixture definition specifying the properties of the shape. 
* `Box` The polygon defining the vertices of the shape.



**Returns:**

A unique identifier representing the newly created shape. 





        

<hr>



### function CreateSegment 

_Creates a segment in the physics world._ 
```C++
b2Segment AGE::Physics2D::CreateSegment () 
```



This function creates and returns a new segment object within the physics world. The specifics of how this is done are not specified as it depends on the implementation of the [**World2D**](class_a_g_e_1_1_world2_d.md) class.




**Returns:**

A newly created segment object. 





        

<hr>



### function CreateSegmentShape 

_Creates a segment shape with the given parameters._ 
```C++
b2ShapeId AGE::Physics2D::CreateSegmentShape (
    const b2BodyId & ID,
    const b2ShapeDef & Fixture,
    const b2Segment & Segment
) 
```



This function creates and adds a new segment shape to the physics world of the game engine. The segment is defined by two points in space.




**Parameters:**


* `ID` A reference to the body id that this fixture will be attached to. 
* `Fixture` A structure containing the definition for the fixture (e.g., density, restitution). 
* `Segment` A structure representing the segment of the shape.



**Returns:**

The unique identifier for the newly created segment shape. 





        

<hr>



### function DestroyWorld 

_Destroys the physics world._ 
```C++
void AGE::Physics2D::DestroyWorld () 
```



This function is used to destroy the physics world, freeing up any resources it was using. After calling this function, the physics world should not be used again until a new one has been created.




**Returns:**

void 





        

<hr>



### function GetBody 

_Retrieves a body from the physics world using its shape id._ 
```C++
b2BodyId AGE::Physics2D::GetBody (
    const b2ShapeId & ID
) 
```



This function takes in a b2ShapeId, which is used to identify a specific shape within the physics world, and returns the corresponding b2BodyId. If no such body exists, it will return an invalid b2BodyId.




**Parameters:**


* `ID` The unique identifier of the shape whose associated body we want to retrieve. 



**Returns:**

The b2BodyId that corresponds to the given shape id. Returns an invalid b2BodyId if no such body exists in the physics world. 





        

<hr>



### function GetBodyPosition 

_Get the position of a body in the 2D physics world._ 
```C++
Vector2 AGE::Physics2D::GetBodyPosition (
    const b2BodyId & ID
) 
```



This function retrieves the current position of a body with a given ID in the 2D physics world. The position is returned as a [**Vector2**](struct_a_g_e_1_1_vector2.md) object.




**Parameters:**


* `ID` The unique identifier for the body whose position you want to retrieve. 



**Returns:**

A [**Vector2**](struct_a_g_e_1_1_vector2.md) object representing the position of the specified body. 





        

<hr>



### function GetCapsule 

_Retrieves a capsule with the given shape id._ 
```C++
b2Capsule AGE::Physics2D::GetCapsule (
    const b2ShapeId & ID
) 
```





**Parameters:**


* `ID` The unique identifier of the capsule to retrieve. 



**Returns:**

A b2Capsule object representing the retrieved capsule, or an empty one if no such capsule exists. 





        

<hr>



### function GetPolygon 

_Retrieves a polygon from the physics world using its shape id._ 
```C++
b2Polygon AGE::Physics2D::GetPolygon (
    const b2ShapeId & ID
) 
```



This function takes an ID of type b2ShapeId as input and returns a b2Polygon object. It retrieves the polygon data associated with the given ID from the physics world.




**Parameters:**


* `ID` The unique identifier for the polygon in the physics world. 



**Returns:**

A b2Polygon object representing the polygon with the provided ID. 





        

<hr>



### function GetRotationAngle 

_This function returns the rotation angle of a body with a given id._ 
```C++
float AGE::Physics2D::GetRotationAngle (
    const b2BodyId & ID
) 
```





**Parameters:**


* `ID` The unique identifier for the body whose rotation angle is to be returned. 



**Returns:**

The rotation angle in radians. If no such body exists, it will return 0. 





        

<hr>



### function GetShapeFromID 

_Retrieves a shape from its ID._ 
```C++
template<typename T>
inline st atic T AGE::Physics2D::GetShapeFromID (
    b2ShapeId ID
) 
```



This function retrieves and returns the shape associated with the given ID. The type of the shape is determined by the value returned by b2Shape\_GetType(ID). If the type is b2\_capsuleShape, it calls b2Shape\_GetCapsule(ID) to get the capsule shape. If the type is b2\_polygonShape, it calls b2Shape\_GetPolygon(ID) to get the polygon shape. If the type is b2\_segmentShape, it calls b2Shape\_GetSegment(ID) to get the segment shape. In all other cases (including if the function returns a default value), it defaults to returning the polygon shape from b2Shape\_GetPolygon(ID).




**Parameters:**


* `ID` The unique identifier of the shape. 



**Returns:**

The shape associated with the given ID, or the default shape if no match is found. 





        

<hr>



### function GetUserData 

_Retrieves the user data associated with a given shape id._ 
```C++
void * AGE::Physics2D::GetUserData (
    const b2ShapeId & ID
) 
```



This function retrieves the user data that was previously set using SetUserData() for a specific shape in the physics world. The shape's ID is used to identify and retrieve its corresponding user data.




**Parameters:**


* `ID` The unique identifier of the shape whose user data needs to be retrieved.



**Returns:**

A void pointer to the user data associated with the given shape id, or nullptr if no such user data exists. 





        

<hr>



### function GetWorld 

_Returns a reference to the_ [_**World**_](class_a_g_e_1_1_world.md) _object._
```C++
inline Re f< World > & AGE::Physics2D::GetWorld () 
```



This function returns a reference to the [**World**](class_a_g_e_1_1_world.md) object that is currently being used by the program. The returned reference can be used to modify or access the state of this object.




**Returns:**

f&lt;World&gt;& A reference to the current [**World**](class_a_g_e_1_1_world.md) object. 





        

<hr>



### function MakeBodyDefinition 

_Creates a body definition for the physics world._ 
```C++
b2BodyDef AGE::Physics2D::MakeBodyDefinition (
    const BodyType & Type,
    const Vector3 & Translation,
    const Vector3 & Rotation,
    bool IsRotationFixed,
    void * UserData
) 
```



This function creates and returns a b2BodyDef object with the given parameters. The body type, translation, rotation, and whether the rotation is fixed are set based on the input parameters. User data can also be provided.




**Parameters:**


* `Type` The type of the body to create. 
* `Translation` The initial position of the body. 
* `Rotation` The initial rotation of the body. 
* `IsRotationFixed` A flag indicating whether the rotation should be fixed or not. 
* `UserData` Pointer to any user data associated with the body.



**Returns:**

Returns a b2BodyDef object based on the input parameters. 





        

<hr>



### function MakeRotation 

_Creates a rotation object based on the given angle in radians._ 
```C++
b2Rot AGE::Physics2D::MakeRotation (
    float Z
) 
```



This function creates and returns a rotation object using the provided angle (in radians). The resulting rotation can be used to rotate objects or perform other transformations.




**Parameters:**


* `Z` The angle in radians for which to create the rotation. 



**Returns:**

A rotation object representing the specified angle. 





        

<hr>



### function MakeShapeDefinition 

_Creates a shape definition with the given parameters._ 
```C++
b2ShapeDef AGE::Physics2D::MakeShapeDefinition (
    float Density,
    float Friction,
    float Restitution,
    bool ShouldGenerateEvents,
    void * UserData
) 
```



This function creates and returns a shape definition using the provided density, friction, restitution, event generation flag, and user data. The resulting shape definition is then used to create a new shape in the physics world.




**Parameters:**


* `Density` The density of the shape. 
* `Friction` The friction coefficient of the shape. 
* `Restitution` The restitution coefficient of the shape. 
* `ShouldGenerateEvents` A flag indicating whether collision events should be generated for this shape. 
* `UserData` Pointer to user-defined data associated with the shape.



**Returns:**

b2ShapeDef The created shape definition. 





        

<hr>



### function QueryBoxOverlap 

_This function is used to perform a box overlap query in the physics world._ 
```C++
void AGE::Physics2D::QueryBoxOverlap (
    const QueryParams & Params
) 
```



The function takes as input a [**QueryParams**](struct_a_g_e_1_1_query_params.md) object which contains all the parameters required for the box overlap query. It then calls the QueryBoxOverlap method on the m\_World object, passing it the [**QueryParams**](struct_a_g_e_1_1_query_params.md) object.




**Parameters:**


* `Params` A const reference to a [**QueryParams**](struct_a_g_e_1_1_query_params.md) object containing the parameters for the box overlap query.



**Returns:**

void This function does not return any value. 





        

<hr>



### function QueryCapsuleOverlap 

_This function is used to query for overlapping between a capsule and the physics world._ 
```C++
void AGE::Physics2D::QueryCapsuleOverlap (
    const QueryParams & Params
) 
```





**Parameters:**


* `Params` The parameters of the capsule overlap query, including position, orientation, radius, and height. 



**Returns:**

void 





        

<hr>



### function QueryHit 

_This function is used to query for a hit in the physics simulation._ 
```C++
bool AGE::Physics2D::QueryHit (
    const QueryParams & Params
) 
```



The function takes as input a const reference to a [**QueryParams**](struct_a_g_e_1_1_query_params.md) object, which contains parameters related to the query. It returns a boolean value indicating whether or not a hit occurred based on these parameters.




**Parameters:**


* `Params` A constant reference to an instance of [**QueryParams**](struct_a_g_e_1_1_query_params.md) containing information about the query. 



**Returns:**

Returns true if a hit is detected and false otherwise. 





        

<hr>



### function QuerySegmentOverlap 

_This function is used to query for overlapping segments in the physics world._ 
```C++
void AGE::Physics2D::QuerySegmentOverlap (
    const QueryParams & Params
) 
```





**Parameters:**


* `Params` The parameters of the segment overlap query, including start and end points, layer mask, etc.



**Returns:**

void 





        

<hr>



### function Step 

_This function steps the physics simulation by a given time step._ 
```C++
void AGE::Physics2D::Step (
    TimeStep DeltaTime
) 
```





**Parameters:**


* `DeltaTime` The amount of time to simulate, in seconds.



**Returns:**

void 





        

<hr>



### function hysics2D 

_Default constructor for the_ [_**Physics2D**_](class_a_g_e_1_1_physics2_d.md) _class._
```C++
~P AGE::Physics2D::hysics2D () = default
```



This function initializes a new instance of the [**Physics2D**](class_a_g_e_1_1_physics2_d.md) class with default values. It does not take any parameters and returns nothing. 


        

<hr>



### function ysics2D 

_Default constructor for the ysics2D class._ 
```C++
Ph AGE::Physics2D::ysics2D () = default
```



This function initializes a new instance of the ysics2D class with default values. It does not take any parameters and returns an object of type ysics2D.




**Returns:**

A new instance of the ysics2D class with default values. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Physics/Public/Physics2D.h`

