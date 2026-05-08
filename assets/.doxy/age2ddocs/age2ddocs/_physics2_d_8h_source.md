

# File Physics2D.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Physics**](dir_0200296fe7041373e4c6a62f3844ed95.md) **>** [**Public**](dir_384ddce68b480931e8586b1cf8a80838.md) **>** [**Physics2D.h**](_physics2_d_8h.md)

[Go to the documentation of this file](_physics2_d_8h.md)


```C++

#pragma once

#include "Core/Public/DeltaTime.h"
#include "Structs/Public/DataStructures.h"
#include "Physics/Public/World.h"
#include "Scene/Public/Components.h"
#include <box2d/types.h>

namespace AGE
{
    class Physics2D final
    {
    public:

        Physics2D() = default;

        ~Physics2D() = default;

        bool CreateNewPhysicsWorld(Ref<Scene> scene);

        void DestroyWorld();

        void Step(TimeStep DeltaTime);

        b2BodyId CreateBody(b2BodyDef& Def);

        b2BodyDef MakeBodyDefinition(const BodyType& Type, const Vector3& Translation, const Vector3& Rotation, bool IsRotationFixed, void* UserData);

        b2ShapeDef MakeShapeDefinition(float Density, float Friction, float Restitution, bool ShouldGenerateEvents, void* UserData);

        b2Rot MakeRotation(float Z);

        b2Polygon CreateBox(float HeightX, float HeightY, const Vector3& Scale);
        b2ShapeId CreatePolygonShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Polygon& Box);

        b2Capsule CreateCapsule(const Vector2& Offset, const Vector3& Scale, const float Radius);
        b2ShapeId CreateCapsuleShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Capsule& Capsule);

        b2Segment CreateSegment();
        b2ShapeId CreateSegmentShape(const b2BodyId& ID, const b2ShapeDef& Fixture, const b2Segment& Segment);

        b2BodyId GetBody(const b2ShapeId& ID);

        Vector2 GetBodyPosition(const b2BodyId& ID);

        b2Polygon GetPolygon(const b2ShapeId& ID);

        b2Capsule GetCapsule(const b2ShapeId& ID);

        void* GetUserData(const b2ShapeId& ID);
        float GetRotationAngle(const b2BodyId& ID);

        void QueryBoxOverlap(const QueryParams& Params);

        void QueryCapsuleOverlap(const QueryParams& Params);

        void QuerySegmentOverlap(const QueryParams& Params);

        bool QueryHit(const QueryParams& Params);

        Ref<World>& GetWorld() { return m_World; }

        template<typename T>
        static T GetShapeFromID(b2ShapeId ID)
        {
            switch (b2Shape_GetType(ID))
            {
            case b2_capsuleShape:
            {
                return b2Shape_GetCapsule(ID);
                break;
            }
            case b2_polygonShape:
            {
                return b2Shape_GetPolygon(ID);
                break;
            }
            case b2_segmentShape:
            {
                return b2Shape_GetSegment(ID);
                break;
            }
            default:
            {
                break;
            }
            }
            return b2Shape_GetPolygon(ID);
        }
    private:

        Ref<World> m_World;
    };
}
```


