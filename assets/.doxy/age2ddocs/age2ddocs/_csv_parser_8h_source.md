

# File CsvParser.h

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Parser**](dir_81d36680c9a9035d38dcc36084da83fe.md) **>** [**Public**](dir_b9d50061ecaa34aafe5e7c2ebce34886.md) **>** [**CsvParser.h**](_csv_parser_8h.md)

[Go to the documentation of this file](_csv_parser_8h.md)


```C++
#pragma once
#ifdef AG_PLATFORM_WINDOWS
#include "rapidcsv.h"
#else
#include "src/rapidcsv.h"
#endif
namespace AGE
{
    class CSVParser
    {
    public:
        template<typename T>
        //Parses a CSV file storing all of the values in a vector by column, returning the number of columns and rows in the csv File
        //It's on the user to know what order this data will be retrieved in and do whatever they like with the data
        static std::pair<int,int> ParseFile(const std::string& FileName, std::vector<T>& OutVec);

    private:

    };
}
```


