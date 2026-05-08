

# Class AGE::FileStreamReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md)








Inherits the following classes: [AGE::DataReader](class_a_g_e_1_1_data_reader.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileStreamReader**](#function-filestreamreader-13) () = default<br> |
|   | [**FileStreamReader**](#function-filestreamreader-23) (const std::filesystem::path & Path) <br> |
|   | [**FileStreamReader**](#function-filestreamreader-33) (const [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) &) = delete<br> |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br> |
| virtual bool | [**ReadBytes**](#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) <br> |
| virtual bool | [**ReadBytes**](#function-readbytes-22) (uint8\_t \* Data, size\_t Size) <br> |
| virtual bool | [**ReadData**](#function-readdata) (char \* Data, size\_t Size) <br> |
| virtual bool | [**ReadJson**](#function-readjson) (std::string & String) <br> |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br> |
| virtual  | [**~FileStreamReader**](#function-filestreamreader) () <br> |


## Public Functions inherited from AGE::DataReader

See [AGE::DataReader](class_a_g_e_1_1_data_reader.md)

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](class_a_g_e_1_1_data_reader.md#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](class_a_g_e_1_1_data_reader.md#function-isstreamgood) () const = 0<br> |
|  void | [**ReadArray**](class_a_g_e_1_1_data_reader.md#function-readarray) (std::vector&lt; T &gt; & Array, uint32\_t Size=0) <br> |
|  void | [**ReadBuffer**](class_a_g_e_1_1_data_reader.md#function-readbuffer) (char \* Data, size\_t Size) <br> |
| virtual bool | [**ReadBytes**](class_a_g_e_1_1_data_reader.md#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadBytes**](class_a_g_e_1_1_data_reader.md#function-readbytes-22) (uint8\_t \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadData**](class_a_g_e_1_1_data_reader.md#function-readdata) (char \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadJson**](class_a_g_e_1_1_data_reader.md#function-readjson) (std::string & String) = 0<br> |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-13) (std::map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-23) (std::unordered\_map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-33) (std::unordered\_map&lt; std::string, Value &gt; & Map, uint32\_t Size=0) <br> |
|  void | [**ReadObject**](class_a_g_e_1_1_data_reader.md#function-readobject) (T & Obj) <br> |
|  void | [**ReadRaw**](class_a_g_e_1_1_data_reader.md#function-readraw) (T & Type) <br> |
|  void | [**ReadString**](class_a_g_e_1_1_data_reader.md#function-readstring) (std::string & String) <br> |
| virtual void | [**SetStreamPosition**](class_a_g_e_1_1_data_reader.md#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|   | [**operator bool**](class_a_g_e_1_1_data_reader.md#function-operator-bool) () const<br> |
| virtual  | [**~DataReader**](class_a_g_e_1_1_data_reader.md#function-datareader) () = default<br> |






















































## Public Functions Documentation




### function FileStreamReader [1/3]

```C++
AGE::FileStreamReader::FileStreamReader () = default
```




<hr>



### function FileStreamReader [2/3]

```C++
AGE::FileStreamReader::FileStreamReader (
    const std::filesystem::path & Path
) 
```




<hr>



### function FileStreamReader [3/3]

```C++
AGE::FileStreamReader::FileStreamReader (
    const FileStreamReader &
) = delete
```




<hr>



### function GetStreamPosition 

```C++
inline virtual uint64_t AGE::FileStreamReader::GetStreamPosition () 
```



Implements [*AGE::DataReader::GetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-getstreamposition)


<hr>



### function IsStreamGood 

```C++
inline virtual bool AGE::FileStreamReader::IsStreamGood () const
```



Implements [*AGE::DataReader::IsStreamGood*](class_a_g_e_1_1_data_reader.md#function-isstreamgood)


<hr>



### function ReadBytes [1/2]

```C++
virtual bool AGE::FileStreamReader::ReadBytes (
    std::vector< std::byte > & Data,
    size_t Size
) 
```



Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-12)


<hr>



### function ReadBytes [2/2]

```C++
virtual bool AGE::FileStreamReader::ReadBytes (
    uint8_t * Data,
    size_t Size
) 
```



Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-22)


<hr>



### function ReadData 

```C++
virtual bool AGE::FileStreamReader::ReadData (
    char * Data,
    size_t Size
) 
```



Implements [*AGE::DataReader::ReadData*](class_a_g_e_1_1_data_reader.md#function-readdata)


<hr>



### function ReadJson 

```C++
virtual bool AGE::FileStreamReader::ReadJson (
    std::string & String
) 
```



Implements [*AGE::DataReader::ReadJson*](class_a_g_e_1_1_data_reader.md#function-readjson)


<hr>



### function SetStreamPosition 

```C++
inline virtual void AGE::FileStreamReader::SetStreamPosition (
    uint64_t Pos
) 
```



Implements [*AGE::DataReader::SetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-setstreamposition)


<hr>



### function ~FileStreamReader 

```C++
virtual AGE::FileStreamReader::~FileStreamReader () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataReader.h`

