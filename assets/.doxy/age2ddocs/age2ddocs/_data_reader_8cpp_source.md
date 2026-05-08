

# File DataReader.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Serializers**](dir_0e7d7552020383c89e3ca069b8b7352b.md) **>** [**Private**](dir_ec26f5e2e3b4d07fbb894a640522da88.md) **>** [**DataReader.cpp**](_data_reader_8cpp.md)

[Go to the documentation of this file](_data_reader_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Serializers/Public/DataReader.h"
#include "Core/Public/Buffer.h"
#include "Parser/Public/JsonParser.h"

namespace AGE
{

    FileStreamReader::FileStreamReader(const std::filesystem::path& Path)
        :m_Path(Path)
    {
        m_Stream = std::ifstream(Path, std::ifstream::in | std::ifstream::binary);

    }
    FileStreamReader::~FileStreamReader()
    {
        m_Stream.close();
    }
    bool FileStreamReader::ReadData(char* Data, size_t Size)
    {
#if __clang__
        m_Stream.read(Data, (long)Size);
#else
        m_Stream.read(Data, Size);
#endif
        return true;
    }

    bool FileStreamReader::ReadBytes(std::vector<std::byte>& Data, size_t Size)
    {
#if __clang__
        m_Stream.read(reinterpret_cast<char*>(Data.data()), (long)Size);
#else
        m_Stream.read(reinterpret_cast<char*>(Data.data()), Size);
#endif
        return true;
    }

    bool FileStreamReader::ReadBytes(uint8_t* Data, size_t Size)
    {
#if __clang__
        m_Stream.read(reinterpret_cast<char*>(Data), (long)Size);
#else
        m_Stream.read(reinterpret_cast<char*>(Data), Size);
#endif
        return true;
    }

    MemoryStreamReader::MemoryStreamReader(void* Addr, size_t Size)
        :m_Addr(Addr)
    {
        std::string s((char*)m_Addr, Size);
        m_Stream = std::istringstream(s);
    }
    MemoryStreamReader::~MemoryStreamReader()
    {
        m_Stream.clear();
    }
    bool MemoryStreamReader::ReadData(char* Data, size_t Size)
    {
#if __clang__
        m_Stream.read(Data, (long)Size);
#else
        m_Stream.read(Data, Size);
#endif
        return true;
    }

    bool MemoryStreamReader::ReadBytes(std::vector<std::byte>& Data, size_t Size)
    {
#if __clang__
        m_Stream.read(reinterpret_cast<char*>(Data.data()), (long)Size);
#else
        m_Stream.read(reinterpret_cast<char*>(Data.data()), Size);
#endif
        return true;
    }

    bool MemoryStreamReader::ReadBytes(uint8_t* Data, size_t Size)
    {
#if __clang__
        m_Stream.read(reinterpret_cast<char*>(Data), (long)Size);
#else
        m_Stream.read(reinterpret_cast<char*>(Data), Size);
#endif
        return true;
    }

    bool MemoryStreamReader::ReadJson(std::string& String)
    {
        return false;
    }

    void DataReader::ReadBuffer(char* Data, size_t Size)
    {
        uint32_t size = 0;
        if (Size == 0)
        {
            ReadRaw<uint32_t>(size);
            ReadData(Data, (size_t)size);
            return;
        }
            ReadData(Data, Size);
    }
    void DataReader::ReadString(std::string& String)
    {
        size_t Sizet = 0;
        std::string In;
        ReadData((char*)&Sizet, sizeof(size_t));
        In.resize(Sizet);
        ReadData(&In[0], Sizet);
        //ReadData(&String[0], Size);

        String = In.data();

    }
    bool FileStreamReader::ReadJson(std::string& String)
    {
        size_t Sizet = 0;
        std::string In;
        ReadData((char*)&Sizet, sizeof(size_t));
        In.resize(Sizet);
        std::fill(&In[0], &In[Sizet-1], 0);

#if __clang__
        m_Stream.read(&In[0], (long)Sizet);
#else
        m_Stream.read(&In[0], Sizet);
#endif
        String = In.data();

        return true;
    }
}
```


