

# Struct AGE::Buffer



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**Buffer**](struct_a_g_e_1_1_buffer.md)


























## Public Attributes

| Type | Name |
| ---: | :--- |
|  void \* | [**Data**](#variable-data)  <br> |
|  uint64\_t | [**Size**](#variable-size)  <br> |
















## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**Allocate**](#function-allocate) (uint64\_t size) <br>_Allocates memory for an array of characters._  |
|   | [**Buffer**](#function-buffer-12) () <br>[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _constructor initializes the data pointer to nullptr and size to 0._ |
|   | [**Buffer**](#function-buffer-22) (const void \* data, uint64\_t size=0) <br>[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _constructor that initializes the buffer with given data and size._ |
|  T & | [**Read**](#function-read) (uint64\_t offset=0) <br>_This function reads a value of type T from the data buffer at a specified offset._  |
|  char \* | [**ReadBytes**](#function-readbytes) (uint64\_t size, uint64\_t offset) const<br>_ReadBytes reads a specified number of bytes from the buffer starting at a given offset._  |
|  void | [**Release**](#function-release) () <br>_Releases the memory allocated for the data._  |
|  void | [**Write**](#function-write) (const void \* data, uint64\_t size, uint64\_t offset=0) <br>_Writes a block of data to the buffer at a specified offset._  |
|  void | [**ZeroInitialize**](#function-zeroinitialize) () <br>_This function initializes a block of memory with zeros._  |
|   | [**operator bool**](#function-operator-bool) () const<br>_This function returns a boolean value based on the truthiness of Data member._  |
|  char & | [**operator[]**](#function-operator) (int Index) <br>_This function returns a reference to the character at the specified index in the Data array._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  [**Buffer**](struct_a_g_e_1_1_buffer.md) | [**Copy**](#function-copy-12) (const [**Buffer**](struct_a_g_e_1_1_buffer.md) & Other) <br>_Copies a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object by allocating the same size and copying data from another_[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object._ |
|  [**Buffer**](struct_a_g_e_1_1_buffer.md) | [**Copy**](#function-copy-22) (const void \* data, uint64\_t size) <br>_Copies a block of memory into a new_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object._ |
|  void | [**Deserialize**](#function-deserialize) ([**DataReader**](class_a_g_e_1_1_data_reader.md) \* Deserializer, [**Buffer**](struct_a_g_e_1_1_buffer.md) & Instance) <br>_Deserialize a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _instance from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._ |
|  void | [**Serialize**](#function-serialize) ([**DataWriter**](class_a_g_e_1_1_data_writer.md) \* Serializer, const [**Buffer**](struct_a_g_e_1_1_buffer.md) & Instance) <br>_This function serializes a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._ |


























## Public Attributes Documentation




### variable Data 

```C++
void* AGE::Buffer::Data;
```




<hr>



### variable Size 

```C++
uint64_t AGE::Buffer::Size;
```




<hr>
## Public Functions Documentation




### function Allocate 

_Allocates memory for an array of characters._ 
```C++
inline void AGE::Buffer::Allocate (
    uint64_t size
) 
```



This function allocates a block of memory to store an array of characters. If the input size is zero, it simply returns without doing anything. The allocated memory should be deallocated using Free() when it's no longer needed.




**Parameters:**


* `size` The number of elements in the array to be allocated.

Allocates memory for an array of pointers to characters.


This function allocates a block of memory for an array of `char` pointers. It first deletes the existing data if any, then it checks if the size is zero. If not, it allocates new memory and sets the `Size` variable accordingly.




**Parameters:**


* `size` The number of elements to be allocated. 




        

<hr>



### function Buffer [1/2]

[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _constructor initializes the data pointer to nullptr and size to 0._
```C++
inline AGE::Buffer::Buffer () 
```



Default constructor for the [**Buffer**](struct_a_g_e_1_1_buffer.md) class. Initializes an empty buffer with a data pointer set to nullptr and size set to 0. 


        

<hr>



### function Buffer [2/2]

[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _constructor that initializes the buffer with given data and size._
```C++
inline AGE::Buffer::Buffer (
    const void * data,
    uint64_t size=0
) 
```





**Parameters:**


* `data` Pointer to the data to be stored in the buffer. Can be null. 
* `size` Size of the data pointed by 'data'. Defaults to 0 if not provided.

[**Buffer**](struct_a_g_e_1_1_buffer.md) constructor that initializes the buffer with a given pointer to data and its size. 

**Parameters:**


* `data` Pointer to the data to be stored in the buffer. Can be null. 
* `size` Size of the data pointed by 'data'. Defaults to 0 if not provided. 




        

<hr>



### function Read 

_This function reads a value of type T from the data buffer at a specified offset._ 
```C++
template<typename T>
inline T & AGE::Buffer::Read (
    uint64_t offset=0
) 
```





**Parameters:**


* `offset` The position in the data buffer to read from, defaults to 0 if not provided. 



**Returns:**

A reference to the value of type T located at the given offset.


This function reads a value of type T from the data buffer at a specified offset. 

**Parameters:**


* `offset` The position in the data buffer to read from, defaults to 0 if not provided. 



**Returns:**

A reference to the value of type T located at the given offset. 





        

<hr>



### function ReadBytes 

_ReadBytes reads a specified number of bytes from the buffer starting at a given offset._ 
```C++
inline char * AGE::Buffer::ReadBytes (
    uint64_t size,
    uint64_t offset
) const
```



The function checks if the requested read operation will result in a buffer overflow by comparing the sum of the size and offset with the total size of the buffer. If it's larger, an assertion is triggered to indicate a potential issue. It then allocates memory for a new char array of the specified size using 'new', copies the data from the buffer starting at the given offset into this newly allocated memory, and returns a pointer to this memory.




**Parameters:**


* `size` The number of bytes to read. 
* `offset` The position in the buffer where reading should start. 



**Returns:**

A pointer to an array containing the read data. This must be deleted by the caller when it's no longer needed.




**Exception:**


* `std::runtime_error` if there is a buffer overflow (i.e., the sum of size and offset exceeds the total size of the buffer).

ReadBytes reads a specified number of bytes from the buffer starting at a given offset.


This function is used to read data from the buffer. It takes two parameters - 'size' which specifies the number of bytes to be read and 'offset', which indicates the position in the buffer where reading should start. The function checks if the requested size plus the offset exceeds the total size of the buffer, and throws an error if it does. It then allocates a new character array of the specified size using dynamic memory allocation (new char[size]), copies 'size' bytes from the buffer starting at the given offset to this newly allocated array, and returns this array. The caller is responsible for deallocating the returned pointer with delete[].




**Parameters:**


* `size` Number of bytes to read. 
* `offset` Position in the buffer where reading should start. 



**Returns:**

Pointer to a new character array containing the read data. Caller must free this memory using 'delete[]'.




**Exception:**


* `std::runtime_error` if the requested size plus the offset exceeds the total size of the buffer. 




        

<hr>



### function Release 

_Releases the memory allocated for the data._ 
```C++
inline void AGE::Buffer::Release () 
```



This function deletes the dynamically allocated array of characters (char\*) Data and sets it to null, effectively releasing the memory. It also resets Size to 0 indicating that no more data is present in the object.




**Returns:**

void


Releases the memory allocated for the data.


This function deletes the dynamically allocated array of characters and sets the Data pointer to null, effectively releasing the memory. It also resets the Size variable to 0 indicating that no more data is present in the object.




**Returns:**

void 





        

<hr>



### function Write 

_Writes a block of data to the buffer at a specified offset._ 
```C++
inline void AGE::Buffer::Write (
    const void * data,
    uint64_t size,
    uint64_t offset=0
) 
```



This function copies 'size' bytes from the memory area pointed by 'data' into the buffer starting at 'offset'. The destination buffer is assumed to be large enough to hold the copied data, i.e., it should have been allocated with Size bytes of space beforehand. If the sum of 'size' and 'offset' exceeds the total size of the buffer (Size), a buffer overflow error will occur.




**Parameters:**


* `data` Pointer to the source of the data to be copied. 
* `size` Number of bytes to copy from the source. 
* `offset` The number of bytes in the destination buffer at which copying begins. Defaults to 0 if not specified.

Writes a block of data to the buffer at a specified offset.


This function copies 'size' bytes from the memory area pointed by 'data' into the buffer starting at position 'offset'. If the sum of 'offset' and 'size' exceeds the total size of the buffer, it results in a "Buffer Overflow!" error.




**Parameters:**


* `data` Pointer to the source of the data to be copied. 
* `size` Number of bytes to copy from the source. 
* `offset` Position within the buffer at which copying begins. Defaults to 0 if not provided. 




        

<hr>



### function ZeroInitialize 

_This function initializes a block of memory with zeros._ 
```C++
inline void AGE::Buffer::ZeroInitialize () 
```



The function takes no parameters and does not return anything. It uses the memset function from the C standard library to fill the Data array with zeros, which is of size Size.


This function initializes a block of memory with zeros.


The function takes no parameters and returns void. It uses the memset function from the cstring library to fill the Data array with zeros, which is assumed to be of size Size. If Data is null, nothing happens.




**Returns:**

Void 





        

<hr>



### function operator bool 

_This function returns a boolean value based on the truthiness of Data member._ 
```C++
inline AGE::Buffer::operator bool () const
```





**Parameters:**


* `None` 



**Returns:**

Returns true if Data is not null, false otherwise.


Converts the object to a boolean value.


This function returns true if Data is not null, and false otherwise. It provides an implicit conversion from the class instance to bool.




**Returns:**

True if Data is not null, False otherwise. 





        

<hr>



### function operator[] 

_This function returns a reference to the character at the specified index in the Data array._ 
```C++
inline char & AGE::Buffer::operator[] (
    int Index
) 
```





**Parameters:**


* `Index` The zero-based index of the character to return. 



**Returns:**

A reference to the character at the given index.


This function returns a reference to the character at the specified index in the Data array.




**Parameters:**


* `Index` The zero-based index of the character to return. 



**Returns:**

A reference to the character at the given index. 





        

<hr>
## Public Static Functions Documentation




### function Copy [1/2]

_Copies a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object by allocating the same size and copying data from another_[_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object._
```C++
static inline Buffer AGE::Buffer::Copy (
    const Buffer & Other
) 
```





**Parameters:**


* `Other` The [**Buffer**](struct_a_g_e_1_1_buffer.md) object to be copied. 



**Returns:**

A new [**Buffer**](struct_a_g_e_1_1_buffer.md) object with the same size as the input and copied data.


Copies a [**Buffer**](struct_a_g_e_1_1_buffer.md) object by allocating the same size and copying data from another [**Buffer**](struct_a_g_e_1_1_buffer.md).


This function creates a new [**Buffer**](struct_a_g_e_1_1_buffer.md) object with the same size as the input [**Buffer**](struct_a_g_e_1_1_buffer.md), then copies the data from the input [**Buffer**](struct_a_g_e_1_1_buffer.md) into this new one. The copied data is returned as the result of the function.




**Parameters:**


* `Other` The [**Buffer**](struct_a_g_e_1_1_buffer.md) to be copied. 



**Returns:**

A copy of the input [**Buffer**](struct_a_g_e_1_1_buffer.md). 





        

<hr>



### function Copy [2/2]

_Copies a block of memory into a new_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _object._
```C++
static inline Buffer AGE::Buffer::Copy (
    const void * data,
    uint64_t size
) 
```



This function creates a new [**Buffer**](struct_a_g_e_1_1_buffer.md) object and allocates the necessary memory to hold 'size' bytes. It then uses memcpy() to copy 'data' into this newly allocated memory. The copied data can be accessed through the Data property of the returned [**Buffer**](struct_a_g_e_1_1_buffer.md) object.




**Parameters:**


* `data` Pointer to the block of memory to copy. 
* `size` Size in bytes of the block of memory to copy.



**Returns:**

A new [**Buffer**](struct_a_g_e_1_1_buffer.md) object containing a copy of 'data'.


Copies a block of memory into a new [**Buffer**](struct_a_g_e_1_1_buffer.md) object.


This function creates a new [**Buffer**](struct_a_g_e_1_1_buffer.md) object and allocates the necessary memory to hold 'size' bytes. It then uses memcpy() to copy the data from the input pointer into this newly allocated memory. The copied buffer is returned as the result.




**Parameters:**


* `data` A pointer to the block of memory to be copied. 
* `size` The number of bytes to copy from 'data'.



**Returns:**

A new [**Buffer**](struct_a_g_e_1_1_buffer.md) object containing a copy of the input data. 





        

<hr>



### function Deserialize 

_Deserialize a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _instance from a_[_**DataReader**_](class_a_g_e_1_1_data_reader.md) _._
```C++
static inline void AGE::Buffer::Deserialize (
    DataReader * Deserializer,
    Buffer & Instance
) 
```



This function reads raw data from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and deserializes it into a [**Buffer**](struct_a_g_e_1_1_buffer.md) instance. The first byte read is stored in an uint8\_t variable, which is then used to allocate memory for the buffer. The size of the buffer is read next as an uint64\_t. After these two values are obtained, the buffer's memory is allocated and the bytes from the [**DataReader**](class_a_g_e_1_1_data_reader.md) are written into it.




**Parameters:**


* `Deserializer` A pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides the raw data for deserialization. 
* `Instance` The [**Buffer**](struct_a_g_e_1_1_buffer.md) instance where the deserialized data will be stored.

Deserialize a [**Buffer**](struct_a_g_e_1_1_buffer.md) instance from a [**DataReader**](class_a_g_e_1_1_data_reader.md).


This function reads raw data from the provided [**DataReader**](class_a_g_e_1_1_data_reader.md) and deserializes it into a [**Buffer**](struct_a_g_e_1_1_buffer.md) instance. The first byte read is stored in an uint8\_t variable, which is then used to allocate memory for the buffer. The size of the buffer is read next as an uint64\_t. After these two values are obtained, the buffer's memory is allocated and the bytes from the [**DataReader**](class_a_g_e_1_1_data_reader.md) are written into it.




**Parameters:**


* `Deserializer` Pointer to a [**DataReader**](class_a_g_e_1_1_data_reader.md) instance that provides raw data for deserialization. 
* `Instance` Reference to a [**Buffer**](struct_a_g_e_1_1_buffer.md) instance where the deserialized data will be stored. 




        

<hr>



### function Serialize 

_This function serializes a_ [_**Buffer**_](struct_a_g_e_1_1_buffer.md) _instance into the provided_[_**DataWriter**_](class_a_g_e_1_1_data_writer.md) _._
```C++
static inline void AGE::Buffer::Serialize (
    DataWriter * Serializer,
    const Buffer & Instance
) 
```



The function writes two pieces of data to the [**DataWriter**](class_a_g_e_1_1_data_writer.md): the first byte of the buffer and its size. It uses WriteRaw method for writing raw bytes, which means it directly writes the memory content pointed by the pointer without any conversion or serialization process.




**Parameters:**


* `Serializer` Pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) instance that will be used for serialization. 
* `Instance` The [**Buffer**](struct_a_g_e_1_1_buffer.md) instance to be serialized.

This function serializes a buffer instance into the provided data writer.


The function writes two pieces of information to the data writer: the first byte of the buffer and its size. It uses raw write operations, meaning it directly accesses the memory pointed by the Instance pointer without any additional processing. 

**Parameters:**


* `Serializer` A pointer to a [**DataWriter**](class_a_g_e_1_1_data_writer.md) object that will be used for serialization. 
* `Instance` The [**Buffer**](struct_a_g_e_1_1_buffer.md) instance to be serialized. 




        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Buffer.h`

