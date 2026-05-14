

# File World2D.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Physics**](dir_0200296fe7041373e4c6a62f3844ed95.md) **>** [**Private**](dir_aa1a9f4b85cc4e4a5149e0c99c6c45ae.md) **>** [**World2D.cpp**](_world2_d_8cpp.md)

[Go to the documentation of this file](_world2_d_8cpp.md)


```C++

#include "AGEpch.hpp"
#include "Physics/Public/World2D.h"

namespace AGE
{
    st
atic b2BodyType Rigid2DTypeToBox2DBody(BodyType BodyType)
    {
        switch (BodyType)
        {
        case BodyType::Static:
        {
            return b2_staticBody;
        }
        case BodyType::Dynamic:
        {
            return b2_dynamicBody;
        }
        case BodyType::Kinematic:
        {
            return b2_kinematicBody;
        }
        }

        CoreLogger::Assert(false, "Unknown Body Type");
        return b2_staticBody;
    }

    Wo
rld2D::World2D(Ref<Scene> scene)
        :m_WorldScene(scene)
    {
        CoreLogger::Trace("Initializing World {}", scene->GetName());
        b2WorldDef WorldDef = b2DefaultWorldDef();
        WorldDef.gravity = { 0.0f,-9.8f };
        m_World = b2CreateWorld(&WorldDef);
    }

    Wo
rld2D::~World2D()
    {
        if (b2World_IsValid(m_World))
        { 
            b2DestroyWorld(m_World);
        }
    }

    vo
id World2D::DestroyWorld()
    {
        b2DestroyWorld(m_World);
    }

    vo
id World2D::Step(TimeStep DeltaTime)
    {
        const int32_t SubStepCount = 4;

        b2World_Step(m_World, DeltaTime, SubStepCount);
    }

    vo
id World2D::MakeDefaultQueryFilter()
    {
        m_QueryFilter = b2DefaultQueryFilter(); 
    }

    vo"This function queries for overlaps within a 2D world using Box2D. It takes as input a QueryParams struct containing all necessary parameters for the overlap query."
id World2D::QueryBoxOverlap(const QueryParams& Params)
    {
        [[maybe_unused]] Box2DQueryContext QC = { Params.Point2D,Params.InstigatorID };
        b2ShapeProxy Proxy{};
        Proxy.count = Params.Box2D.count;
        for (size_t i = 0; i < 4; i++)
        {
            Proxy.points[i] = Params.Box2D.vertices[i];
        }
        b2Transform Trans;
        Trans.p = { Params.Location.x,Params.Location.y };
        Trans.q = b2MakeRot(Params.Rotation.z);
        b2World_OverlapShape(m_World, &Proxy,GetQueryFilter(),Params.OverlapFunc2D, Params.Context);
    }

    vo
id World2D::QueryCapsuleOverlap(const QueryParams& Params)
    {
        [[maybe_unused]] Box2DQueryContext QC = { Params.Point2D,Params.InstigatorID };
        b2ShapeProxy Proxy{};
        Proxy.count = 2;
        Proxy.points[0] = Params.Capsule2D.center1;
        Proxy.points[1] = Params.Capsule2D.center2;
        Proxy.radius = Params.Box2D.radius;
        b2Transform Trans;
        Trans.p = { Params.Location.x,Params.Location.y };
        Trans.q = b2MakeRot(Params.Rotation.z);
        b2World_OverlapShape(m_World, &Proxy,GetQueryFilter(),Params.OverlapFunc2D, Params.Context);
    }

    vo"Unknown"
id World2D::QuerySegmentOverlap(const QueryParams& Params)
    {

        Box2DQueryContext QC = { Params.Point2D,Params.InstigatorID };
        b2Transform Trans;
        Trans.p = { Params.Location.x,Params.Location.y };
        Trans.q = b2MakeRot(Params.Rotation.z);
        b2AABB SegAABB = b2ComputeSegmentAABB(&Params.Segment2D, Trans);
        b2World_OverlapAABB(m_World, SegAABB, GetQueryFilter(), Params.OverlapFunc2D, &QC);
    }

    vo
id World2D::QueryHit(const QueryParams& Params)
    {
        Box2DQueryContext QC = { Params.Point2D, Params.InstigatorID };
        b2Vec2 Origin = { Params.Point2D.x, Params.Point2D.y };
        b2Vec2 Translation = { Params.Location.x, Params.Location.y };

        //b2WorldId worldId, const b2Circle* circle, b2Transform originTransform, b2Vec2 translation, b2QueryFilter filter, b2CastResultFcn* fcn, void* context
        b2World_CastRay(m_World, Origin, Translation, GetQueryFilter(), Params.CastFunc2D, &QC);
    }

    b2
BodyDef World2D::MakeBodyDefinition(const BodyType& Type, const Vector3& Translation, const Vector3& Rotation, bool IsRotationFixed, void* UserData)
    {
        b2BodyDef Def = b2DefaultBodyDef();

        Def.userData = UserData;
        Def.type = Rigid2DTypeToBox2DBody(Type);
        Def.position.x = Translation.x;
        Def.position.y = Translation.y;
        Def.rotation = b2MakeRot(Rotation.z);
        //Def.rotation = MakeRotation(Rotation.z);
        Def.fixedRotation = IsRotationFixed;
        
        return Def;
    }

    b2
ShapeDef World2D::MakeShapeDefinition(float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void* UserData)
    {
        b2ShapeDef Fixture = b2DefaultShapeDef();
        Fixture.userData = UserData;
        Fixture.density = Density;
        //Fixture.friction = Friction;
        //Fixture.restitution = Restitution;
        Fixture.enableContactEvents = ShouldGenerateEvents;
        Fixture.enableHitEvents = ShouldGenerateEvents;

        return Fixture;
    }

    b2
Rot World2D::MakeRotation(float Z)
    {
        return b2MakeRot(Z);
    }

    b2
Polygon World2D::CreateBox(float HeightX, float HeightY, const Vector3& Scale)
    {
        return b2MakeBox(HeightX * Scale.x, HeightY * Scale.y);
    }

    b2
ShapeId World2D::CreatePolygonShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Polygon& Box)
    {
        return b2CreatePolygonShape(ID, &Fixture, &Box);
    }

    b2
Capsule World2D::CreateCapsule(const Vector2& Offset, const Vector3& Scale, const float Radius)
    {
        b2Capsule Capsule;
        Capsule.center1 = { Offset.x * Scale.x, Offset.y * Scale.y };
        Capsule.center2 = { (Offset.x * Scale.x) - 1.f, (Offset.y * Scale.y) - 1.f };
        Capsule.radius = Scale.x * Radius;

        return Capsule;
    }

    b2
ShapeId World2D::CreateCapsuleShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Capsule& Capsule)
    {
        return b2CreateCapsuleShape(ID, &Fixture, &Capsule);
    }

    b2
Segment World2D::CreateSegment()
    {
        return { {0.f, 0.f},{1.f, 0.f} };
    }

    b2
ShapeId World2D::CreateSegmentShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Segment& Segment)
    {
        return b2CreateSegmentShape(ID, &Fixture, &Segment);
    }

    b2
BodyId World2D::CreateBody(b2BodyDef& Def)
    {
        return b2CreateBody(m_World, &Def);;
    }

    b2
BodyId World2D::GetBody(const b2ShapeId& ID)
    {
        return b2Shape_GetBody(ID);
    }

    Ve
ctor2 World2D::GetBodyPosition(const b2BodyId& ID)
    {
        b2Vec2 Vec = b2Body_GetPosition(ID);
        return Vector2(Vec.x, Vec.y);
    }

    b2
Polygon World2D::GetPolygon(const b2ShapeId& ID)
    {
        return b2Shape_GetPolygon(ID);
    }

    b2
Capsule World2D::GetCapsule(const b2ShapeId& ID)
    {
        return b2Shape_GetCapsule(ID);
    }

    fl
oat World2D::GetRotationAngle(const b2BodyId& ID)
    {
        return Math::Degrees(b2Rot_GetAngle(b2Body_GetRotation(ID)));
    }

    vo
id* World2D::GetUserData(const b2ShapeId& ID)
    {
        return b2Shape_GetUserData(ID);
    }

    b2
WorldId& World2D::GetWorld()
    {
        return m_World;
    }
    Re
f<Scene>& World2D::GetWorldScene()
    {
        return m_WorldScene;
    }

    template<>
    Wo
rld2D* World::As()
    {
        return (World2D*)this;
    }
}
```


