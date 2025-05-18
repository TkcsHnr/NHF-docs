---
title: vector
summary: A simple dynamic array class template, similar to std::vector. 

---

# vector



A simple dynamic array class template, similar to std::vector.  [More...](#detailed-description)


`#include <vector.hpp>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[vector](/Classes/classvector/#function-vector)**()<br>Default constructor. Initializes an empty vector.  |
| | **[vector](/Classes/classvector/#function-vector)**(size_t capacity)<br>Constructs a vector with a given capacity.  |
| | **[vector](/Classes/classvector/#function-vector)**(const [vector](/Classes/classvector/) & other)<br>Copy constructor.  |
| void | **[push_back](/Classes/classvector/#function-push-back)**(const T & element)<br>Adds an element to the end of the vector.  |
| T & | **[operator[]](/Classes/classvector/#function-operator[])**(size_t idx)<br>Provides access to element at given index with bounds checking.  |
| const T & | **[operator[]](/Classes/classvector/#function-operator[])**(size_t idx) const<br>Provides const access to element at given index with bounds checking.  |
| [vector](/Classes/classvector/)< T > & | **[operator=](/Classes/classvector/#function-operator=)**(const [vector](/Classes/classvector/) & other)<br>Assignment operator for deep copying.  |
| size_t | **[capacity](/Classes/classvector/#function-capacity)**() const<br>Getter for capacity.  |
| size_t | **[size](/Classes/classvector/#function-size)**() const<br>Getter for size.  |
| T * | **[begin](/Classes/classvector/#function-begin)**()<br>Iterator to the beginning of the vector.  |
| T * | **[end](/Classes/classvector/#function-end)**()<br>Iterator to the end of the vector.  |
| const T * | **[begin](/Classes/classvector/#function-begin)**() const<br>Const iterator to the beginning of the vector.  |
| const T * | **[end](/Classes/classvector/#function-end)**() const<br>Const iterator to the end of the vector.  |
| void | **[clear](/Classes/classvector/#function-clear)**()<br>Clears the contents of the vector.  |
| void | **[resize](/Classes/classvector/#function-resize)**(size_t newCapacity)<br>Resizes the vector to a new capacity.  |
| | **[~vector](/Classes/classvector/#function-~vector)**()<br>Destructor. Clears and deallocates the vector.  |

## Detailed Description

```cpp
template <typename T >
class vector;
```

A simple dynamic array class template, similar to std::vector. 

**Template Parameters**: 

  * **T** Type of elements stored in the vector. 

## Public Functions Documentation

### function vector

```cpp
inline vector()
```

Default constructor. Initializes an empty vector. 

### function vector

```cpp
inline vector(
    size_t capacity
)
```

Constructs a vector with a given capacity. 

**Parameters**: 

  * **capacity** Initial capacity of the vector. 


### function vector

```cpp
inline vector(
    const vector & other
)
```

Copy constructor. 

**Parameters**: 

  * **other** Vector to copy from. 


### function push_back

```cpp
inline void push_back(
    const T & element
)
```

Adds an element to the end of the vector. 

**Parameters**: 

  * **element** Element to be added. 


### function operator[]

```cpp
inline T & operator[](
    size_t idx
)
```

Provides access to element at given index with bounds checking. 

**Parameters**: 

  * **idx** Index of the element. 


**Exceptions**: 

  * **std::out_of_range** if index is invalid. 


**Return**: Reference to the element at the specified index. 

### function operator[]

```cpp
inline const T & operator[](
    size_t idx
) const
```

Provides const access to element at given index with bounds checking. 

**Parameters**: 

  * **idx** Index of the element. 


**Exceptions**: 

  * **std::out_of_range** if index is invalid. 


**Return**: Const reference to the element at the specified index. 

### function operator=

```cpp
inline vector< T > & operator=(
    const vector & other
)
```

Assignment operator for deep copying. 

**Parameters**: 

  * **other** vector to copy from. 


**Return**: Reference to this vector. 

### function capacity

```cpp
inline size_t capacity() const
```

Getter for capacity. 

**Return**: Maximum number of elements that can be stored. 

### function size

```cpp
inline size_t size() const
```

Getter for size. 

**Return**: The number of stored elements in the vector. 

### function begin

```cpp
inline T * begin()
```

Iterator to the beginning of the vector. 

**Return**: Pointer to the first element. 

### function end

```cpp
inline T * end()
```

Iterator to the end of the vector. 

**Return**: Pointer to one-past-the-last element. 

### function begin

```cpp
inline const T * begin() const
```

Const iterator to the beginning of the vector. 

**Return**: Const pointer to the first element. 

### function end

```cpp
inline const T * end() const
```

Const iterator to the end of the vector. 

**Return**: Const pointer to one-past-the-last element. 

### function clear

```cpp
inline void clear()
```

Clears the contents of the vector. 

Destroys all elements (if not pointers) and resets the size to zero. 


### function resize

```cpp
inline void resize(
    size_t newCapacity
)
```

Resizes the vector to a new capacity. 

**Parameters**: 

  * **newCapacity** The new capacity to allocate. 


Copies existing elements up to the new capacity.


### function ~vector

```cpp
inline ~vector()
```

Destructor. Clears and deallocates the vector. 

-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200