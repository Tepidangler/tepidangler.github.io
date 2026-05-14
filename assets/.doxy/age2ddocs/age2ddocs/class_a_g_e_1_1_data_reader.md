

# Class AGE::DataReader



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**DataReader**](class_a_g_e_1_1_data_reader.md)










Inherited by the following classes: [AGE::FileStreamReader](class_a_g_e_1_1_file_stream_reader.md),  [AGE::MemoryStreamReader](class_a_g_e_1_1_memory_stream_reader.md)
































## Public Functions

| Type | Name |
| ---: | :--- |
| virtual uint64\_t | [**GetStreamPosition**](#function-getstreamposition) () = 0<br> |
| virtual bool | [**IsStreamGood**](#function-isstreamgood) () const = 0<br> |
|  void | [**ReadArray**](#function-readarray) (std::vector&lt; T &gt; & Array, uint32\_t Size=0) <br>_Reads an array of elements from the input stream. If the size is not provided, it reads the size first and then the array. The function uses C++14's std::is\_trivial to determine whether T is a trivial type or not. For trivial types, it directly reads into the array element using ReadRaw. For non-trivial types, it uses ReadObject._  |
|  void | [**ReadBuffer**](#function-readbuffer) (char \* Data, size\_t Size) <br>_Reads data from the buffer. If size is zero, it reads a uint32\_t to determine the size of the data to read next._  |
| virtual bool | [**ReadBytes**](#function-readbytes-12) (std::vector&lt; std::byte &gt; & Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadBytes**](#function-readbytes-22) (uint8\_t \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadData**](#function-readdata) (char \* Data, size\_t Size) = 0<br> |
| virtual bool | [**ReadJson**](#function-readjson) (std::string & String) = 0<br> |
|  void | [**ReadMap**](#function-readmap-13) (std::map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream._  |
|  void | [**ReadMap**](#function-readmap-23) (std::unordered\_map&lt; Key, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream._  |
|  void | [**ReadMap**](#function-readmap-33) (std::unordered\_map&lt; std::string, Value &gt; & Map, uint32\_t Size=0) <br>_Reads a map from the input stream. The size of the map is read if not provided as an argument. If the key and value types are trivial, raw data is read directly; otherwise, objects are read._  |
|  void | [**ReadObject**](#function-readobject) (T & Obj) <br>_This function reads an object of type T from the stream using Deserialize method._  |
|  void | [**ReadRaw**](#function-readraw) (T & Type) <br>_This function reads raw data into a specified type._  |
|  void | [**ReadString**](#function-readstring) (std::string & String) <br>_Reads a string from the data source._  |
| virtual void | [**SetStreamPosition**](#function-setstreamposition) (uint64\_t Pos) = 0<br> |
|   | [**operator bool**](#function-operator-bool) () const<br>_Checks the state of the stream._  |
| virtual  | [**~DataReader**](#function-datareader) () = default<br>_Virtual destructor for the_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _class._ |




























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

_Reads an array of elements from the input stream. If the size is not provided, it reads the size first and then the array. The function uses C++14's std::is\_trivial to determine whether T is a trivial type or not. For trivial types, it directly reads into the array element using ReadRaw. For non-trivial types, it uses ReadObject._ 
```C++
template<typename T>
inline void AGE::DataReader::ReadArray (
    std::vector< T > & Array,
    uint32_t Size=0
) 
```





**Parameters:**


* `Array` Reference to the vector that will hold the read elements. 
* `Size` The size of the array. If zero, the function first reads the size.



**Returns:**

void


Reads an array of elements from the input stream. If the size is not provided, it reads the size first. The function uses `ReadRaw` for trivial types and `ReadObject` for non-trivial types.




**Parameters:**


* `Array` Reference to the vector where the data will be stored. 
* `Size` Optional parameter specifying the number of elements in the array. If not provided, it is read first. 




        

<hr>



### function ReadBuffer 

_Reads data from the buffer. If size is zero, it reads a uint32\_t to determine the size of the data to read next._ 
```C++
void AGE::DataReader::ReadBuffer (
    char * Data,
    size_t Size
) 
```





**Parameters:**


* `Data` Pointer to the buffer where the data will be stored. 
* `Size` The size of the data to read. If this is zero, it means that the size of the data is expected to follow in a uint32\_t format.

Reads data from the buffer. If size is zero, it reads a uint32\_t to determine the size of the data to read next.




**Parameters:**


* `Data` Pointer to the buffer where the data will be stored. 
* `Size` The size of the data in bytes. If this is zero, the function assumes that the actual size needs to be read first. 




        

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

_Reads a map from the input stream._ 
```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::map< Key, Value > & Map,
    uint32_t Size=0
) 
```



This function reads a map of keys and values from the input stream. If the size is not provided, it will read it first. The key type can be any trivial or non-trivial type that has been defined for serialization. The value type must also be either trivial or non-trivial. It uses ReadRaw to read raw data if the key or value types are trivial and ReadObject otherwise.




**Parameters:**


* `Map` Reference to the map to be populated with keys and values. 
* `Size` Optional parameter specifying the size of the map. If not provided, it will be read first.

Reads a map from the input stream. The size of the map is read if not provided as an argument. If the key or value types are trivial, raw data is read directly; otherwise, objects are read. 

**Parameters:**


* `Map` Reference to the map that will be populated with the values read from the input stream. 
* `Size` Optional parameter specifying the size of the map. If not provided, it is read from the input stream. 




        

<hr>



### function ReadMap [2/3]

_Reads a map from the input stream._ 
```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::unordered_map< Key, Value > & Map,
    uint32_t Size=0
) 
```



This function reads a map of keys and values from the input stream. If the size is not provided, it will read the size first. For each key-value pair, if the key or value type is trivial (like int, float etc.), it uses `ReadRaw` to read them directly; otherwise, it uses `ReadObject` to read them.




**Parameters:**


* `Map` The map to be filled with keys and values from the input stream. 
* `Size` Optional parameter specifying the size of the map. If not provided, it will be read first.

Reads a map from the input stream.


This function reads a map of keys and values from the input stream. If no size is provided, it will read one first. The key-value pairs are read in order based on the size. For each pair, if the key type is trivial (like int or float), it directly reads the key; otherwise, it calls ReadObject to read the key. Similarly for the value, if its type is trivial, it directly reads the value; otherwise, it calls ReadObject to read the value.




**Parameters:**


* `Map` The map to be populated with the data from the input stream. 
* `Size` The number of elements in the map (default: 0). If not provided, a size is expected to follow. 




        

<hr>



### function ReadMap [3/3]

_Reads a map from the input stream. The size of the map is read if not provided as an argument. If the key and value types are trivial, raw data is read directly; otherwise, objects are read._ 
```C++
template<typename Key, typename Value>
inline void AGE::DataReader::ReadMap (
    std::unordered_map< std::string, Value > & Map,
    uint32_t Size=0
) 
```





**Parameters:**


* `Map` The unordered\_map to be populated with the data read from the input stream. 
* `Size` The size of the map. Defaults to 0 if not provided. 



**Returns:**

void


Reads a map from the input stream.


This function reads a map of keys to values from the input stream. The size of the map is read first if not provided, then each key-value pair is read in a loop. If the Key or Value type is trivial (e.g., int, float), it uses ReadRaw to read directly into them; otherwise, it uses ReadObject.




**Parameters:**


* `Map` The unordered map to be populated with keys and values. 
* `Size` Optional parameter specifying the size of the map. If not provided, it is read from the input stream first. 




        

<hr>



### function ReadObject 

_This function reads an object of type T from the stream using Deserialize method._ 
```C++
template<typename T>
inline void AGE::DataReader::ReadObject (
    T & Obj
) 
```





**Parameters:**


* `Obj` The object to be read into. 



**Returns:**

void


This function reads an object from the stream using Deserialize method of T.




**Parameters:**


* `Obj` The object to be read into. 




        

<hr>



### function ReadRaw 

_This function reads raw data into a specified type._ 
```C++
template<typename T>
inline void AGE::DataReader::ReadRaw (
    T & Type
) 
```



The function takes a reference to the variable of type T and attempts to read data from an underlying source into it. If successful, it asserts that the operation was successful; if not, it throws an exception with the message "Failed to Read Data".




**Parameters:**


* `Type` A reference to the variable where the raw data will be stored. 



**Returns:**

void


This function reads raw data into a specified type.


The function takes a reference to an object of type T and attempts to read the size of T bytes from the input source. If successful, it will store the read data in the provided variable. Otherwise, it will throw an assertion with the message "Failed to Read Data".




**Parameters:**


* `Type` A reference to an object of type T where the read data will be stored. 



**Returns:**

void 





        

<hr>



### function ReadString 

_Reads a string from the data source._ 
```C++
void AGE::DataReader::ReadString (
    std::string & String
) 
```



This function reads a string from the data source, resizing the input string to match the size of the read data and assigning it the value of the read data.




**Parameters:**


* `String` The string to be read into.

Reads a string from the data source.


This function reads a string from the data source, which is expected to be in the format of a size\_t followed by the actual string data. The size\_t indicates the length of the following string data.




**Parameters:**


* `String` A reference to the string that will hold the read data. 




        

<hr>



### function SetStreamPosition 

```C++
virtual void AGE::DataReader::SetStreamPosition (
    uint64_t Pos
) = 0
```




<hr>



### function operator bool 

_Checks the state of the stream._ 
```C++
inline AGE::DataReader::operator bool () const
```



This function returns a boolean value indicating whether or not the stream is in a good state. It does this by calling the private method `IsStreamGood()`, which should be implemented elsewhere in the codebase.




**Returns:**

True if the stream is in a good state, false otherwise.


Checks the status of the stream.


This function checks whether the stream is in a good state or not by calling the `IsStreamGood` method. It returns true if the stream is good, and false otherwise.




**Returns:**

True if the stream is good, false otherwise. 





        

<hr>



### function ~DataReader 

_Virtual destructor for the_ [_**DataReader**_](class_a_g_e_1_1_data_reader.md) _class._
```C++
virtual AGE::DataReader::~DataReader () = default
```



This function is responsible for releasing any resources that were acquired by the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance, such as memory or file handles. It does not return anything and has no parameters.


Virtual destructor for the [**DataReader**](class_a_g_e_1_1_data_reader.md) class.


This function is responsible for releasing any resources that were acquired by the [**DataReader**](class_a_g_e_1_1_data_reader.md) instance, such as memory or file handles. It does not return anything (void) and hence it doesn't need a Doxygen comment to document its return value. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Serializers/Public/DataReader.h`

