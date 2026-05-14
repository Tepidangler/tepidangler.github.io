

# Class AGE::FileStreamReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md)








Inherits the following classes: [AGE::DataReader](class_a_g_e_1_1_data_reader.md)






















































## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**FileStreamReader**](#function-filestreamreader-13) () = default<br>_Default constructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class._ |
|   | [**FileStreamReader**](#function-filestreamreader-23) (const std::filesystem::path & Path) <br>_Constructs a_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _object with the given file path._ |
|   | [**FileStreamReader**](#function-filestreamreader-33) (const [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) &) = delete<br>_This function is a copy constructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class and it has been explicitly deleted to prevent copying of objects._ |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () <br>_Get the current position of the stream._  |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const<br>_Checks the state of the stream object._  |
| virtual bool | [**ReadBytes**](#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) <br>_Reads a specified number of bytes from the stream into a vector._  |
| virtual bool | [**ReadBytes**](#function-readbytes-22) (uint8\_t \* Data, size\_t Size) <br>_Reads a specified number of bytes from the stream into a buffer._  |
| virtual bool | [**ReadData**](#function-readdata) (char \* Data, size\_t Size) <br>_Reads data from the stream into a buffer._  |
| virtual bool | [**ReadJson**](#function-readjson) (std::string & String) <br>_Reads a JSON string from the stream and stores it in the provided string reference. The size of the JSON string is read first, then the actual data is read into a string of that size._  |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) <br>_This function sets the stream position to a specific value._  |
| virtual  | [**~FileStreamReader**](#function-filestreamreader) () <br>_Destructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class. Closes the file stream if it is open._ |


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




### function FileStreamReader [1/3]

_Default constructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class._
```C++
AGE::FileStreamReader::FileStreamReader () = default
```



This function initializes a new instance of the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class with default settings. It does not open any file or stream, but sets up the object to handle reading from files and streams in the future.




**Returns:**

A new instance of the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class with no associated file or stream.


Default constructor for the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class.


This function initializes a new instance of the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class with default settings. It does not open any file streams or initialize any other resources.




**Returns:**

A newly constructed [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) object. 





        

<hr>



### function FileStreamReader [2/3]

_Constructs a_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _object with the given file path._
```C++
AGE::FileStreamReader::FileStreamReader (
    const std::filesystem::path & Path
) 
```



This constructor opens an ifstream in binary mode for reading from the provided file path. The opened stream is stored in m\_Stream member variable.




**Parameters:**


* `Path` The file path to open as a stream.

Constructs a [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) object with the given file path.


This constructor opens an ifstream in binary mode for reading from the provided file path. The opened stream is stored in m\_Stream member variable.




**Parameters:**


* `Path` The file path to open as a stream. 




        

<hr>



### function FileStreamReader [3/3]

_This function is a copy constructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class and it has been explicitly deleted to prevent copying of objects._
```C++
AGE::FileStreamReader::FileStreamReader (
    const FileStreamReader &
) = delete
```





**Parameters:**


* `other` The object to be copied from.



**Returns:**

No return value as this function does not return anything.


This function is a copy constructor for the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class and it has been explicitly deleted to prevent copying of objects.




**Parameters:**


* `other` The object to be copied. 




        

<hr>



### function GetStreamPosition 

_Get the current position of the stream._ 
```C++
inline virtual uint64_t AGE::FileStreamReader::GetStreamPosition () 
```



This function returns the current position in the stream. If the tellg() call fails, it will return UINT64\_MAX to indicate an error.




**Returns:**

uint64\_t The current position in the stream.


Get the current position of the stream


This function returns the current position in the stream. It uses a platform-specific method to get the position, and handles any errors that may occur.




**Returns:**

uint64\_t The current position in the stream. If an error occurs, it returns UINT64\_MAX. 





        
Implements [*AGE::DataReader::GetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-getstreamposition)


<hr>



### function IsStreamGood 

_Checks the state of the stream object._ 
```C++
inline virtual bool AGE::FileStreamReader::IsStreamGood () const
```



This function checks whether the underlying input/output operations on the stream are good or not. It returns true if the stream is in a good state, false otherwise.




**Returns:**

A boolean value indicating the health of the stream. True means the stream is in a good state, while false indicates an error has occurred.


Checks the state of the stream.


This function checks whether the underlying stream is in a good state, i.e., it has no errors or failures that would prevent further operations on it.




**Returns:**

True if the stream is in a good state; false otherwise. 





        
Implements [*AGE::DataReader::IsStreamGood*](class_a_g_e_1_1_data_reader.md#function-isstreamgood)


<hr>



### function ReadBytes [1/2]

_Reads a specified number of bytes from the stream into a vector._ 
```C++
virtual bool AGE::FileStreamReader::ReadBytes (
    std::vector< std::byte > & Data,
    size_t Size
) 
```



This function reads 'Size' bytes from the underlying stream and stores them in the provided vector, 'Data'. The data is read as raw byte values (std::byte), so it can be used with any type that requires byte-level access.




**Parameters:**


* `Data` A reference to a std::vector of std::bytes where the read bytes will be stored. 
* `Size` The number of bytes to read from the stream. 



**Returns:**

bool Returns true if the operation was successful, false otherwise (e.g., end-of-file or error).


Reads a specified number of bytes from the stream into a vector.


This function reads a specified number of bytes from the underlying input stream, storing them in a provided vector. The size of the data read is determined by the 'Size' parameter.




**Parameters:**


* `Data` A reference to a std::vector&lt;std::byte&gt; where the read data will be stored. 
* `Size` The number of bytes to read from the stream.



**Returns:**

Returns true if the operation was successful, false otherwise (e.g., end-of-file or error). 





        
Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-12)


<hr>



### function ReadBytes [2/2]

_Reads a specified number of bytes from the stream into a buffer._ 
```C++
virtual bool AGE::FileStreamReader::ReadBytes (
    uint8_t * Data,
    size_t Size
) 
```



This function reads a specified number of bytes from the underlying input stream into a provided buffer. The size of the data read is determined by the 'Size' parameter.




**Parameters:**


* `Data` A pointer to the buffer where the read data will be stored. 
* `Size` The number of bytes to read from the stream. 



**Returns:**

Returns true if the operation was successful, false otherwise. In this case, it always returns true as there is no way for an error to occur in this function.


ReadBytes reads a specified number of bytes from the stream into a buffer.


This function attempts to read 'Size' bytes from the file stream and store them in the provided buffer 'Data'. The function returns true if it was able to successfully read all requested bytes, false otherwise.




**Parameters:**


* `Data` Pointer to the buffer where the data will be stored. 
* `Size` Number of bytes to read. 



**Returns:**

True if successful, false otherwise. 





        
Implements [*AGE::DataReader::ReadBytes*](class_a_g_e_1_1_data_reader.md#function-readbytes-22)


<hr>



### function ReadData 

_Reads data from the stream into a buffer._ 
```C++
virtual bool AGE::FileStreamReader::ReadData (
    char * Data,
    size_t Size
) 
```



This function reads 'Size' bytes of data from the file stream into the character array pointed to by 'Data'. The read operation is performed using the standard library method std::basic\_istream&lt;char&gt;::read(). If successful, it returns true; otherwise, false.




**Parameters:**


* `Data` Pointer to a buffer where the data will be stored. 
* `Size` Number of bytes to read from the stream. 



**Returns:**

True if the operation was successful, false otherwise.


Reads data from the stream into a buffer.


This function reads a specified number of bytes from the stream into a provided buffer. The size of the buffer is passed as an argument, and the actual amount read may be less if there are fewer than 'Size' bytes left in the stream.




**Parameters:**


* `Data` Pointer to the buffer where the data will be stored. 
* `Size` Number of bytes to read from the stream. 



**Returns:**

Returns true on success, false otherwise (e.g., if the end of the file is reached). 





        
Implements [*AGE::DataReader::ReadData*](class_a_g_e_1_1_data_reader.md#function-readdata)


<hr>



### function ReadJson 

_Reads a JSON string from the stream and stores it in the provided string reference. The size of the JSON string is read first, then the actual data is read into a string of that size._ 
```C++
virtual bool AGE::FileStreamReader::ReadJson (
    std::string & String
) 
```





**Parameters:**


* `String` Reference to a string where the JSON data will be stored. 



**Returns:**

True if successful, false otherwise.


Reads a JSON string from the stream and stores it in the provided string reference. The size of the JSON string is read first, then the actual data is read into a string buffer.




**Parameters:**


* `String` Reference to a string where the JSON data will be stored. 



**Returns:**

True if successful, false otherwise. This function always returns true as it should not fail in this context. 





        
Implements [*AGE::DataReader::ReadJson*](class_a_g_e_1_1_data_reader.md#function-readjson)


<hr>



### function SetStreamPosition 

_This function sets the stream position to a specific value._ 
```C++
inline virtual void AGE::FileStreamReader::SetStreamPosition (
    uint64_t Pos
) 
```





**Parameters:**


* `Pos` The new position in bytes from the beginning of the stream.

This function sets the stream position to a specified value. 

**Parameters:**


* `Pos` The new position in bytes from the beginning of the stream. 




        
Implements [*AGE::DataReader::SetStreamPosition*](class_a_g_e_1_1_data_reader.md#function-setstreamposition)


<hr>



### function ~FileStreamReader 

_Destructor for the_ [_**FileStreamReader**_](class_a_g_e_1_1_file_stream_reader.md) _class. Closes the file stream if it is open._
```C++
virtual AGE::FileStreamReader::~FileStreamReader () 
```



Destructor for the [**FileStreamReader**](class_a_g_e_1_1_file_stream_reader.md) class. Closes the file stream if it is open. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataReader.h`

