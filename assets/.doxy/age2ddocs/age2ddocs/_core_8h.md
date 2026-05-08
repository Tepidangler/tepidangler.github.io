

# File Core.h



[**FileList**](files.md) **>** [**AGE**](dir_c1649042ac9dcb65c6181568c305ecb0.md) **>** [**Core**](dir_40f28070a54f843eaf86230230ee6eb2.md) **>** [**Public**](dir_4d1ade32537ccbee8ff5d36b16abbd57.md) **>** [**Core.h**](_core_8h.md)

[Go to the source code of this file](_core_8h_source.md)



* `#include <memory>`
* `#include <string>`
* `#include <filesystem>`
* `#include <any>`
* `#include "Core/Public/Log.h"`













## Namespaces

| Type | Name |
| ---: | :--- |
| namespace | [**AGE**](namespace_a_g_e.md) <br> |
| namespace | [**GameFramework**](namespace_game_framework.md) <br> |


## Classes

| Type | Name |
| ---: | :--- |
| class | [**Reverse**](class_a_g_e_1_1_reverse.md) &lt;typename T&gt;<br> |

















































## Macros

| Type | Name |
| ---: | :--- |
| define  | [**BIND\_ACTION\_FN**](_core_8h.md#define-bind_action_fn) (x) `std::bind(&x, this)`<br> |
| define  | [**BIND\_AXIS\_FN**](_core_8h.md#define-bind_axis_fn) (x) `std::bind(&x, this, std::placeholders::\_1)`<br> |
| define  | [**BIND\_EVENT\_FN**](_core_8h.md#define-bind_event_fn) (x) `std::bind(&x, this, std::placeholders::\_1)`<br> |
| define  | [**BIT**](_core_8h.md#define-bit) (x) `(1 &lt;&lt; x)`<br> |

## Macro Definition Documentation





### define BIND\_ACTION\_FN 

```C++
#define BIND_ACTION_FN (
    x
) `std::bind(&x, this)`
```




<hr>



### define BIND\_AXIS\_FN 

```C++
#define BIND_AXIS_FN (
    x
) `std::bind(&x, this, std::placeholders::_1)`
```




<hr>



### define BIND\_EVENT\_FN 

```C++
#define BIND_EVENT_FN (
    x
) `std::bind(&x, this, std::placeholders::_1)`
```




<hr>



### define BIT 

```C++
#define BIT (
    x
) `(1 << x)`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/Core.h`

