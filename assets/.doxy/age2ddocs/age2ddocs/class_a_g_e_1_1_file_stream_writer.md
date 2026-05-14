

# Class AGE::FileStreamWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md)








Inherits the following classes: [AGE::DataWriter](class_a_g_e_1_1_data_writer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileStreamWriter**](#function-filestreamwriter-13) () = default<br>_Default constructor for_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class._ |
|   | [**FileStreamWriter**](#function-filestreamwriter-23) (const std::filesystem::path & Path) <br>_Constructs a_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _object with the given file path._ |
|   | [**FileStreamWriter**](#function-filestreamwriter-33) (const [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) &) = delete<br>_This function is a copy constructor for the_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class and it has been explicitly deleted to prevent copying of objects._ |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br>_Get the current position in the stream._  |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br>_Checks the state of the stream._  |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br>_Sets the stream position to a specified value._  |
| virtual bool | [**WriteData**](#function-writedata) (const char \* Data, size\_t Size) <br>_Writes data to the file stream._  |
| virtual  | [**~FileStreamWriter**](#function-filestreamwriter) () <br>_Destructor for the_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class. Closes the file stream associated with this object._ |


## Public Functions inherited from AGE::DataWriter

See [AGE::DataWriter](class_a_g_e_1_1_data_writer.md)

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](class_a_g_e_1_1_data_writer.md#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](class_a_g_e_1_1_data_writer.md#function-isstreamgood) () const = 0<br> |
| virtual void | [**SetStreamPosition**](class_a_g_e_1_1_data_writer.md#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|  void | [**WriteArray**](class_a_g_e_1_1_data_writer.md#function-writearray) (const std::vector&lt; T &gt; & Array, bool WriteSize=true) <br>_Writes an array to a stream._  |
|  void | [**WriteBuffer**](class_a_g_e_1_1_data_writer.md#function-writebuffer) ([**Buffer**](struct_a_g_e_1_1_buffer.md) buffer, bool WriteSize=true) <br>_Writes a buffer to the data stream._  |
| virtual bool | [**WriteData**](class_a_g_e_1_1_data_writer.md#function-writedata) (const char \* Data, size\_t Size) = 0<br> |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-13) (const std::map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br>_Writes a map to the underlying storage._  |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-23) (const std::unordered\_map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br>_This function writes an unordered map to a data stream. It can optionally write the size of the map as well._  |
|  void | [**WriteMap**](class_a_g_e_1_1_data_writer.md#function-writemap-33) (const std::unordered\_map&lt; std::string, Value &gt; & Map, bool WriteSize=true) <br>_Writes a map to the stream. If WriteSize is true, it writes the size of the map first. Then for each key-value pair in the map, it writes the key as a string and the value. For trivial types, it directly writes the value using WriteRaw. For non-trivial types, it uses WriteObject._  |
|  void | [**WriteObject**](class_a_g_e_1_1_data_writer.md#function-writeobject) (const T & Obj) <br>_This function writes an object to the stream by serializing it._  |
|  void | [**WriteRaw**](class_a_g_e_1_1_data_writer.md#function-writeraw) (const T & Type) <br>_Writes raw data of a specific type._  |
|  void | [**WriteString**](class_a_g_e_1_1_data_writer.md#function-writestring) (const std::string & String) <br>_Writes a string to the data stream, including its length prefix._  |
|  void | [**WriteZero**](class_a_g_e_1_1_data_writer.md#function-writezero) (uint64\_t Size) <br>_Writes a block of zeros to the data stream._  |
|   | [**operator bool**](class_a_g_e_1_1_data_writer.md#function-operator-bool) () const<br>_Checks the state of the stream._  |
| virtual  | [**~DataWriter**](class_a_g_e_1_1_data_writer.md#function-datawriter) () = default<br>_Virtual destructor for the_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _class._ |






















































## Public Functions Documentation




### function FileStreamWriter [1/3]

_Default constructor for_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class._
```C++
AGE::FileStreamWriter::FileStreamWriter () = default
```



This function initializes an instance of the [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) class with default settings. It does not take any parameters and returns no value.


Default constructor for [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) class.


This function initializes an instance of the [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) class with default values. It does not take any parameters and returns nothing. 


        

<hr>



### function FileStreamWriter [2/3]

_Constructs a_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _object with the given file path._
```C++
AGE::FileStreamWriter::FileStreamWriter (
    const std::filesystem::path & Path
) 
```



This constructor opens an output stream to the specified file path using binary mode. If the file does not exist, it will be created when data is written to the stream.




**Parameters:**


* `Path` The path of the file to open or create.

Constructs a [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) object with the given file path.


This constructor opens an ofstream to the provided file path in binary mode. If the file does not exist, it will be created when data is written to the stream.




**Parameters:**


* `Path` The path to the file that this writer should operate on. 




        

<hr>



### function FileStreamWriter [3/3]

_This function is a copy constructor for the_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class and it has been explicitly deleted to prevent copying of objects._
```C++
AGE::FileStreamWriter::FileStreamWriter (
    const FileStreamWriter &
) = delete
```





**Parameters:**


* `other` The object to be copied. 



**Returns:**

No return value as this function throws an exception if called.


This function is a copy constructor for the [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) class and it has been explicitly deleted to prevent copying of objects.




**Parameters:**


* `other` The object to be copied.



**Returns:**

No return value as this function does not provide any meaningful output. 





        

<hr>



### function GetStreamPosition 

_Get the current position in the stream._ 
```C++
inline virtual uint64_t AGE::FileStreamWriter::GetStreamPosition () 
```



This function returns the current position within the stream. If an error occurs while trying to get the position, it will return UINT64\_MAX.




**Returns:**

uint64\_t The current position in the stream. Returns UINT64\_MAX if there was an error getting the position.


Get the current position of the stream in bytes.


This function retrieves the current position within the stream, which is typically a file pointer or similar. The return value is cast to uint64\_t for compatibility with large files. If the tellp() call fails (e.g., due to an error condition), it returns UINT64\_MAX to indicate such a failure.




**Returns:**

uint64\_t Current position within the stream in bytes, or UINT64\_MAX if the operation failed. 





        
Implements [*AGE::DataWriter::GetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-getstreamposition)


<hr>



### function IsStreamGood 

_Checks the state of the stream._ 
```C++
inline virtual bool AGE::FileStreamWriter::IsStreamGood () const
```



This function checks whether the underlying stream is in a good state, i.e., it has not encountered any errors or reaching EOF.




**Returns:**

A boolean value indicating if the stream is in a good state (true) or not (false).


Checks the state of the stream object.


This function returns a boolean value indicating whether the stream is in a good state or not. The state of the stream can be determined by calling the `std::basic_ios::good` method on the underlying stream buffer.




**Returns:**

A boolean value that indicates if the stream is in a good state (true) or not (false). 





        
Implements [*AGE::DataWriter::IsStreamGood*](class_a_g_e_1_1_data_writer.md#function-isstreamgood)


<hr>



### function SetStreamPosition 

_Sets the stream position to a specified value._ 
```C++
inline virtual void AGE::FileStreamWriter::SetStreamPosition (
    uint64_t Pos
) 
```



This function sets the current read/write position in the stream to a specific point, defined by an unsigned 64-bit integer parameter 'Pos'. The new position is calculated as (long)Pos, which means it will be truncated if Pos exceeds the maximum value that can be stored in a long.




**Parameters:**


* `Pos` - The desired position to set in the stream.

Sets the stream position to a specific value.


This function sets the current read/write position in the stream to the specified position. The new position is relative to the beginning of the file, which is at offset 0.




**Parameters:**


* `Pos` The desired position in the stream, measured in bytes from the start of the file. 




        
Implements [*AGE::DataWriter::SetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-setstreamposition)


<hr>



### function WriteData 

_Writes data to the file stream._ 
```C++
virtual bool AGE::FileStreamWriter::WriteData (
    const char * Data,
    size_t Size
) 
```



This function writes a block of data of specified size into the file stream. It takes in a pointer to the data and its size, then writes that data into the file stream. The function returns true if the write operation is successful, false otherwise.




**Parameters:**


* `Data` Pointer to the data to be written. 
* `Size` Size of the data to be written. 



**Returns:**

True if the write operation was successful, false otherwise.


Writes data to the file stream.


This function writes a block of data of a specified size into the file stream. The data is written as an array of characters.




**Parameters:**


* `Data` A pointer to the data to be written. 
* `Size` The size of the data in bytes. 



**Returns:**

Returns true if the write operation was successful, false otherwise. This function always returns true because it only writes data and does not check for errors during writing. 





        
Implements [*AGE::DataWriter::WriteData*](class_a_g_e_1_1_data_writer.md#function-writedata)


<hr>



### function ~FileStreamWriter 

_Destructor for the_ [_**FileStreamWriter**_](class_a_g_e_1_1_file_stream_writer.md) _class. Closes the file stream associated with this object._
```C++
virtual AGE::FileStreamWriter::~FileStreamWriter () 
```



Destructor for the [**FileStreamWriter**](class_a_g_e_1_1_file_stream_writer.md) class. Closes the file stream. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataWriter.h`

