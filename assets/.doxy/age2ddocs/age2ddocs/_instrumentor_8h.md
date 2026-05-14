

# File Instrumentor.h



[**FileList**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Debug**](dir_f319587f04f95a4a2d227b307381fcad.md) **>** [**Public**](dir_9538c177d856a6b0b9437f7654347dcb.md) **>** [**Instrumentor.h**](_instrumentor_8h.md)

[Go to the source code of this file](_instrumentor_8h_source.md)



* `#include "Core/Public/Log.h"`
* `#include <algorithm>`
* `#include <chrono>`
* `#include <fstream>`
* `#include <iomanip>`
* `#include <string>`
* `#include <thread>`
* `#include <mutex>`
* `#include <sstream>`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**AGE**](namespace_a_g_e.md) <br> |
| namespace | [**InstrumentorUtils**](namespace_a_g_e_1_1_instrumentor_utils.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| struct | [**InstrumentationSession**](struct_a_g_e_1_1_instrumentation_session.md) <br> |
| class | [**InstrumentationTimer**](class_a_g_e_1_1_instrumentation_timer.md) <br> |
| class | [**Instrumentor**](class_a_g_e_1_1_instrumentor.md) <br> |
| struct | [**ChangeResult**](struct_a_g_e_1_1_instrumentor_utils_1_1_change_result.md) &lt;N&gt;<br> |
| struct | [**ProfileResult**](struct_a_g_e_1_1_profile_result.md) <br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**AGE\_FUNC\_SIG**](_instrumentor_8h.md#define-age_func_sig)  `"AGE\_FUNC\_SIG unknown!"`<br> |
| define  | [**AGE\_PROFILE**](_instrumentor_8h.md#define-age_profile)  `1`<br> |
| define  | [**AGE\_PROFILE\_BEGIN\_SESSION**](_instrumentor_8h.md#define-age_profile_begin_session) (name, filepath) `[**::AGE::Instrumentor::Get**](class_a_g_e_1_1_instrumentor.md#function-get)().BeginSession(name, filepath)`<br> |
| define  | [**AGE\_PROFILE\_END\_SESSION**](_instrumentor_8h.md#define-age_profile_end_session) () `[**::AGE::Instrumentor::Get**](class_a_g_e_1_1_instrumentor.md#function-get)().EndSession()`<br> |
| define  | [**AGE\_PROFILE\_FUNCTION**](_instrumentor_8h.md#define-age_profile_function) () `AGE\_PROFILE\_SCOPE(AGE\_FUNC\_SIG)`<br> |
| define  | [**AGE\_PROFILE\_SCOPE**](_instrumentor_8h.md#define-age_profile_scope) (name) `AGE\_PROFILE\_SCOPE\_LINE(name, \_\_LINE\_\_)`<br> |
| define  | [**AGE\_PROFILE\_SCOPE\_LINE**](_instrumentor_8h.md#define-age_profile_scope_line) (name, line) `AGE\_PROFILE\_SCOPE\_LINE2(name, line)`<br> |
| define  | [**AGE\_PROFILE\_SCOPE\_LINE2**](_instrumentor_8h.md#define-age_profile_scope_line2) (name, line) `/* multi line expression */`<br> |

## Macro Definition Documentation





### define AGE\_FUNC\_SIG 

```C++
#define AGE_FUNC_SIG `"AGE_FUNC_SIG unknown!"`
```




<hr>



### define AGE\_PROFILE 

```C++
#define AGE_PROFILE `1`
```




<hr>



### define AGE\_PROFILE\_BEGIN\_SESSION 

```C++
#define AGE_PROFILE_BEGIN_SESSION (
    name,
    filepath
) `::AGE::Instrumentor::Get ().BeginSession(name, filepath)`
```




<hr>



### define AGE\_PROFILE\_END\_SESSION 

```C++
#define AGE_PROFILE_END_SESSION (
    
) `::AGE::Instrumentor::Get ().EndSession()`
```




<hr>



### define AGE\_PROFILE\_FUNCTION 

```C++
#define AGE_PROFILE_FUNCTION (
    
) `AGE_PROFILE_SCOPE(AGE_FUNC_SIG)`
```




<hr>



### define AGE\_PROFILE\_SCOPE 

```C++
#define AGE_PROFILE_SCOPE (
    name
) `AGE_PROFILE_SCOPE_LINE(name, __LINE__)`
```




<hr>



### define AGE\_PROFILE\_SCOPE\_LINE 

```C++
#define AGE_PROFILE_SCOPE_LINE (
    name,
    line
) `AGE_PROFILE_SCOPE_LINE2(name, line)`
```




<hr>



### define AGE\_PROFILE\_SCOPE\_LINE2 

```C++
#define AGE_PROFILE_SCOPE_LINE2 (
    name,
    line
) `/* multi line expression */`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Debug/Public/Instrumentor.h`

