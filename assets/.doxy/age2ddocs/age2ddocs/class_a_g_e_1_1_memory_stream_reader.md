

# Class AGE::MemoryStreamReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**MemoryStreamReader**](class_a_g_e_1_1_memory_stream_reader.md)








Inherits the following classes: [AGE::DataReader](class_a_g_e_1_1_data_reader.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br>_Get the current position of the stream._  |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br>_Checks the state of the stream._  |
|   | [**MemoryStreamReader**](#function-memorystreamreader-12) (void \* Addr, size\_t Size) <br>_Constructor for_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class. Initializes a memory stream reader with the given address and size._ |
|   | [**MemoryStreamReader**](#function-memorystreamreader-22) (const [**MemoryStreamReader**](class_a_g_e_1_1_memory_stream_reader.md) &) = delete<br>_Constructs a new instance of the_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class using an existing memory stream._ |
| virtual bool | [**ReadBytes**](#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) <br>_Reads a specified number of bytes from the stream into a vector._  |
| virtual bool | [**ReadBytes**](#function-readbytes-22) (uint8\_t \* Data, size\_t Size) <br>_Reads a specified number of bytes from the stream into a buffer._  |
| virtual bool | [**ReadData**](#function-readdata) (char \* Data, size\_t Size) <br>_Reads data from the stream into a buffer._  |
| virtual bool | [**ReadJson**](#function-readjson) (std::string & String) <br>_Reads a JSON string from the memory stream._  |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br>_This function sets the stream position to a specified value._  |
| virtual  | [**~MemoryStreamReader**](#function-memorystreamreader) () <br>_Destructor for_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class. Clears the stream of any error flags._ |


## Public Functions inherited from AGE::DataReader

See [AGE::DataReader](class_a_g_e_1_1_data_reader.md)

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](class_a_g_e_1_1_data_reader.md#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](class_a_g_e_1_1_data_reader.md#function-isstreamgood) () const = 0<br> |
|  void | [**ReadArray**](class_a_g_e_1_1_data_reader.md#function-readarray) (std::vector&lt; T &gt; & Array, uint32\_t Size=0) <br>_Reads an array of elements from the input stream. If the size is not provided, it reads the size first and then the array. The function uses C++14's std::is\_trivial to determine whether T is a trivial type or not. For trivial types, it directly reads into the array element using ReadRaw. For non-trivial types, it uses ReadObject._  |
|  void | [**ReadBuffer**](class_a_g_e_1_1_data_reader.md#function-readbuffer) (char \* Data, size\_t Size) <br>_Reads data from the buffer. If size is zero, it reads a uint32\_t to determine the size of the data to read next._  |
| virtual bool | [**ReadBytes**](class_a_g_e_1_1_data_reader.md#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadBytes**](class_a_g_e_1_1_data_reader.md#function-readbytes-22) (uint8\_t \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadData**](class_a_g_e_1_1_data_reader.md#function-readdata) (char \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadJson**](class_a_g_e_1_1_data_reader.md#function-readjson) (std::string & String) = 0<br> |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-13) (std::map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream._  |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-23) (std::unordered\_map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream._  |
|  void | [**ReadMap**](class_a_g_e_1_1_data_reader.md#function-readmap-33) (std::unordered\_map&lt; std::string, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream. The size of the map is read if not provided as an argument. If the key and value types are trivial, raw data is read directly; otherwise, objects are read._  |
|  void | [**ReadObject**](class_a_g_e_1_1_data_reader.md#function-readobject) (T & Obj) <br>_This function reads an object of type T from the stream using Deserialize method._  |
|  void | [**ReadRaw**](class_a_g_e_1_1_data_reader.md#function-readraw) (T & Type) <br>_This function reads raw data into a specified type._  |
|  void | [**ReadString**](class_a_g_e_1_1_data_reader.md#function-readstring) (std::string & String) <br>_Reads a string from the data source._  |
| virtual void | [**SetStreamPosition**](class_a_g_e_1_1_data_reader.md#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|   | [**operator bool**](class_a_g_e_1_1_data_reader.md#function-operator-bool) () const<br>_Checks the state of the stream._  |
| virtual  | [**~DataReader**](class_a_g_e_1_1_data_reader.md#function-datareader) () = default<br>_Virtual destructor for the_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _class._ |






















































## Public Functions Documentation




### function GetStreamPosition 

_Get the current position of the stream._ 
```C++
inline virtual uint64_t AGE::MemoryStreamReader::GetStreamPosition () 
```



This function returns the current position in the stream. If an error occurs while trying to get the position, it will return UINT64\_MAX. The behavior is platform-dependent and depends on whether **clang** is defined or not. For Clang, if tellg() fails (returns -1), this function returns UINT64\_MAX. Otherwise, it converts the result to uint64\_t and returns it. For other platforms, it simply calls tellg(). This means that the return value is always a valid position in the stream.




**Returns:**

The current position of the stream as an unsigned 64-bit integer. If an error occurs while trying to get the position, UINT64\_MAX is returned.


Get the current position of the stream


This function retrieves the current position in the stream. It uses a platform-specific method to do so, and handles any errors that may occur. On platforms where `tellg()` returns -1 on failure (such as Clang), it instead returns UINT64\_MAX to indicate an error state.




**Returns:**

uint64\_t The current position in the stream, or UINT64\_MAX if there was an error getting the position 





        
Implements [*AGE::DataReader::GetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-getstreamposition)


<hr>



### function IsStreamGood 

_Checks the state of the stream._ 
```C++
inline virtual bool AGE::MemoryStreamReader::IsStreamGood () const
```



This function checks whether the underlying input/output stream is in a good state, i.e., it has no errors or failures that would prevent further operations on it.




**Returns:**

A boolean value indicating if the stream is in a good state (true) or not (false).


Checks the state of the stream.


This function checks whether the underlying input-output operations on the stream are good or not. It returns true if the stream is in a good state, false otherwise.




**Returns:**

True if the stream is in a good state, false otherwise. 





        
Implements [*AGE::DataReader::IsStreamGood*](class_a_g_e_1_1_data_reader.md#function-isstreamgood)


<hr>



### function MemoryStreamReader [1/2]

_Constructor for_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class. Initializes a memory stream reader with the given address and size._
```C++
AGE::MemoryStreamReader::MemoryStreamReader (
    void * Addr,
    size_t Size
) 
```





**Parameters:**


* `Addr` Pointer to the start of the data buffer. 
* `Size` The size of the data in bytes.

Constructor for [**MemoryStreamReader**](class_a_g_e_1_1_memory_stream_reader.md). Initializes the object with a given memory address and size. 

**Parameters:**


* `Addr` Pointer to the memory location to be read from. 
* `Size` The size of the data in bytes at the provided memory location. 




        

<hr>



### function MemoryStreamReader [2/2]

_Constructs a new instance of the_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class using an existing memory stream._
```C++
AGE::MemoryStreamReader::MemoryStreamReader (
    const MemoryStreamReader &
) = delete
```



The constructor takes in a reference to an existing memory stream and sets it as the source for reading data. It also initializes the read position to zero.




**Parameters:**


* `mem_stream` A reference to an existing memory stream that will be used as the source of data.

Constructor for the [**MemoryStreamReader**](class_a_g_e_1_1_memory_stream_reader.md) class. It is deleted to prevent copying of objects.




**Parameters:**


* `other` The object to be copied. This parameter is not used in this function as it's a copy constructor and does nothing. 




        

<hr>



### function ReadBytes [1/2]

_Reads a specified number of bytes from the stream into a vector._ 
```C++
virtual bool AGE::MemoryStreamReader::ReadBytes (
    std::vector< std::byte > & Data,
    size_t Size
) 
```



This function reads a specified number of bytes from the underlying stream and stores them in a provided vector. The data is read as raw byte values, so it can be used with any type that supports std::byte.




**Parameters:**


* `Data` A reference to a vector where the read bytes will be stored. 
* `Size` The number of bytes to read from the stream. 



**Returns:**

Always returns true. In future this may change if we decide to add error handling for when not enough data is available in the stream.


Reads a specified number of bytes from the stream into a vector.


This function reads 'Size' bytes from the underlying stream and stores them in the provided vector, 'Data'. The data is read as raw byte values (std::byte), so it can be used with any type that supports these operations.




**Parameters:**


* `Data` A reference to a std::vector of std::bytes where the read data will be stored. 
* `Size` The number of bytes to read from the stream. 



**Returns:**

Returns true if the operation was successful, false otherwise (e.g., if there is an error in reading or EOF has been reached). 





        
Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-12)


<hr>



### function ReadBytes [2/2]

_Reads a specified number of bytes from the stream into a buffer._ 
```C++
virtual bool AGE::MemoryStreamReader::ReadBytes (
    uint8_t * Data,
    size_t Size
) 
```



This function reads a specified number of bytes from the underlying input stream, storing them in a provided buffer. The size of the data read is determined by the 'Size' parameter.




**Parameters:**


* `Data` Pointer to the buffer where the read data will be stored. 
* `Size` Number of bytes to read from the stream. 



**Returns:**

Returns true if the operation was successful, false otherwise (e.g., end of file).


Reads a specified number of bytes from the stream into a buffer.


This function reads a specified number of bytes from the underlying input stream into a provided buffer. The size of the data read is determined by the 'Size' parameter.




**Parameters:**


* `Data` A pointer to the buffer where the read data will be stored. 
* `Size` The number of bytes to read from the stream. 



**Returns:**

Returns true if the operation was successful, false otherwise. In this case, it always returns true as there are no failure conditions for reading from the stream. 





        
Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-22)


<hr>



### function ReadData 

_Reads data from the stream into a buffer._ 
```C++
virtual bool AGE::MemoryStreamReader::ReadData (
    char * Data,
    size_t Size
) 
```



This function reads 'Size' bytes of data from the stream and stores it in the buffer pointed to by 'Data'. The function returns true if successful, false otherwise.




**Parameters:**


* `Data` Pointer to the buffer where the read data will be stored. 
* `Size` Number of bytes to read from the stream. 



**Returns:**

True if successful, false otherwise.


Reads data from the stream into a buffer.


This function reads 'Size' bytes of data from the stream and stores it in the buffer pointed to by 'Data'. The function returns true if successful, false otherwise.




**Parameters:**


* `Data` Pointer to the buffer where the read data will be stored. 
* `Size` Number of bytes to read from the stream. 



**Returns:**

True if the operation was successful, false otherwise. 





        
Implements [*AGE::DataReader::ReadData*](class_a_g_e_1_1_data_reader.md#function-readdata)


<hr>



### function ReadJson 

_Reads a JSON string from the memory stream._ 
```C++
virtual bool AGE::MemoryStreamReader::ReadJson (
    std::string & String
) 
```



This function attempts to read a JSON string from the memory stream and stores it in the provided string reference parameter. If successful, the function returns true; otherwise, false is returned.




**Parameters:**


* `String` A reference to a std::string object where the JSON string will be stored. 



**Returns:**

bool Returns true if the operation was successful, and false otherwise.


Reads a JSON string from the memory stream.


This function attempts to read a JSON string from the memory stream and stores it in the provided string reference. If successful, it returns true, otherwise it returns false.




**Parameters:**


* `String` A reference to a std::string where the JSON string will be stored. 



**Returns:**

bool Returns true if the operation was successful, false otherwise. 





        
Implements [*AGE::DataReader::ReadJson*](class_a_g_e_1_1_data_reader.md#function-readjson)


<hr>



### function SetStreamPosition 

_This function sets the stream position to a specified value._ 
```C++
inline virtual void AGE::MemoryStreamReader::SetStreamPosition (
    uint64_t Pos
) 
```





**Parameters:**


* `Pos` The new position in bytes from the beginning of the stream.

Sets the stream position to a specified value.


This function sets the current read/write position in the stream to a specific byte offset from the beginning of the file. The new position is determined by the input parameter 'Pos'.




**Parameters:**


* `Pos` The desired position within the stream, measured in bytes from the start of the file. 




        
Implements [*AGE::DataReader::SetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-setstreamposition)


<hr>



### function ~MemoryStreamReader 

_Destructor for_ [_**MemoryStreamReader**_](class_a_g_e_1_1_memory_stream_reader.md) _class. Clears the stream of any error flags._
```C++
virtual AGE::MemoryStreamReader::~MemoryStreamReader () 
```



Destructor for [**MemoryStreamReader**](class_a_g_e_1_1_memory_stream_reader.md) class. Clears the stream of any error flags. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataReader.h`

