

# Class AGE::DataWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**DataWriter**](class_a_g_e_1_1_data_writer.md)










Inherited by the following classes: [AGE::FileStreamWriter](class_a_g_e_1_1_file_stream_writer.md),  [AGE::MemoryStreamWriter](class_a_g_e_1_1_memory_stream_writer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const = 0<br> |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|  void | [**WriteArray**](#function-writearray) (const std::vector&lt; T &gt; & Array, bool WriteSize=true) <br> |
|  void | [**WriteBuffer**](#function-writebuffer) ([**Buffer**](struct_a_g_e_1_1_buffer.md) buffer, bool WriteSize=true) <br> |
| virtual bool | [**WriteData**](#function-writedata) (const char \* Data, size\_t Size) = 0<br> |
|  void | [**WriteMap**](#function-writemap-13) (const std::map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteMap**](#function-writemap-23) (const std::unordered\_map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteMap**](#function-writemap-33) (const std::unordered\_map&lt; std::string, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteObject**](#function-writeobject) (const T & Obj) <br> |
|  void | [**WriteRaw**](#function-writeraw) (const T & Type) <br> |
|  void | [**WriteString**](#function-writestring) (const std::string & String) <br> |
|  void | [**WriteZero**](#function-writezero) (uint64\_t Size) <br> |
|   | [**operator bool**](#function-operator-bool) () const<br> |
| virtual  | [**~DataWriter**](#function-datawriter) () = default<br> |




























## Public Functions Documentation




### function GetStreamPosition 

```C++
virtual uint64_t AGE::DataWriter::GetStreamPosition () = 0
```




<hr>



### function IsStreamGood 

```C++
virtual bool AGE::DataWriter::IsStreamGood () const = 0
```




<hr>



### function SetStreamPosition 

```C++
virtual void AGE::DataWriter::SetStreamPosition (
    uint64_t Pos
) = 0
```




<hr>



### function WriteArray 

```C++
template<typename T>
inline void AGE::DataWriter::WriteArray (
    const std::vector< T > & Array,
    bool WriteSize=true
) 
```




<hr>



### function WriteBuffer 

```C++
void AGE::DataWriter::WriteBuffer (
    Buffer buffer,
    bool WriteSize=true
) 
```




<hr>



### function WriteData 

```C++
virtual bool AGE::DataWriter::WriteData (
    const char * Data,
    size_t Size
) = 0
```




<hr>



### function WriteMap [1/3]

```C++
template<typename Key, typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::map< Key, Value > & Map,
    bool WriteSize=true
) 
```




<hr>



### function WriteMap [2/3]

```C++
template<typename Key, typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::unordered_map< Key, Value > & Map,
    bool WriteSize=true
) 
```




<hr>



### function WriteMap [3/3]

```C++
template<typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::unordered_map< std::string, Value > & Map,
    bool WriteSize=true
) 
```




<hr>



### function WriteObject 

```C++
template<typename T>
inline void AGE::DataWriter::WriteObject (
    const T & Obj
) 
```




<hr>



### function WriteRaw 

```C++
template<typename T>
inline void AGE::DataWriter::WriteRaw (
    const T & Type
) 
```




<hr>



### function WriteString 

```C++
void AGE::DataWriter::WriteString (
    const std::string & String
) 
```




<hr>



### function WriteZero 

```C++
void AGE::DataWriter::WriteZero (
    uint64_t Size
) 
```




<hr>



### function operator bool 

```C++
inline AGE::DataWriter::operator bool () const
```




<hr>



### function ~DataWriter 

```C++
virtual AGE::DataWriter::~DataWriter () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataWriter.h`

