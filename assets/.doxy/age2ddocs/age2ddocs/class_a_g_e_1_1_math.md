

# Class AGE::Math



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Math**](class_a_g_e_1_1_math.md)












































## Public Static Functions

| Type | Name |
| ---: | :--- |
|  float | [**ACos**](#function-acos) (float a) <br> |
|  T | [**Add**](#function-add) (T a, T b) <br> |
|  float | [**Cos**](#function-cos) (float a) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**CrossProduct**](#function-crossproduct) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br> |
|  float | [**CrossProduct2D**](#function-crossproduct2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br> |
|  float | [**CubeRoot**](#function-cuberoot) (float a) <br> |
|  bool | [**DecomposeTransform**](#function-decomposetransform) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & Transform, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Translation, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br> |
|  float | [**DegreeToRadians**](#function-degreetoradians) (float Deg) <br> |
|  float | [**Degrees**](#function-degrees-12) (const float Rad) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Degrees**](#function-degrees-22) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) Vec) <br> |
|  float | [**Determinant**](#function-determinant) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & M) <br> |
|  float | [**DistLineLine2D**](#function-distlineline2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & p1, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & v1) <br> |
|  float | [**DistLineLine3D**](#function-distlineline3d) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p1, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v1, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p2, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v2) <br> |
|  float | [**DistPointLine2D**](#function-distpointline2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & q, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & p) <br> |
|  float | [**DistPointLine3D**](#function-distpointline3d) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & q, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br> |
|  T | [**Divide**](#function-divide) (T a, T b) <br> |
|  float | [**DotProduct2D**](#function-dotproduct2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br> |
|  float | [**DotProduct3D**](#function-dotproduct3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br> |
|  float | [**DotProductPlanePoint**](#function-dotproductplanepoint) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f, const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p) <br> |
|  float | [**DotProductPlaneVector**](#function-dotproductplanevector) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br> |
|  bool | [**IntersectLinePlane**](#function-intersectlineplane) (const [**Point3D**](struct_a_g_e_1_1_point3_d.md) & p, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, const [**Plane**](struct_a_g_e_1_1_plane.md) & f, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* q) <br> |
|  bool | [**IntersectThreePlanes**](#function-intersectthreeplanes) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f1, const [**Plane**](struct_a_g_e_1_1_plane.md) & f2, const [**Plane**](struct_a_g_e_1_1_plane.md) & f3, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* p) <br> |
|  bool | [**IntersectTwoPlanes**](#function-intersecttwoplanes) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f1, const [**Plane**](struct_a_g_e_1_1_plane.md) & f2, [**Point3D**](struct_a_g_e_1_1_point3_d.md) \* p, [**Vector3**](struct_a_g_e_1_1_vector3.md) \* v) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**Inverse**](#function-inverse-13) (const [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) & M) <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**Inverse**](#function-inverse-23) (const [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) & M) <br> |
|  [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) | [**Inverse**](#function-inverse-33) (const [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) & H) <br> |
|  float | [**Magnitude**](#function-magnitude) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeInvolution**](#function-makeinvolution) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeReflection**](#function-makereflection-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br> |
|  [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) | [**MakeReflection**](#function-makereflection-22) (const [**Plane**](struct_a_g_e_1_1_plane.md) & f) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotation**](#function-makerotation-12) (float t, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeRotation**](#function-makerotation-22) (float t, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationX**](#function-makerotationx) (float t) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationY**](#function-makerotationy) (float t) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeRotationZ**](#function-makerotationz) (float t) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeScale**](#function-makescale-12) (float s, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a) <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeScale**](#function-makescale-22) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) M, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br> |
|  [**Matrix3D**](struct_a_g_e_1_1_matrix3_d.md) | [**MakeSkew**](#function-makeskew) (float t, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**MakeTransform**](#function-maketransform) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Position, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Rotation, const [**Vector3**](struct_a_g_e_1_1_vector3.md) & Scale) <br> |
|  double | [**Modulo**](#function-modulo) (double a, double b) <br> |
|  T | [**Multiply**](#function-multiply) (T a, T b) <br> |
|  float | [**Pow**](#function-pow) (float a, float b=2.f) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Project2D**](#function-project2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Project3D**](#function-project3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br> |
|  float | [**Radians**](#function-radians-12) (const float Deg) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Radians**](#function-radians-22) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) Vec) <br> |
|  [**Vector2**](struct_a_g_e_1_1_vector2.md) | [**Reject2D**](#function-reject2d) (const [**Vector2**](struct_a_g_e_1_1_vector2.md) & a, const [**Vector2**](struct_a_g_e_1_1_vector2.md) & b) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Reject3D**](#function-reject3d) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & a, [**Vector3**](struct_a_g_e_1_1_vector3.md) & b) <br> |
|  float | [**Sin**](#function-sin) (float a) <br> |
|  float | [**Sqrt**](#function-sqrt) (float a) <br> |
|  T | [**Subtract**](#function-subtract) (T a, T b) <br> |
|  [**Vector3**](struct_a_g_e_1_1_vector3.md) | [**Transform**](#function-transform-12) (const [**Vector3**](struct_a_g_e_1_1_vector3.md) & v, const [**Quaternion**](struct_a_g_e_1_1_quaternion.md) & q) <br> |
|  [**Line**](struct_a_g_e_1_1_line.md) | [**Transform**](#function-transform-22) (const [**Line**](struct_a_g_e_1_1_line.md) & line, const [**Transform4D**](struct_a_g_e_1_1_transform4_d.md) & H) <br> |
|  [**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) | [**Translate**](#function-translate) ([**Matrix4D**](struct_a_g_e_1_1_matrix4_d.md) M, const [**Vector4**](struct_a_g_e_1_1_vector4.md) & a) <br> |


























## Public Static Functions Documentation




### function ACos 

```C++
static inline float AGE::Math::ACos (
    float a
) 
```




<hr>



### function Add 

```C++
template<typename T>
static inline T AGE::Math::Add (
    T a,
    T b
) 
```




<hr>



### function Cos 

```C++
static inline float AGE::Math::Cos (
    float a
) 
```




<hr>



### function CrossProduct 

```C++
static inline Vector3 AGE::Math::CrossProduct (
    const Vector3 & a,
    const Vector3 & b
) 
```




<hr>



### function CrossProduct2D 

```C++
static inline float AGE::Math::CrossProduct2D (
    const Vector2 & a,
    const Vector2 & b
) 
```




<hr>



### function CubeRoot 

```C++
static inline float AGE::Math::CubeRoot (
    float a
) 
```




<hr>



### function DecomposeTransform 

```C++
static bool AGE::Math::DecomposeTransform (
    const Matrix4D & Transform,
    Vector3 & Translation,
    Vector3 & Rotation,
    Vector3 & Scale
) 
```




<hr>



### function DegreeToRadians 

```C++
static inline float AGE::Math::DegreeToRadians (
    float Deg
) 
```




<hr>



### function Degrees [1/2]

```C++
static inline float AGE::Math::Degrees (
    const float Rad
) 
```




<hr>



### function Degrees [2/2]

```C++
static inline Vector3 AGE::Math::Degrees (
    const Vector3 Vec
) 
```




<hr>



### function Determinant 

```C++
static float AGE::Math::Determinant (
    const Matrix3D & M
) 
```




<hr>



### function DistLineLine2D 

```C++
static float AGE::Math::DistLineLine2D (
    const Vector2 & p1,
    const Vector2 & v1
) 
```




<hr>



### function DistLineLine3D 

```C++
static float AGE::Math::DistLineLine3D (
    const Point3D & p1,
    const Vector3 & v1,
    const Point3D & p2,
    const Vector3 & v2
) 
```




<hr>



### function DistPointLine2D 

```C++
static float AGE::Math::DistPointLine2D (
    const Vector2 & q,
    const Vector2 & p
) 
```




<hr>



### function DistPointLine3D 

```C++
static float AGE::Math::DistPointLine3D (
    const Point3D & q,
    const Point3D & p,
    const Vector3 & v
) 
```




<hr>



### function Divide 

```C++
template<typename T>
static inline T AGE::Math::Divide (
    T a,
    T b
) 
```




<hr>



### function DotProduct2D 

```C++
static inline float AGE::Math::DotProduct2D (
    const Vector2 & a,
    const Vector2 & b
) 
```




<hr>



### function DotProduct3D 

```C++
static inline float AGE::Math::DotProduct3D (
    const Vector3 & a,
    const Vector3 & b
) 
```




<hr>



### function DotProductPlanePoint 

```C++
static inline float AGE::Math::DotProductPlanePoint (
    const Plane & f,
    const Point3D & p
) 
```




<hr>



### function DotProductPlaneVector 

```C++
static inline float AGE::Math::DotProductPlaneVector (
    const Plane & f,
    const Vector3 & v
) 
```




<hr>



### function IntersectLinePlane 

```C++
static bool AGE::Math::IntersectLinePlane (
    const Point3D & p,
    const Vector3 & v,
    const Plane & f,
    Point3D * q
) 
```




<hr>



### function IntersectThreePlanes 

```C++
static bool AGE::Math::IntersectThreePlanes (
    const Plane & f1,
    const Plane & f2,
    const Plane & f3,
    Point3D * p
) 
```




<hr>



### function IntersectTwoPlanes 

```C++
static bool AGE::Math::IntersectTwoPlanes (
    const Plane & f1,
    const Plane & f2,
    Point3D * p,
    Vector3 * v
) 
```




<hr>



### function Inverse [1/3]

```C++
static Matrix3D AGE::Math::Inverse (
    const Matrix3D & M
) 
```




<hr>



### function Inverse [2/3]

```C++
static Matrix4D AGE::Math::Inverse (
    const Matrix4D & M
) 
```




<hr>



### function Inverse [3/3]

```C++
static Transform4D AGE::Math::Inverse (
    const Transform4D & H
) 
```




<hr>



### function Magnitude 

```C++
static inline float AGE::Math::Magnitude (
    const Vector3 & v
) 
```




<hr>



### function MakeInvolution 

```C++
static Matrix3D AGE::Math::MakeInvolution (
    const Vector3 & a
) 
```




<hr>



### function MakeReflection [1/2]

```C++
static Matrix3D AGE::Math::MakeReflection (
    const Vector3 & a
) 
```




<hr>



### function MakeReflection [2/2]

```C++
static Transform4D AGE::Math::MakeReflection (
    const Plane & f
) 
```




<hr>



### function MakeRotation [1/2]

```C++
static Matrix3D AGE::Math::MakeRotation (
    float t,
    const Vector3 & a
) 
```




<hr>



### function MakeRotation [2/2]

```C++
static Matrix4D AGE::Math::MakeRotation (
    float t,
    const Vector4 & a
) 
```




<hr>



### function MakeRotationX 

```C++
static Matrix3D AGE::Math::MakeRotationX (
    float t
) 
```




<hr>



### function MakeRotationY 

```C++
static Matrix3D AGE::Math::MakeRotationY (
    float t
) 
```




<hr>



### function MakeRotationZ 

```C++
static Matrix3D AGE::Math::MakeRotationZ (
    float t
) 
```




<hr>



### function MakeScale [1/2]

```C++
static Matrix3D AGE::Math::MakeScale (
    float s,
    const Vector3 & a
) 
```




<hr>



### function MakeScale [2/2]

```C++
static Matrix4D AGE::Math::MakeScale (
    Matrix4D M,
    const Vector4 & a
) 
```




<hr>



### function MakeSkew 

```C++
static Matrix3D AGE::Math::MakeSkew (
    float t,
    const Vector3 & a,
    const Vector3 & b
) 
```




<hr>



### function MakeTransform 

```C++
static Matrix4D AGE::Math::MakeTransform (
    const Vector3 & Position,
    const Vector3 & Rotation,
    const Vector3 & Scale
) 
```




<hr>



### function Modulo 

```C++
static inline double AGE::Math::Modulo (
    double a,
    double b
) 
```




<hr>



### function Multiply 

```C++
template<typename T>
static inline T AGE::Math::Multiply (
    T a,
    T b
) 
```




<hr>



### function Pow 

```C++
static inline float AGE::Math::Pow (
    float a,
    float b=2.f
) 
```




<hr>



### function Project2D 

```C++
static inline Vector2 AGE::Math::Project2D (
    const Vector2 & a,
    const Vector2 & b
) 
```




<hr>



### function Project3D 

```C++
static inline Vector3 AGE::Math::Project3D (
    const Vector3 & a,
    Vector3 & b
) 
```




<hr>



### function Radians [1/2]

```C++
static inline float AGE::Math::Radians (
    const float Deg
) 
```




<hr>



### function Radians [2/2]

```C++
static inline Vector3 AGE::Math::Radians (
    const Vector3 Vec
) 
```




<hr>



### function Reject2D 

```C++
static inline Vector2 AGE::Math::Reject2D (
    const Vector2 & a,
    const Vector2 & b
) 
```




<hr>



### function Reject3D 

```C++
static inline Vector3 AGE::Math::Reject3D (
    const Vector3 & a,
    Vector3 & b
) 
```




<hr>



### function Sin 

```C++
static inline float AGE::Math::Sin (
    float a
) 
```




<hr>



### function Sqrt 

```C++
static inline float AGE::Math::Sqrt (
    float a
) 
```




<hr>



### function Subtract 

```C++
template<typename T>
static inline T AGE::Math::Subtract (
    T a,
    T b
) 
```




<hr>



### function Transform [1/2]

```C++
static Vector3 AGE::Math::Transform (
    const Vector3 & v,
    const Quaternion & q
) 
```




<hr>



### function Transform [2/2]

```C++
static inline Line AGE::Math::Transform (
    const Line & line,
    const Transform4D & H
) 
```




<hr>



### function Translate 

```C++
static Matrix4D AGE::Math::Translate (
    Matrix4D M,
    const Vector4 & a
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/Math.h`

