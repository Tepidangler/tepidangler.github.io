

# Struct AGE::Statistics



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Statistics**](struct_a_g_e_1_1_statistics.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**CircleCount**](#variable-circlecount)   = `0`<br> |
|  uint32\_t | [**CubeCount**](#variable-cubecount)   = `0`<br> |
|  uint32\_t | [**CylinderCount**](#variable-cylindercount)   = `0`<br> |
|  uint32\_t | [**DrawCalls**](#variable-drawcalls)   = `0`<br> |
|  uint32\_t | [**LineCount**](#variable-linecount)   = `0`<br> |
|  uint32\_t | [**ModelCount**](#variable-modelcount)   = `0`<br> |
|  uint32\_t | [**PyramidCount**](#variable-pyramidcount)   = `0`<br> |
|  uint32\_t | [**QuadCount**](#variable-quadcount)   = `0`<br> |
|  uint32\_t | [**SphereCount**](#variable-spherecount)   = `0`<br> |
|  uint32\_t | [**TextCount**](#variable-textcount)   = `0`<br> |
|  uint32\_t | [**TileCount**](#variable-tilecount)   = `0`<br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  uint32\_t | [**GetTotalCubeIndexCount**](#function-gettotalcubeindexcount) () <br>_This function returns the total count of cube indices in the scene. The count is calculated by multiplying the number of cubes (_ `CubeCount` _) by 36 (the number of indices per cube)._ |
|  uint32\_t | [**GetTotalCubeVertexCount**](#function-gettotalcubevertexcount) () <br>_Calculates the total number of vertices in a cube._  |
|  uint32\_t | [**GetTotalCylinderIndexCount**](#function-gettotalcylinderindexcount) () <br>_This function returns the total number of cylinders in the system, multiplied by 18._  |
|  uint32\_t | [**GetTotalCylinderVertexCount**](#function-gettotalcylindervertexcount) () <br>_This function returns the total number of vertices in all cylinders. The calculation is based on each cylinder having 8 vertices._  |
|  uint32\_t | [**GetTotalPyramidIndexCount**](#function-gettotalpyramidindexcount) () <br>_This function calculates the total number of indices in a pyramid. The pyramid is represented as an array where each element represents a cube. Each cube has 6 faces, so to get the total number of indices, we multiply the number of cubes by 6._  |
|  uint32\_t | [**GetTotalPyramidVertexCount**](#function-gettotalpyramidvertexcount) () <br>_Calculates the total number of vertices in a pyramid._  |
|  uint32\_t | [**GetTotalQuadIndexCount**](#function-gettotalquadindexcount) () <br>_This function returns the total number of indices used by all quads in the scene. Each quad is composed of four vertices and each vertex has three coordinates, so a quad uses 24 indices. The function multiplies the number of quads (QuadCount) by 6 to get the total index count._  |
|  uint32\_t | [**GetTotalQuadVertexCount**](#function-gettotalquadvertexcount) () <br>_This function returns the total number of vertices in all quads._  |
|  uint32\_t | [**GetTotalSphereIndexCount**](#function-gettotalsphereindexcount) () <br>_This function returns the total number of sphere indices in the scene. Each sphere is represented by 36 indices (12 for each face). The count of spheres is multiplied by 36 to get the total index count._  |
|  uint32\_t | [**GetTotalSphereVertexCount**](#function-gettotalspherevertexcount) () <br>_Calculates the total number of vertices in all spheres._  |
|  uint32\_t | [**GetTotalTileIndexCount**](#function-gettotaltileindexcount) () <br>_This function returns the total number of tile indices in the game world. The count is calculated by multiplying the total number of tiles (TileCount) with 6._  |
|  uint32\_t | [**GetTotalTileVertexCount**](#function-gettotaltilevertexcount) () <br>_Calculates the total number of vertices in all tiles._  |




























## Public Attributes Documentation




### variable CircleCount 

```C++
uint32_t AGE::Statistics::CircleCount;
```




<hr>



### variable CubeCount 

```C++
uint32_t AGE::Statistics::CubeCount;
```




<hr>



### variable CylinderCount 

```C++
uint32_t AGE::Statistics::CylinderCount;
```




<hr>



### variable DrawCalls 

```C++
uint32_t AGE::Statistics::DrawCalls;
```




<hr>



### variable LineCount 

```C++
uint32_t AGE::Statistics::LineCount;
```




<hr>



### variable ModelCount 

```C++
uint32_t AGE::Statistics::ModelCount;
```




<hr>



### variable PyramidCount 

```C++
uint32_t AGE::Statistics::PyramidCount;
```




<hr>



### variable QuadCount 

```C++
uint32_t AGE::Statistics::QuadCount;
```




<hr>



### variable SphereCount 

```C++
uint32_t AGE::Statistics::SphereCount;
```




<hr>



### variable TextCount 

```C++
uint32_t AGE::Statistics::TextCount;
```




<hr>



### variable TileCount 

```C++
uint32_t AGE::Statistics::TileCount;
```




<hr>
## Public Functions Documentation




### function GetTotalCubeIndexCount 

_This function returns the total count of cube indices in the scene. The count is calculated by multiplying the number of cubes (_ `CubeCount` _) by 36 (the number of indices per cube)._
```C++
inline uint32_t AGE::Statistics::GetTotalCubeIndexCount () 
```





**Returns:**

Total count of cube indices in the scene.


This function returns the total count of cube indices in the scene. Each cube has 36 indices (2 for each of its 18 edges). 

**Returns:**

The total number of cube indices in the scene. 





        

<hr>



### function GetTotalCubeVertexCount 

_Calculates the total number of vertices in a cube._ 
```C++
inline uint32_t AGE::Statistics::GetTotalCubeVertexCount () 
```



The function multiplies the number of cubes by 8 to get the total vertex count. This is because each cube has 8 vertices.




**Returns:**

uint32\_t Total number of vertices in all cubes.


Calculates the total number of vertices in a cube.


The function multiplies the number of cubes by 8 to get the total vertex count. This is because each cube has 8 vertices.




**Returns:**

uint32\_t Total number of vertices in all cubes. 





        

<hr>



### function GetTotalCylinderIndexCount 

_This function returns the total number of cylinders in the system, multiplied by 18._ 
```C++
inline uint32_t AGE::Statistics::GetTotalCylinderIndexCount () 
```





**Returns:**

The total count of cylinders in the system.


This function returns the total count of cylinder indices based on the number of cylinders. 

**Returns:**

The total count of cylinder indices as a uint32\_t value. 





        

<hr>



### function GetTotalCylinderVertexCount 

_This function returns the total number of vertices in all cylinders. The calculation is based on each cylinder having 8 vertices._ 
```C++
inline uint32_t AGE::Statistics::GetTotalCylinderVertexCount () 
```





**Returns:**

uint32\_t Total number of vertices in all cylinders.


This function returns the total number of vertices in all cylinders. The calculation is based on each cylinder having 8 vertices. 

**Returns:**

uint32\_t Total count of vertices in all cylinders. 





        

<hr>



### function GetTotalPyramidIndexCount 

_This function calculates the total number of indices in a pyramid. The pyramid is represented as an array where each element represents a cube. Each cube has 6 faces, so to get the total number of indices, we multiply the number of cubes by 6._ 
```C++
inline uint32_t AGE::Statistics::GetTotalPyramidIndexCount () 
```





**Returns:**

uint32\_t Total number of indices in the pyramid.


This function calculates the total number of indices in a pyramid. The pyramid is represented as an equilateral triangle and each face of the triangle is a cube, so the total number of cubes that make up the pyramid is multiplied by 6 to get the total number of indices. 

**Returns:**

uint32\_t This function returns the total number of indices in the pyramid as an unsigned 32-bit integer. 





        

<hr>



### function GetTotalPyramidVertexCount 

_Calculates the total number of vertices in a pyramid._ 
```C++
inline uint32_t AGE::Statistics::GetTotalPyramidVertexCount () 
```



The function multiplies the number of pyramids by 5 to get the total vertex count.




**Returns:**

uint32\_t Total number of vertices in all pyramids.


Calculates the total number of vertices in a pyramid.


The function multiplies the number of pyramids by 5 to get the total vertex count.




**Returns:**

uint32\_t Total number of vertices in all pyramids. 





        

<hr>



### function GetTotalQuadIndexCount 

_This function returns the total number of indices used by all quads in the scene. Each quad is composed of four vertices and each vertex has three coordinates, so a quad uses 24 indices. The function multiplies the number of quads (QuadCount) by 6 to get the total index count._ 
```C++
inline uint32_t AGE::Statistics::GetTotalQuadIndexCount () 
```





**Returns:**

uint32\_t Total number of indices used by all quads in the scene.


This function returns the total number of indices used by all quads in the system. The count is calculated as the product of the quad count and 6, representing each quad's four triangles (2 triangles per face) and three vertices per triangle.




**Returns:**

uint32\_t Total index count for all quads. 





        

<hr>



### function GetTotalQuadVertexCount 

_This function returns the total number of vertices in all quads._ 
```C++
inline uint32_t AGE::Statistics::GetTotalQuadVertexCount () 
```



The function multiplies the number of quads by 4 to get the total vertex count.




**Returns:**

uint32\_t Total number of vertices in all quads.


This function returns the total number of vertices in all quads. It multiplies the count of quads by 4 to get the total vertex count.




**Returns:**

The total number of vertices in all quads. 





        

<hr>



### function GetTotalSphereIndexCount 

_This function returns the total number of sphere indices in the scene. Each sphere is represented by 36 indices (12 for each face). The count of spheres is multiplied by 36 to get the total index count._ 
```C++
inline uint32_t AGE::Statistics::GetTotalSphereIndexCount () 
```





**Returns:**

uint32\_t Total number of sphere indices in the scene.


This function returns the total number of sphere indices in the scene. The calculation is based on the assumption that each sphere has 36 indices (vertices, normals and texture coordinates). 

**Returns:**

uint32\_t Total number of sphere indices. 





        

<hr>



### function GetTotalSphereVertexCount 

_Calculates the total number of vertices in all spheres._ 
```C++
inline uint32_t AGE::Statistics::GetTotalSphereVertexCount () 
```



This function multiplies the number of spheres by 8 to get the total vertex count. It assumes that each sphere has 8 vertices.




**Returns:**

The total number of vertices in all spheres.


Calculates the total number of vertices in all spheres.


This function multiplies the count of spheres by 8 to get the total vertex count. It assumes that each sphere has 8 vertices.




**Returns:**

The total number of vertices in all spheres. 





        

<hr>



### function GetTotalTileIndexCount 

_This function returns the total number of tile indices in the game world. The count is calculated by multiplying the total number of tiles (TileCount) with 6._ 
```C++
inline uint32_t AGE::Statistics::GetTotalTileIndexCount () 
```





**Returns:**

uint32\_t Total number of tile indices in the game world.


This function returns the total number of tile indices in the game world. The count is calculated by multiplying the total number of tiles (TileCount) with 6. 

**Returns:**

uint32\_t Total number of tile indices in the game world. 





        

<hr>



### function GetTotalTileVertexCount 

_Calculates the total number of vertices in all tiles._ 
```C++
inline uint32_t AGE::Statistics::GetTotalTileVertexCount () 
```



This function multiplies the number of tiles by 4 to get the total vertex count. The assumption is that each tile has 4 vertices.




**Returns:**

Total number of vertices across all tiles.


This function returns the total number of vertices in all tiles. The calculation is based on each tile having 4 vertices. Therefore, it multiplies the number of tiles by 4 to get the total vertex count.




**Returns:**

uint32\_t Total number of vertices across all tiles. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Math/Public/MathStructures.h`

