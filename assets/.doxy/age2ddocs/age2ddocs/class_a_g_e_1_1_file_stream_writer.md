

# Class AGE::FileStreamWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md)








Inherits the following classes: [AGE::DataWriter](class_a_g_e_1_1_data_writer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileStreamWriter**](#function-filestreamwriter-13) () = default<br> |
|   | [**FileStreamWriter**](#function-filestreamwriter-23) (const std::filesystem::path & Path) <br> |
|   | [**FileStreamWriter**](#function-filestreamwriter-33) (const [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) &) = delete<br> |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br> |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br> |
| virtual bool | [**WriteData**](#function-writedata) (const char \* Data, size\_t Size) <br> |
| virtual  | [**~FileStreamWriter**](#function-filestreamwriter) () <br> |


## Public Functions inherited from AGE::DataWriter

See [AGE::DataWriter](class_a_g_e_1_1_data_writer.md)

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](class_a_g_e_1_1_data_writer.md#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](class_a_g_e_1_1_data_writer.md#function-isstreamgood) () const = 0<br> |
| virtual void | [**SetStreamPosition**](class_a_g_e_1_1_data_writer.md#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|  void | [**WriteArray**](class_a_g_e_1_1_data_writer.md#function-writearray) (const std::vector&lt; T &gt; & Array, bool WriteSize=true) <br> |
|  void | [**WriteBuffer**](class_a_g_e_1_1_data_writer.md#function-writebuffer) ([**Buffer**](struct_a_g_e_1_1_buffer.md) buffer, bool WriteSize=true) <br> |
| virtual bool | [**WriteData**](class_a_g_e_1_1_data_writer.md#function-writedata) (const char \* Data, size\_t Size) = 0<br> |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-13) (const std::map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-23) (const std::unordered\_map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-33) (const std::unordered\_map&lt; std::string, Value &gt; & Map, bool WriteSize=true) <br> |
|  void | [**WriteObject**](class_a_g_e_1_1_data_writer.md#function-writeobject) (const T & Obj) <br> |
|  void | [**WriteRaw**](class_a_g_e_1_1_data_writer.md#function-writeraw) (const T & Type) <br> |
|  void | [**WriteString**](class_a_g_e_1_1_data_writer.md#function-writestring) (const std::string & String) <br> |
|  void | [**WriteZero**](class_a_g_e_1_1_data_writer.md#function-writezero) (uint64\_t Size) <br> |
|   | [**operator bool**](class_a_g_e_1_1_data_writer.md#function-operator-bool) () const<br> |
| virtual  | [**~DataWriter**](class_a_g_e_1_1_data_writer.md#function-datawriter) () = default<br> |






















































## Public Functions Documentation




### function FileStreamWriter [1/3]

```C++
AGE::FileStreamWriter::FileStreamWriter () = default
```




<hr>



### function FileStreamWriter [2/3]

```C++
AGE::FileStreamWriter::FileStreamWriter (
    const std::filesystem::path & Path
) 
```




<hr>



### function FileStreamWriter [3/3]

```C++
AGE::FileStreamWriter::FileStreamWriter (
    const FileStreamWriter &
) = delete
```




<hr>



### function GetStreamPosition 

```C++
inline virtual uint64_t AGE::FileStreamWriter::GetStreamPosition () 
```



Implements [*AGE::DataWriter::GetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-getstreamposition)


<hr>



### function IsStreamGood 

```C++
inline virtual bool AGE::FileStreamWriter::IsStreamGood () const
```



Implements [*AGE::DataWriter::IsStreamGood*](class_a_g_e_1_1_data_writer.md#function-isstreamgood)


<hr>



### function SetStreamPosition 

```C++
inline virtual void AGE::FileStreamWriter::SetStreamPosition (
    uint64_t Pos
) 
```



Implements [*AGE::DataWriter::SetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-setstreamposition)


<hr>



### function WriteData 

```C++
virtual bool AGE::FileStreamWriter::WriteData (
    const char * Data,
    size_t Size
) 
```



Implements [*AGE::DataWriter::WriteData*](class_a_g_e_1_1_data_writer.md#function-writedata)


<hr>



### function ~FileStreamWriter 

```C++
virtual AGE::FileStreamWriter::~FileStreamWriter () 
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataWriter.h`

