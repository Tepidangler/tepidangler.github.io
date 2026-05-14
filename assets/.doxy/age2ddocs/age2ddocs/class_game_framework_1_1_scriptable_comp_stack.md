

# Class GameFramework::ScriptableCompStack



[**ClassList**](annotated.md) **>** [**GameFramework**](namespace_game_framework.md) **>** [**ScriptableCompStack**](class_game_framework_1_1_scriptable_comp_stack.md)










































## Public Functions

| Type | Name |
| ---: | :--- |
|  void | [**PopComponent**](#function-popcomponent) ([**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* Entt) <br>_Removes a ScriptableEntity from the stack of components._  |
|  void | [**PushComponent**](#function-pushcomponent) ([**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* Entt) <br>_Pushes a ScriptableEntity onto the stack at the specified index._  |
|   | [**ScriptableCompStack**](#function-scriptablecompstack) () <br>_Constructor for the_ [_**ScriptableCompStack**_](class_game_framework_1_1_scriptable_comp_stack.md) _class. Initializes an empty stack of components._ |
|  std::vector&lt; [**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* &gt;::iterator | [**begin**](#function-begin-12) () <br>_Returns an iterator pointing to the beginning of the 'm\_Entitys' vector._  |
|  std::vector&lt; [**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* &gt;::const\_iterator | [**begin**](#function-begin-22) () const<br>_Returns a constant iterator pointing to the beginning of the 'm\_Entitys' vector._  |
|  std::vector&lt; [**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* &gt;::iterator | [**end**](#function-end-12) () <br>_Returns an iterator pointing to the theoretical element that follows the last element of the container. This function returns an iterator pointing to one past the last element in the vector, which is considered as a valid position for insertion but does not point to any real data._  |
|  std::vector&lt; [**AGE::ScriptableEntity**](class_a_g_e_1_1_scriptable_entity.md) \* &gt;::const\_iterator | [**end**](#function-end-22) () const<br>_Returns a constant iterator pointing to the past-the-end element of the container._  |
|   | [**~ScriptableCompStack**](#function-scriptablecompstack) () <br>_Destructor for the_ [_**ScriptableCompStack**_](class_game_framework_1_1_scriptable_comp_stack.md) _class. It iterates over all elements in the vector 'm\_Entitys' and deletes each one using the destructor of the ScriptableEntity class._ |




























## Public Functions Documentation




### function PopComponent 

_Removes a ScriptableEntity from the stack of components._ 
```C++
void GameFramework::ScriptableCompStack::PopComponent (
    AGE::ScriptableEntity * Entt
) 
```



This function searches for the provided ScriptableEntity in the m\_Entitys vector and removes it if found. It also decrements the m\_EntityInsertIndex by one to ensure that new entities are inserted at the correct position.




**Parameters:**


* `Entt` Pointer to the ScriptableEntity to be removed from the stack.



**Returns:**

void


Removes a ScriptableEntity from the stack of components.


This function searches for the provided entity in the m\_Entitys vector and if it is found, removes it along with its associated data. The iterator 'it' is used to find the position of the entity within the vector. If the entity is not found, nothing happens.




**Parameters:**


* `Entt` Pointer to the ScriptableEntity that needs to be removed from the stack. 




        

<hr>



### function PushComponent 

_Pushes a ScriptableEntity onto the stack at the specified index._ 
```C++
void GameFramework::ScriptableCompStack::PushComponent (
    AGE::ScriptableEntity * Entt
) 
```



This function inserts a new ScriptableEntity into the m\_Entitys vector at the position indicated by m\_EntityInsertIndex. The entity is then incremented for the next push operation.




**Parameters:**


* `Entt` Pointer to the ScriptableEntity that will be pushed onto the stack. 



**Returns:**

void No return value.


Pushes a ScriptableEntity onto the stack at the specified index.


This function inserts the given ScriptableEntity into the m\_Entitys vector at the position indicated by m\_EntityInsertIndex. The entity is then incremented for future use.




**Parameters:**


* `Entt` Pointer to the ScriptableEntity that will be pushed onto the stack.



**Returns:**

void No return value. 





        

<hr>



### function ScriptableCompStack 

_Constructor for the_ [_**ScriptableCompStack**_](class_game_framework_1_1_scriptable_comp_stack.md) _class. Initializes an empty stack of components._
```C++
GameFramework::ScriptableCompStack::ScriptableCompStack () 
```



Constructor for the [**ScriptableCompStack**](class_game_framework_1_1_scriptable_comp_stack.md) class. Initializes an empty stack of components. 


        

<hr>



### function begin [1/2]

_Returns an iterator pointing to the beginning of the 'm\_Entitys' vector._ 
```C++
inline std::vector< AGE::ScriptableEntity * >::iterator GameFramework::ScriptableCompStack::begin () 
```





**Returns:**

An iterator to the start of the 'm\_Entitys' vector.


Returns an iterator pointing to the beginning of the 'm\_Entitys' vector. 

**Returns:**

An iterator to the start of the 'm\_Entitys' vector. 





        

<hr>



### function begin [2/2]

_Returns a constant iterator pointing to the beginning of the 'm\_Entitys' vector._ 
```C++
inline std::vector< AGE::ScriptableEntity * >::const_iterator GameFramework::ScriptableCompStack::begin () const
```





**Returns:**

A constant iterator to the beginning of the 'm\_Entitys' vector. If the vector is empty, past-the-end (cend) iterator is returned.


Returns a constant iterator pointing to the beginning of the 'm\_Entitys' vector. 

**Returns:**

A constant iterator to the beginning of the 'm\_Entitys' vector. 





        

<hr>



### function end [1/2]

_Returns an iterator pointing to the theoretical element that follows the last element of the container. This function returns an iterator pointing to one past the last element in the vector, which is considered as a valid position for insertion but does not point to any real data._ 
```C++
inline std::vector< AGE::ScriptableEntity * >::iterator GameFramework::ScriptableCompStack::end () 
```





**Returns:**

An iterator to the theoretical element that follows the end of the sequence.


Returns an iterator pointing to the theoretical element that follows the last element of the vector. 

**Returns:**

An iterator to the theoretical element following the last element of the vector. 





        

<hr>



### function end [2/2]

_Returns a constant iterator pointing to the past-the-end element of the container._ 
```C++
inline std::vector< AGE::ScriptableEntity * >::const_iterator GameFramework::ScriptableCompStack::end () const
```





**Returns:**

A constant iterator pointing to the past-the-end element in the container.


Returns a constant iterator pointing to the past-the-end element of the container. 

**Returns:**

A constant iterator pointing to the past-the-end element in the container. 





        

<hr>



### function ~ScriptableCompStack 

_Destructor for the_ [_**ScriptableCompStack**_](class_game_framework_1_1_scriptable_comp_stack.md) _class. It iterates over all elements in the vector 'm\_Entitys' and deletes each one using the destructor of the ScriptableEntity class._
```C++
GameFramework::ScriptableCompStack::~ScriptableCompStack () 
```



Destructor for the [**ScriptableCompStack**](class_game_framework_1_1_scriptable_comp_stack.md) class. It iterates over all elements in the 'm\_Entitys' vector and deletes each one using the destructor of the ScriptableEntity class. 


        

<hr>

------------------------------
The documentation for this class was generated from the following file `C:/Programming/AGE2D/Engine/src/AGE/Core/Public/ScriptableComponentStack.h`

