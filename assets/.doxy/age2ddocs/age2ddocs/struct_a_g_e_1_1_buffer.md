

# Struct AGE::Buffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Buffer**](struct_a_g_e_1_1_buffer.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  void \* | [**Data**](#variable-data)  <br> |
|  uint64\_t | [**Size**](#variable-size)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Allocate**](#function-allocate) (uint64\_t size) <br> |
|   | [**Buffer**](#function-buffer-12) () <br> |
|   | [**Buffer**](#function-buffer-22) (const void \* data, uint64\_t size=0) <br> |
|  T & | [**Read**](#function-read) (uint64\_t offset=0) <br> |
|  char \* | [**ReadBytes**](#function-readbytes) (uint64\_t size, uint64\_t offset) const<br> |
|  void | [**Release**](#function-release) () <br> |
|  void | [**Write**](#function-write) (const void \* data, uint64\_t size, uint64\_t offset=0) <br> |
|  void | [**ZeroInitialize**](#function-zeroinitialize) () <br> |
|   | [**operator bool**](#function-operator-bool) () const<br> |
|  char & | [**operator[]**](#function-operator) (int Index) <br> |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Buffer**](struct_a_g_e_1_1_buffer.md) | [**Copy**](#function-copy-12) (const [**Buffer**](struct_a_g_e_1_1_buffer.md) & Other) <br> |
|  [**Buffer**](struct_a_g_e_1_1_buffer.md) | [**Copy**](#function-copy-22) (const void \* data, uint64\_t size) <br> |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Buffer**](struct_a_g_e_1_1_buffer.md) & Instance) <br> |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Buffer**](struct_a_g_e_1_1_buffer.md) & Instance) <br> |


























## Public Attributes Documentation




### variable Data 

```C++
void* AGE::Buffer::Data;
```




<hr>



### variable Size 

```C++
uint64_t AGE::Buffer::Size;
```




<hr>
## Public Functions Documentation




### function Allocate 

```C++
inline void AGE::Buffer::Allocate (
    uint64_t size
) 
```




<hr>



### function Buffer [1/2]

```C++
inline AGE::Buffer::Buffer () 
```




<hr>



### function Buffer [2/2]

```C++
inline AGE::Buffer::Buffer (
    const void * data,
    uint64_t size=0
) 
```




<hr>



### function Read 

```C++
template<typename T>
inline T & AGE::Buffer::Read (
    uint64_t offset=0
) 
```




<hr>



### function ReadBytes 

```C++
inline char * AGE::Buffer::ReadBytes (
    uint64_t size,
    uint64_t offset
) const
```




<hr>



### function Release 

```C++
inline void AGE::Buffer::Release () 
```




<hr>



### function Write 

```C++
inline void AGE::Buffer::Write (
    const void * data,
    uint64_t size,
    uint64_t offset=0
) 
```




<hr>



### function ZeroInitialize 

```C++
inline void AGE::Buffer::ZeroInitialize () 
```




<hr>



### function operator bool 

```C++
inline AGE::Buffer::operator bool () const
```




<hr>



### function operator[] 

```C++
inline char & AGE::Buffer::operator[] (
    int Index
) 
```




<hr>
## Public Static Functions Documentation




### function Copy [1/2]

```C++
static inline Buffer AGE::Buffer::Copy (
    const Buffer & Other
) 
```




<hr>



### function Copy [2/2]

```C++
static inline Buffer AGE::Buffer::Copy (
    const void * data,
    uint64_t size
) 
```




<hr>



### function Deserialize 

```C++
static inline void AGE::Buffer::Deserialize (
    DataReader * Deserializer,
    Buffer & Instance
) 
```




<hr>



### function Serialize 

```C++
static inline void AGE::Buffer::Serialize (
    DataWriter * Serializer,
    const Buffer & Instance
) 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Buffer.h`

