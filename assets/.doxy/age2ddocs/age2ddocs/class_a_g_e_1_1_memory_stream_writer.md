

# Class AGE::MemoryStreamWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MemoryStreamWriter**](class_a_g_e_1_1_memory_stream_writer.md)








Inherits the following classes: [AGE::DataWriter](class_a_g_e_1_1_data_writer.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br>_Get the current position of the stream in bytes._  |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br>_Checks the state of the stream object._  |
|   | [**MemoryStreamWriter**](#function-memorystreamwriter-12) (void \* Addr) <br>_Constructs a_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _object with the given address._ |
|   | [**MemoryStreamWriter**](#function-memorystreamwriter-22) (const [**MemoryStreamWriter**](class_a_g_e_1_1_memory_stream_writer.md) &) = delete<br>_This is a copy constructor for the_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _class. It's marked as deleted to prevent copying of objects._ |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br>_Sets the stream position to a specified value._  |
| virtual bool | [**WriteData**](#function-writedata) (const char \* Data, size\_t Size) <br>_Writes data to the memory stream._  |
| virtual  | [**~MemoryStreamWriter**](#function-memorystreamwriter) () <br>_Destructor for_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _class. Clears the stream associated with this object._ |


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




### function GetStreamPosition 

_Get the current position of the stream in bytes._ 
```C++
inline virtual uint64_t AGE::MemoryStreamWriter::GetStreamPosition () 
```



This function retrieves the current position within a stream object, which is useful for determining how much data has been written to the stream so far. The return value is always non-negative and represents the number of characters successfully read from the stream buffer. If an error occurs during reading (e.g., end of file), it returns UINT64\_MAX indicating failure.




**Returns:**

uint64\_t Current position in bytes, or UINT64\_MAX if there was an error.


Get the current position in the stream


This function retrieves the current position within a stream. It returns this as an unsigned 64-bit integer. If the tellp() call fails, it will return UINT64\_MAX to indicate failure.




**Returns:**

uint64\_t The current position in the stream 





        
Implements [*AGE::DataWriter::GetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-getstreamposition)


<hr>



### function IsStreamGood 

_Checks the state of the stream object._ 
```C++
inline virtual bool AGE::MemoryStreamWriter::IsStreamGood () const
```



This function checks whether the underlying input/output operations on the stream are good or not. It returns true if the stream is in a good state, false otherwise.




**Returns:**

True if the stream is in a good state, false otherwise.


Checks the state of the stream.


This function checks whether the underlying stream is in a good state, i.e., it has no errors or failures that would prevent further operations on it.




**Returns:**

True if the stream is in a good state, false otherwise. 





        
Implements [*AGE::DataWriter::IsStreamGood*](class_a_g_e_1_1_data_writer.md#function-isstreamgood)


<hr>



### function MemoryStreamWriter [1/2]

_Constructs a_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _object with the given address._
```C++
AGE::MemoryStreamWriter::MemoryStreamWriter (
    void * Addr
) 
```



This constructor initializes the memory stream writer with an address to write data into. The mode of the stream is set to binary and out for writing operations.




**Parameters:**


* `Addr` A void pointer representing the starting address in memory where data will be written.

Constructs a [**MemoryStreamWriter**](class_a_g_e_1_1_memory_stream_writer.md) object with the given address.


This constructor initializes the memory stream writer with an address to write data into. The stream is initialized as binary and outgoing.




**Parameters:**


* `Addr` A void pointer representing the address where data will be written. 




        

<hr>



### function MemoryStreamWriter [2/2]

_This is a copy constructor for the_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _class. It's marked as deleted to prevent copying of objects._
```C++
AGE::MemoryStreamWriter::MemoryStreamWriter (
    const MemoryStreamWriter &
) = delete
```





**Parameters:**


* `other` The object to be copied.

This is a copy constructor for the [**MemoryStreamWriter**](class_a_g_e_1_1_memory_stream_writer.md) class. It's marked as deleted to prevent copying of objects. 

**Parameters:**


* `other` The object to be copied. 




        

<hr>



### function SetStreamPosition 

_Sets the stream position to a specified value._ 
```C++
inline virtual void AGE::MemoryStreamWriter::SetStreamPosition (
    uint64_t Pos
) 
```



This function sets the current read/write position in the stream to the provided position. The new position is calculated as an offset from the beginning of the file, which is given by the parameter 'Pos'.




**Parameters:**


* `Pos` The new position to set in the stream.

Sets the stream position to a specified value.


This function sets the current read/write position in the stream to the provided position. The new position is calculated as an offset from the beginning of the file, measured in bytes.




**Parameters:**


* `Pos` The desired position in the stream, measured in bytes. 




        
Implements [*AGE::DataWriter::SetStreamPosition*](class_a_g_e_1_1_data_writer.md#function-setstreamposition)


<hr>



### function WriteData 

_Writes data to the memory stream._ 
```C++
virtual bool AGE::MemoryStreamWriter::WriteData (
    const char * Data,
    size_t Size
) 
```



This function writes a block of data of specified size into the memory stream. It takes in a pointer to the data and its size, then writes that data into the stream. The function returns true if the write operation is successful, false otherwise.




**Parameters:**


* `Data` Pointer to the data to be written. 
* `Size` Size of the data to be written.



**Returns:**

True if the write operation was successful, false otherwise.


Writes data to the memory stream.


This function writes a block of data of a specified size into the memory stream. It takes in a pointer to the data and its size, then writes this data into the stream. The function returns true if the write operation is successful, false otherwise.




**Parameters:**


* `Data` Pointer to the data that needs to be written into the stream. 
* `Size` Size of the data block in bytes.



**Returns:**

True if the data was successfully written into the memory stream, false otherwise. 





        
Implements [*AGE::DataWriter::WriteData*](class_a_g_e_1_1_data_writer.md#function-writedata)


<hr>



### function ~MemoryStreamWriter 

_Destructor for_ [_**MemoryStreamWriter**_](class_a_g_e_1_1_memory_stream_writer.md) _class. Clears the stream associated with this object._
```C++
virtual AGE::MemoryStreamWriter::~MemoryStreamWriter () 
```



Destructor for [**MemoryStreamWriter**](class_a_g_e_1_1_memory_stream_writer.md) class. Clears the stream associated with this instance. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataWriter.h`

