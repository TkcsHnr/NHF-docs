---
title: ShapeCollection
summary: A container class for managing a collection of Shape pointers. 

---

# ShapeCollection



A container class for managing a collection of [Shape](/Classes/class_shape/) pointers.  [More...](#detailed-description)


`#include <shape_collection.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[ShapeCollection](/Classes/class_shape_collection/#function-shapecollection)**()<br>Default constructor. Creates an empty collection.  |
| | **[ShapeCollection](/Classes/class_shape_collection/#function-shapecollection)**(size_t capacity)<br>Constructor with preallocated capacity.  |
| | **[ShapeCollection](/Classes/class_shape_collection/#function-shapecollection)**(const [ShapeCollection](/Classes/class_shape_collection/) & other)<br>Copy constructor.  |
| [ShapeCollection](/Classes/class_shape_collection/) & | **[operator=](/Classes/class_shape_collection/#function-operator=)**(const [ShapeCollection](/Classes/class_shape_collection/) & other)<br>Assignment operator.  |
| void | **[push_back](/Classes/class_shape_collection/#function-push-back)**([Shape](/Classes/class_shape/) * shape)<br>Adds a shape pointer to the collection.  |
| [Shape](/Classes/class_shape/) * | **[operator[]](/Classes/class_shape_collection/#function-operator[])**(size_t idx)<br>Provides access to shape by index (non-const).  |
| const [Shape](/Classes/class_shape/) * | **[operator[]](/Classes/class_shape_collection/#function-operator[])**(size_t idx) const<br>Provides access to shape by index (const).  |
| size_t | **[capacity](/Classes/class_shape_collection/#function-capacity)**() const<br>Getter for capacity.  |
| size_t | **[size](/Classes/class_shape_collection/#function-size)**() const<br>Getter for size.  |
| void | **[printSVG](/Classes/class_shape_collection/#function-printsvg)**(std::ostream & out) const<br>Outputs all shapes in the collection as SVG elements.  |
| void | **[clear](/Classes/class_shape_collection/#function-clear)**()<br>Clears the collection.  |
| | **[~ShapeCollection](/Classes/class_shape_collection/#function-~shapecollection)**()<br>Destructor. Cleans up all dynamically allocated shapes.  |

## Detailed Description

```cpp
class ShapeCollection;
```

A container class for managing a collection of [Shape](/Classes/class_shape/) pointers. 

Provides basic operations such as adding shapes, accessing by index, and exporting the collection as an SVG representation. 

## Public Functions Documentation

### function ShapeCollection

```cpp
ShapeCollection()
```

Default constructor. Creates an empty collection. 

### function ShapeCollection

```cpp
ShapeCollection(
    size_t capacity
)
```

Constructor with preallocated capacity. 

**Parameters**: 

  * **capacity** Initial capacity of the collection. 


### function ShapeCollection

```cpp
ShapeCollection(
    const ShapeCollection & other
)
```

Copy constructor. 

**Parameters**: 

  * **other** The [ShapeCollection](/Classes/class_shape_collection/) to copy from. 


### function operator=

```cpp
ShapeCollection & operator=(
    const ShapeCollection & other
)
```

Assignment operator. 

**Parameters**: 

  * **other** The [ShapeCollection](/Classes/class_shape_collection/) to copy from. 


**Return**: Reference to this collection after assignment. 

### function push_back

```cpp
void push_back(
    Shape * shape
)
```

Adds a shape pointer to the collection. 

**Parameters**: 

  * **shape** Pointer to the shape to add. 


### function operator[]

```cpp
Shape * operator[](
    size_t idx
)
```

Provides access to shape by index (non-const). 

**Parameters**: 

  * **idx** Index of the shape. 


**Return**: Pointer to the shape at the specified index. 

### function operator[]

```cpp
const Shape * operator[](
    size_t idx
) const
```

Provides access to shape by index (const). 

**Parameters**: 

  * **idx** Index of the shape. 


**Return**: Const pointer to the shape at the specified index. 

### function capacity

```cpp
size_t capacity() const
```

Getter for capacity. 

**Return**: Max number of shapes the collection can hold. 

### function size

```cpp
size_t size() const
```

Getter for size. 

**Return**: Current number of stored shapes. 

### function printSVG

```cpp
void printSVG(
    std::ostream & out
) const
```

Outputs all shapes in the collection as SVG elements. 

**Parameters**: 

  * **out** Output stream to write the SVG content to. 


### function clear

```cpp
void clear()
```

Clears the collection. 

Deletes all [Shape](/Classes/class_shape/) pointers and resets the collection. 


### function ~ShapeCollection

```cpp
~ShapeCollection()
```

Destructor. Cleans up all dynamically allocated shapes. 

-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200