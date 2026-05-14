

# File CsvParser.cpp

[**File List**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Parser**](dir_81d36680c9a9035d38dcc36084da83fe.md) **>** [**Private**](dir_2593ff35d59f997c5ff64f0f197c6542.md) **>** [**CsvParser.cpp**](_csv_parser_8cpp.md)

[Go to the documentation of this file](_csv_parser_8cpp.md)


```C++
#include "AGEpch.hpp"
#include "Parser/Public/CsvParser.h"

namespace AGE
{
    template<typename T>
std::pair<int, int> CSVParser::ParseFile(const std::string& FileName, std::vector<T>& OutVec)
    {
        std::vector<T> Values;
        rapidcsv::Document Doc(FileName, rapidcsv::LabelParams(0, 0));
        std::vector<std::string> ColumnNames = Doc.GetColumnNames();
        std::vector <std::string> RowNames = Doc.GetRowNames();

        
        for (auto CN : ColumnNames)
        {
            Values.clear();
            Values = Doc.GetColumn<T>(CN);
            for (auto V : Values)
            {
                OutVec.push_back(V);
            }
        }

        return std::pair<int,int>((OutVec.size() / ColumnNames.size()), (OutVec.size()/RowNames.size()));

    }

    template<>
std::pair<int, int> CSVParser::ParseFile(const std::string& FileName, std::vector<float>& OutVec)
    {
        std::vector<float> Values;
        rapidcsv::Document Doc(FileName, rapidcsv::LabelParams(0, 0));
        std::vector<std::string> ColumnNames = Doc.GetColumnNames();
        std::vector <std::string> RowNames = Doc.GetRowNames();


        for (auto CN : ColumnNames)
        {
            Values.clear();
            Values = Doc.GetColumn<float>(CN);
            for (auto V : Values)
            {
                OutVec.push_back(V);
            }
        }

        return std::pair<int, int>((int)ColumnNames.size(), (int)RowNames.size());

    }
}
```


