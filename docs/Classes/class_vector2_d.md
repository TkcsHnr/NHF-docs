---
title: Vector2D
summary: A class representing a 2D vector with basic operations. 

---

# Vector2D



A class representing a 2D vector with basic operations. 


`#include <vector2D.h>`

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[Vector2D](/Classes/class_vector2_d/#function-vector2d)**()<br>Default constructor. Initializes vector to (0,0).  |
| | **[Vector2D](/Classes/class_vector2_d/#function-vector2d)**(double x, double y)<br>Constructs a vector with the specified x and y components.  |
| | **[Vector2D](/Classes/class_vector2_d/#function-vector2d)**(const [Vector2D](/Classes/class_vector2_d/) & other)<br>Copy constructor.  |
| double | **[abs](/Classes/class_vector2_d/#function-abs)**() const<br>Calculates the magnitude (length) of the vector.  |
| double | **[distance](/Classes/class_vector2_d/#function-distance)**(const [Vector2D](/Classes/class_vector2_d/) & other) const<br>Calculates the Euclidean distance to another vector.  |
| [Vector2D](/Classes/class_vector2_d/) | **[operator+](/Classes/class_vector2_d/#function-operator+)**(const [Vector2D](/Classes/class_vector2_d/) & other) const<br>Adds two vectors.  |
| [Vector2D](/Classes/class_vector2_d/) | **[operator-](/Classes/class_vector2_d/#function-operator-)**(const [Vector2D](/Classes/class_vector2_d/) & other) const<br>Subtracts one vector from another.  |
| [Vector2D](/Classes/class_vector2_d/) | **[operator*](/Classes/class_vector2_d/#function-operator*)**(double scalar) const<br>Multiplies the vector by a scalar.  |
| [Vector2D](/Classes/class_vector2_d/) & | **[operator=](/Classes/class_vector2_d/#function-operator=)**(const [Vector2D](/Classes/class_vector2_d/) & other)<br>Assignment operator.  |
| bool | **[operator==](/Classes/class_vector2_d/#function-operator==)**(const [Vector2D](/Classes/class_vector2_d/) & other) const<br>Equality comparison operator.  |
| void | **[rotate](/Classes/class_vector2_d/#function-rotate)**(const [Vector2D](/Classes/class_vector2_d/) & center, double angle)<br>Rotates the vector around a given center by a specified angle.  |
| double | **[dot](/Classes/class_vector2_d/#function-dot)**(const [Vector2D](/Classes/class_vector2_d/) & other) const<br>Calculates the dot product with another vector.  |
| [Vector2D](/Classes/class_vector2_d/) | **[closestPointOnSegment](/Classes/class_vector2_d/#function-closestpointonsegment)**(const [Vector2D](/Classes/class_vector2_d/) & v1, const [Vector2D](/Classes/class_vector2_d/) & v2) const<br>Finds the closest point on a line segment to this point.  |
| double | **[getX](/Classes/class_vector2_d/#function-getx)**() const<br>Getter for X component of the vector.  |
| double | **[getY](/Classes/class_vector2_d/#function-gety)**() const<br>Getter for Y component of the vector.  |

## Friends

|                | Name           |
| -------------- | -------------- |
| std::istream & | **[operator>>](/Classes/class_vector2_d/#friend-operator>>)**(std::istream & is, [Vector2D](/Classes/class_vector2_d/) & vec) <br>Input stream operator for reading a vector.  |

## Public Functions Documentation

### function Vector2D

```cpp
Vector2D()
```

Default constructor. Initializes vector to (0,0). 

### function Vector2D

```cpp
Vector2D(
    double x,
    double y
)
```

Constructs a vector with the specified x and y components. 

**Parameters**: 

  * **x** X component of the vector. 
  * **y** Y component of the vector. 


### function Vector2D

```cpp
Vector2D(
    const Vector2D & other
)
```

Copy constructor. 

**Parameters**: 

  * **other** Another [Vector2D](/Classes/class_vector2_d/) object to copy from. 


### function abs

```cpp
double abs() const
```

Calculates the magnitude (length) of the vector. 

**Return**: The absolute value of the vector. 

### function distance

```cpp
double distance(
    const Vector2D & other
) const
```

Calculates the Euclidean distance to another vector. 

**Parameters**: 

  * **other** Another [Vector2D](/Classes/class_vector2_d/) object. 


**Return**: Distance between this vector and the other vector. 

### function operator+

```cpp
Vector2D operator+(
    const Vector2D & other
) const
```

Adds two vectors. 

**Parameters**: 

  * **other** The vector to add. 


**Return**: A new [Vector2D](/Classes/class_vector2_d/) which is the sum of the two vectors. 

### function operator-

```cpp
Vector2D operator-(
    const Vector2D & other
) const
```

Subtracts one vector from another. 

**Parameters**: 

  * **other** The vector to subtract. 


**Return**: A new [Vector2D](/Classes/class_vector2_d/) which is the difference of the two vectors. 

### function operator*

```cpp
Vector2D operator*(
    double scalar
) const
```

Multiplies the vector by a scalar. 

**Parameters**: 

  * **scalar** The scalar value. 


**Return**: A new [Vector2D](/Classes/class_vector2_d/) scaled by the given scalar. 

### function operator=

```cpp
Vector2D & operator=(
    const Vector2D & other
)
```

Assignment operator. 

**Parameters**: 

  * **other** The vector to assign from. 


**Return**: A reference to this vector after assignment. 

### function operator==

```cpp
bool operator==(
    const Vector2D & other
) const
```

Equality comparison operator. 

**Parameters**: 

  * **other** The vector to compare with. 


**Return**: True if both vectors have the same components, false otherwise. 

### function rotate

```cpp
void rotate(
    const Vector2D & center,
    double angle
)
```

Rotates the vector around a given center by a specified angle. 

**Parameters**: 

  * **center** The point around which to rotate. 
  * **angle** The angle in degrees. 


### function dot

```cpp
double dot(
    const Vector2D & other
) const
```

Calculates the dot product with another vector. 

**Parameters**: 

  * **other** The other vector. 


**Return**: The dot product of the two vectors. 

### function closestPointOnSegment

```cpp
Vector2D closestPointOnSegment(
    const Vector2D & v1,
    const Vector2D & v2
) const
```

Finds the closest point on a line segment to this point. 

**Parameters**: 

  * **v1** One endpoint of the segment. 
  * **v2** Other endpoint of the segment. 


**Return**: The closest point on the segment to this point. 

### function getX

```cpp
double getX() const
```

Getter for X component of the vector. 

**Return**: The X value. 

### function getY

```cpp
double getY() const
```

Getter for Y component of the vector. 

**Return**: The Y value. 

## Friends

### friend operator>>

```cpp
friend std::istream & operator>>(
    std::istream & is,

    Vector2D & vec
);
```

Input stream operator for reading a vector. 

**Parameters**: 

  * **is** Input stream. 
  * **vec** The vector to read into. 


**Return**: Reference to the input stream. 

-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200