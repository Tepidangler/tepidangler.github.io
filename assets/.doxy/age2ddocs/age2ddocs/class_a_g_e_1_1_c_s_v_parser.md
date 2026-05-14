

# Class AGE::CSVParser



[**ClassList**](annotated.md) **>** [**AGE**](namespace_a_g_e.md) **>** [**CSVParser**](class_a_g_e_1_1_c_s_v_parser.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  std::pair&lt; int, int &gt; | [**ParseFile**](#function-parsefile-22) (const std::string & FileName, std::vector&lt; float &gt; & OutVec) <br>_Parses a CSV file and stores the values in an output vector._  |


## Public Static Functions

| Type | Name |
| ---: | :--- |
|  std::pair&lt; int, int &gt; | [**ParseFile**](#function-parsefile-12) (const std::string & FileName, std::vector&lt; T &gt; & OutVec) <br>_Parses a CSV file and stores the values in an output vector._  |


























## Public Functions Documentation




### function ParseFile [2/2]

_Parses a CSV file and stores the values in an output vector._ 
```C++
template<>
std::pair< int, int > AGE::CSVParser::ParseFile (
    const std::string & FileName,
    std::vector< float > & OutVec
) 
```



This function reads a CSV file specified by its filename, extracts all column names and row names from it using rapidcsv library, then iterates over each column to get its values as floats. These float values are pushed back into the provided output vector. The number of columns and rows in the CSV file is returned as a pair.




**Parameters:**


* `FileName` A constant string reference representing the filename of the CSV file to be parsed. 
* `OutVec` A reference to an output vector where the extracted float values will be stored.



**Returns:**

A pair of integers, where the first integer represents the number of columns in the CSV file and the second integer represents the number of rows.


Parses a CSV file and stores the values in an output vector.


This function reads a CSV file specified by its filename, extracts all column names and row names from it using rapidcsv library. It then iterates over each column, retrieving the values as floats and pushing them into the provided output vector. The number of columns and rows in the CSV file are returned as a pair.




**Parameters:**


* `FileName` A constant string reference representing the filename of the CSV file to be parsed. 
* `OutVec` A vector of floats that will store all values from the CSV file. 



**Returns:**

A pair of integers, where the first value is the number of columns in the CSV file and the second value is the number of rows. 





        

<hr>
## Public Static Functions Documentation




### function ParseFile [1/2]

_Parses a CSV file and stores the values in an output vector._ 
```C++
template<typename T>
static std::pair< int, int > AGE::CSVParser::ParseFile (
    const std::string & FileName,
    std::vector< T > & OutVec
) 
```



This function reads a CSV file specified by its filename, extracts all column names and row names from it using rapidcsv library. It then iterates over each column, retrieving the values of that column into a temporary vector. These values are then pushed back to the output vector. The function finally returns a pair of integers where the first element is the average number of elements per column and the second one is the average number of elements per row in the CSV file.




**Parameters:**


* `FileName` A constant string reference representing the name of the CSV file to be parsed. 
* `OutVec` An output vector where all values from the CSV file will be stored. 



**Returns:**

A pair of integers, where the first element is the average number of elements per column and the second one is the average number of elements per row in the CSV file.


Parses a CSV file and stores the values in an output vector.


This function reads a CSV file specified by its filename, extracts all column names and row names from it using rapidcsv library. It then iterates over each column, retrieving the corresponding values of type T (template parameter), and pushes them into the output vector. The function finally returns a pair of integers representing the average number of elements per column and row in the CSV file.




**Parameters:**


* `FileName` A constant string reference to the filename of the CSV file to be parsed. 
* `OutVec` An output vector where the values from the CSV file will be stored.



**Returns:**

A pair of integers representing the average number of elements per column and row in the CSV file. 





        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Parser/Public/CsvParser.h`

