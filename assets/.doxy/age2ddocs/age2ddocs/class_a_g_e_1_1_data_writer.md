

# Class AGE::DataWriter



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**DataWriter**](class_a_g_e_1_1_data_writer.md)










Inherited by the following classes: [AGE::FileStreamWriter](class_a_g_e_1_1_file_stream_writer.md),  [AGE::MemoryStreamWriter](class_a_g_e_1_1_memory_stream_writer.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const = 0<br> |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|  void | [**WriteArray**](#function-writearray) (const std::vector&lt; T &gt; & Array, bool WriteSize=true) <br>_Writes an array to a stream._  |
|  void | [**WriteBuffer**](#function-writebuffer) ([**Buffer**](struct_a_g_e_1_1_buffer.md) buffer, bool WriteSize=true) <br>_Writes a buffer to the data stream._  |
| virtual bool | [**WriteData**](#function-writedata) (const char \* Data, size\_t Size) = 0<br> |
|  void | [**WriteMap**](#function-writemap-13) (const std::map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br>_Writes a map to the underlying storage._  |
|  void | [**WriteMap**](#function-writemap-23) (const std::unordered\_map&lt; Key, Value &gt; & Map, bool WriteSize=true) <br>_This function writes an unordered map to a data stream. It can optionally write the size of the map as well._  |
|  void | [**WriteMap**](#function-writemap-33) (const std::unordered\_map&lt; std::string, Value &gt; & Map, bool WriteSize=true) <br>_Writes a map to the stream. If WriteSize is true, it writes the size of the map first. Then for each key-value pair in the map, it writes the key as a string and the value. For trivial types, it directly writes the value using WriteRaw. For non-trivial types, it uses WriteObject._  |
|  void | [**WriteObject**](#function-writeobject) (const T & Obj) <br>_This function writes an object to the stream by serializing it._  |
|  void | [**WriteRaw**](#function-writeraw) (const T & Type) <br>_Writes raw data of a specific type._  |
|  void | [**WriteString**](#function-writestring) (const std::string & String) <br>_Writes a string to the data stream, including its length prefix._  |
|  void | [**WriteZero**](#function-writezero) (uint64\_t Size) <br>_Writes a block of zeros to the data stream._  |
|   | [**operator bool**](#function-operator-bool) () const<br>_Checks the state of the stream._  |
| virtual  | [**~DataWriter**](#function-datawriter) () = default<br>_Virtual destructor for the_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _class._ |




























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

_Writes an array to a stream._ 
```C++
template<typename T>
inline void AGE::DataWriter::WriteArray (
    const std::vector< T > & Array,
    bool WriteSize=true
) 
```



This function writes the elements of an array to a stream, optionally also writing its size. The type T must be trivially serializable or have a custom serialization method.




**Parameters:**


* `Array` The array to write. 
* `WriteSize` If true, the size of the array will be written first. Defaults to true.

Writes an array to a data stream.


This function writes the elements of an array to a data stream, optionally including its size as well. The type `T` is expected to be trivially copyable or serializable. If it's not, then the object-specific write method (WriteObject&lt;T&gt;) will be used instead.




**Parameters:**


* `Array` A const reference to the array that should be written. 
* `WriteSize` An optional boolean indicating whether the size of the array should also be written. Default is true. 




        

<hr>



### function WriteBuffer 

_Writes a buffer to the data stream._ 
```C++
void AGE::DataWriter::WriteBuffer (
    Buffer buffer,
    bool WriteSize=true
) 
```



This function writes a given buffer to the data stream. If the WriteSize parameter is true, it will first write the size of the buffer to the stream. The buffer's data and its size are then written to the stream. 

**Parameters:**


* `buffer` The buffer to be written. 
* `WriteSize` A flag indicating whether or not to write the size of the buffer to the stream.



**Returns:**

void


Writes a buffer to the data stream.


This function writes a given buffer to the data stream. It first checks if the WriteSize parameter is true and if so, it writes the size of the buffer as a uint64\_t. Then it writes the actual data of the buffer. 

**Parameters:**


* `buffer` The buffer to be written. 
* `WriteSize` A flag indicating whether or not to write the size of the buffer. 




        

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

_Writes a map to the underlying storage._ 
```C++
template<typename Key, typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::map< Key, Value > & Map,
    bool WriteSize=true
) 
```



This function writes a given map to the underlying storage. If WriteSize is true, it first writes the size of the map. Then for each key-value pair in the map, it checks if the Key and Value types are trivial (i.e., they can be copied using memcpy). If so, it directly writes them; otherwise, it uses a more complex serialization method.




**Parameters:**


* `Map` The map to write. 
* `WriteSize` Whether or not to write the size of the map first. Defaults to true.



**Returns:**

void


Writes a map to the stream. If WriteSize is true, it writes the size of the map first. Then for each pair in the map, if Key and Value are trivial types, they are written directly; otherwise, WriteObject function is used. 

**Parameters:**


* `Map` The map to be written. 
* `WriteSize` If true, write the size of the map before writing pairs. Defaults to true. 




        

<hr>



### function WriteMap [2/3]

_This function writes an unordered map to a data stream. It can optionally write the size of the map as well._ 
```C++
template<typename Key, typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::unordered_map< Key, Value > & Map,
    bool WriteSize=true
) 
```





**Parameters:**


* `Map` The unordered map to be written. 
* `WriteSize` A flag indicating whether or not to write the size of the map. Defaults to true.

Writes a map to the underlying storage.


This function writes an unordered\_map to the underlying storage. If WriteSize is true, it first writes the size of the map. Then for each key-value pair in the map, if the key and value types are trivial (i.e., they can be copied using memcpy), it directly writes them; otherwise, it uses a more complex serialization method.




**Parameters:**


* `Map` The unordered\_map to write. 
* `WriteSize` Whether or not to write the size of the map first. Defaults to true. 



**Returns:**

void 





        

<hr>



### function WriteMap [3/3]

_Writes a map to the stream. If WriteSize is true, it writes the size of the map first. Then for each key-value pair in the map, it writes the key as a string and the value. For trivial types, it directly writes the value using WriteRaw. For non-trivial types, it uses WriteObject._ 
```C++
template<typename Value>
inline void AGE::DataWriter::WriteMap (
    const std::unordered_map< std::string, Value > & Map,
    bool WriteSize=true
) 
```





**Parameters:**


* `Map` The unordered\_map to write. 
* `WriteSize` Whether or not to write the size of the map first. Defaults to true. 



**Returns:**

None


Writes a map to the stream. If WriteSize is true, it writes the size of the map first. Then for each key-value pair in the map, it writes the key and value. For non-trivial types, it uses WriteObject function, otherwise it directly writes the value using WriteRaw function. 

**Parameters:**


* `Map` The unordered\_map to be written. 
* `WriteSize` A flag indicating whether or not to write the size of the map first. Defaults to true. 



**Returns:**

None 





        

<hr>



### function WriteObject 

_This function writes an object to the stream by serializing it._ 
```C++
template<typename T>
inline void AGE::DataWriter::WriteObject (
    const T & Obj
) 
```





**Parameters:**


* `const` T& Obj - The reference to the object that needs to be written.

This function writes an object to the stream by serializing it using a static method.




**Parameters:**


* `const` T& Obj - A constant reference to the object that needs to be written. The type of this object must have a Serialize() method defined for it. 




        

<hr>



### function WriteRaw 

_Writes raw data of a specific type._ 
```C++
template<typename T>
inline void AGE::DataWriter::WriteRaw (
    const T & Type
) 
```



This function writes raw data into the game file using the `WriteData` method. It takes an object of any type as input and converts it to a byte array before writing it. The size of this byte array is determined by the sizeof operator, which allows for different types to be handled uniformly.




**Parameters:**


* `Type` An object of any type that can be converted into raw data. 



**Returns:**

void


Writes raw data of a specific type.


This function writes raw data into the game file using the provided data and its size. It ensures that all data is written correctly by checking if the write operation was successful.




**Parameters:**


* `Type` The reference to the data to be written. 



**Returns:**

void 





        

<hr>



### function WriteString 

_Writes a string to the data stream, including its length prefix._ 
```C++
void AGE::DataWriter::WriteString (
    const std::string & String
) 
```





**Parameters:**


* `String` The string to write. 



**Returns:**

None.


Writes a string to the data stream, including its length prefix. 

**Parameters:**


* `String` The string to write. 




        

<hr>



### function WriteZero 

_Writes a block of zeros to the data stream._ 
```C++
void AGE::DataWriter::WriteZero (
    uint64_t Size
) 
```



This function writes a specified number of zero bytes to the data stream. It uses a loop to write each byte individually.




**Parameters:**


* `Size` The number of zero bytes to write.

Writes a block of zeros to the data stream.


This function writes a specified number of zero bytes to the data stream. The size of the block is determined by the input parameter 'Size'.




**Parameters:**


* `Size` The number of zero bytes to write to the data stream. 




        

<hr>



### function operator bool 

_Checks the state of the stream._ 
```C++
inline AGE::DataWriter::operator bool () const
```



This function returns a boolean value indicating whether or not the underlying stream is in a good state. It does this by calling the private method `IsStreamGood()`, which should be implemented elsewhere in the class.




**Returns:**

A boolean value indicating if the stream is in a good state.


Checks the state of the stream.


This function returns a boolean value indicating whether or not the stream is in a good state. It does this by calling the private method `IsStreamGood()`, which should be implemented elsewhere in the class.




**Returns:**

bool - Returns true if the stream is in a good state, false otherwise. 





        

<hr>



### function ~DataWriter 

_Virtual destructor for the_ [_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _class._
```C++
virtual AGE::DataWriter::~DataWriter () = default
```



This function is responsible for freeing any resources that were allocated by the [**DataWriter**](class_a_g_e_1_1_data_writer.md) object, such as memory or file handles. It does not return anything (void) and thus it doesn't need a Doxygen comment to explain its behavior.


Virtual destructor for the [**DataWriter**](class_a_g_e_1_1_data_writer.md) class.


This function is responsible for releasing any resources that were acquired by the object during its lifetime, such as memory or file handles. It does not return anything and has no parameters. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataWriter.h`

