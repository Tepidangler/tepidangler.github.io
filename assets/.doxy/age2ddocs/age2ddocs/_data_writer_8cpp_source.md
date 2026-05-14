

# File DataWriter.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Serializers**](dir_0e7d7552020383c89e3ca069b8b7352b.md) **>** [**Private**](dir_ec26f5e2e3b4d07fbb894a640522da88.md) **>** [**DataWriter.cpp**](_data_writer_8cpp.md)

[Go to the documentation of this file](_data_writer_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Serializers/Public/DataWriter.h"
#include "Core/Public/Buffer.h"

namespace AGE
{
FileStreamWriter::FileStreamWriter(const std::filesystem::path& Path)
        :m_Path(Path)
    {
        m_Stream = std::ofstream(Path, std::ofstream::out | std::ofstream::binary);
    }
FileStreamWriter::~FileStreamWriter()
    {
        m_Stream.close();
    }
bool FileStreamWriter::WriteData(const char* Data, size_t Size)
    {
#if __clang__
        m_Stream.write(Data, (long)Size);
#else
        m_Stream.write(Data, Size);
#endif
        return true;
    }
void DataWriter::WriteBuffer(Buffer buffer, bool WriteSize)
    {
        if (WriteSize)
        {
            WriteData((char*)&buffer.Size, sizeof(uint64_t));
        }

        WriteData((char*)buffer.Data, buffer.Size);
    }
void DataWriter::WriteZero(uint64_t Size)
    {
        char Zero = 0;
        for (uint64_t i = 0; i < Size; i++)
        {
            WriteData(&Zero, 1);
        }
    }
void DataWriter::WriteString(const std::string& String)
    {
        //Lol this isn't how it works
        size_t Size = String.length();
        WriteData((char*)&Size, sizeof(size_t));
        WriteData((char*)String.data(), sizeof(char) * Size); //This should probably be String.length() as we should be multiplying the size of a char (1 byte) by the number of chars in the string
    }
MemoryStreamWriter::MemoryStreamWriter(void* Addr)
        :m_Addr(Addr)
    {
        m_Stream = std::stringstream(std::stringstream::out | std::stringstream::binary);
    }
MemoryStreamWriter::~MemoryStreamWriter()
    {
        m_Stream.clear();
    }
bool MemoryStreamWriter::WriteData(const char* Data, size_t Size)
    {
#if __clang__
        m_Stream.write(Data, (long)Size);
#else
        m_Stream.write(Data, Size);
#endif

        return true;
    }
}
```


