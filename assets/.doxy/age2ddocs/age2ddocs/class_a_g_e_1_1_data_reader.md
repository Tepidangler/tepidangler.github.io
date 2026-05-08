

# Class AGE::DataReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**DataReader**](class_a_g_e_1_1_data_reader.md)










Inherited by the following classes: [AGE::FileStreamReader](class_a_g_e_1_1_file_stream_reader.md),  [AGE::MemoryStreamReader](class_a_g_e_1_1_memory_stream_reader.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const = 0<br> |
|  void | [**ReadArray**](#function-readarray) (std::vector&lt; T &gt; & Array, uint32\_t Size=0) <br> |
|  void | [**ReadBuffer**](#function-readbuffer) (char \* Data, size\_t Size) <br> |
| virtual bool | [**ReadBytes**](#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadBytes**](#function-readbytes-22) (uint8\_t \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadData**](#function-readdata) (char \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadJson**](#function-readjson) (std::string & String) = 0<br> |
|  void | [**ReadMap**](#function-readmap-13) (std::map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadMap**](#function-readmap-23) (std::unordered\_map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadMap**](#function-readmap-33) (std::unordered\_map&lt; std::string, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadObject**](#function-readobject) (T & Obj) <br> |
|  void | [**ReadRaw**](#function-readraw) (T & Type) <br> |
|  void | [**ReadString**](#function-readstring) (std::string & String) <br> |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|   | [**operator bool**](#function-operator-bool) () const<br> |
| virtual  | [**~DataReader**](#function-datareader) () = default<br> |




























## Public Functions Documentation




### function GetStreamPosition 

```C++
virtual uint64_t AGE::DataReader::GetStreamPosition () = 0
```




<hr>



### function IsStreamGood 

```C++
virtual bool AGE::DataReader::IsStreamGood () const = 0
```




<hr>



### function ReadArray 

```C++
template<typename T>
inline void AGE::DataReader::ReadArray (
    std::vector< T > & Array,
    uint32_t Size=0
) 
```




<hr>



### function ReadBuffer 

```C++
void AGE::DataReader::ReadBuffer (
    char * Data,
    size_t Size
) 
```




<hr>



### function ReadBytes [1/2]

```C++
virtual bool AGE::DataReader::ReadBytes (
    std::vector< std::byte > & Data,
    size_t Size
) = 0
```




<hr>



### function ReadBytes [2/2]

```C++
virtual bool AGE::DataReader::ReadBytes (
    uint8_t * Data,
    size_t Size
) = 0
```




<hr>



### function ReadData 

```C++
virtual bool AGE::DataReader::ReadData (
    char * Data,
    size_t Size
) = 0
```




<hr>



### function ReadJson 

```C++
virtual bool AGE::DataReader::ReadJson (
    std::string & String
) = 0
```




<hr>



### function ReadMap [1/3]

```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::map< Key, Value > & Map,
    uint32_t Size=0
) 
```




<hr>



### function ReadMap [2/3]

```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::unordered_map< Key, Value > & Map,
    uint32_t Size=0
) 
```




<hr>



### function ReadMap [3/3]

```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::unordered_map< std::string, Value > & Map,
    uint32_t Size=0
) 
```




<hr>



### function ReadObject 

```C++
template<typename T>
inline void AGE::DataReader::ReadObject (
    T & Obj
) 
```




<hr>



### function ReadRaw 

```C++
template<typename T>
inline void AGE::DataReader::ReadRaw (
    T & Type
) 
```




<hr>



### function ReadString 

```C++
void AGE::DataReader::ReadString (
    std::string & String
) 
```




<hr>



### function SetStreamPosition 

```C++
virtual void AGE::DataReader::SetStreamPosition (
    uint64_t Pos
) = 0
```




<hr>



### function operator bool 

```C++
inline AGE::DataReader::operator bool () const
```




<hr>



### function ~DataReader 

```C++
virtual AGE::DataReader::~DataReader () = default
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataReader.h`

