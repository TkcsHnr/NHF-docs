---
title: Shape
summary: Abstract base class for geometric shapes. 

---

# Shape



Abstract base class for geometric shapes.  [More...](#detailed-description)


`#include <circle.h>`

Inherited by [Circle](/Classes/class_circle/), [Polygon](/Classes/class_polygon/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| virtual bool | **[containsPoint](/Classes/class_shape/#function-containspoint)**(const [Vector2D](/Classes/class_vector2_d/) & point) const =0<br>Checks whether the given point lies within the shape.  |
| virtual bool | **[containedByCircle](/Classes/class_shape/#function-containedbycircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const =0<br>Checks whether the shape is fully contained within a circle.  |
| virtual bool | **[intersectsCircle](/Classes/class_shape/#function-intersectscircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const =0<br>Checks whether the shape intersects a circle.  |
| virtual double | **[perimeter](/Classes/class_shape/#function-perimeter)**() const =0<br>Returns the perimeter of the shape.  |
| virtual double | **[area](/Classes/class_shape/#function-area)**() const =0<br>Returns the area of the shape.  |
| virtual void | **[rotate](/Classes/class_shape/#function-rotate)**(double angle) =0<br>Rotates the shape by a specified angle around its centroid.  |
| virtual void | **[move](/Classes/class_shape/#function-move)**(const [Vector2D](/Classes/class_vector2_d/) & offset) =0<br>Moves the shape by an offset vector.  |
| virtual [BoundingBox](/Classes/struct_bounding_box/) | **[getBoundingBox](/Classes/class_shape/#function-getboundingbox)**() const =0<br>Returns the bounding box of the shape.  |
| virtual string | **[generateSVG](/Classes/class_shape/#function-generatesvg)**() const =0<br>Generates an SVG string representation of the shape.  |
| virtual [Shape](/Classes/class_shape/) * | **[clone](/Classes/class_shape/#function-clone)**() const =0<br>Creates a deep copy of the shape.  |
| virtual | **[~Shape](/Classes/class_shape/#function-~shape)**() =default<br>Virtual destructor.  |
| string | **[getFillColor](/Classes/class_shape/#function-getfillcolor)**()<br>Getter for fill color.  |
| string | **[getBorderColor](/Classes/class_shape/#function-getbordercolor)**()<br>Getter for border color.  |

## Protected Functions

|                | Name           |
| -------------- | -------------- |
| | **[Shape](/Classes/class_shape/#function-shape)**()<br>Protected default constructor.  |
| | **[Shape](/Classes/class_shape/#function-shape)**(string fillColor, string borderColor)<br>Constructs a shape with specific fill and border colors.  |

## Protected Attributes

|                | Name           |
| -------------- | -------------- |
| string | **[fillColor](/Classes/class_shape/#variable-fillcolor)**  |
| string | **[borderColor](/Classes/class_shape/#variable-bordercolor)**  |

## Detailed Description

```cpp
class Shape;
```

Abstract base class for geometric shapes. 

Represents a circle shape defined by a center point and radius.

Defines a common interface for operations like area, perimeter, transformation, SVG export, and collision detection. 

## Public Functions Documentation

### function containsPoint

```cpp
virtual bool containsPoint(
    const Vector2D & point
) const =0
```

Checks whether the given point lies within the shape. 

**Parameters**: 

  * **point** The point to test. 


**Return**: True if the point is inside the shape, false otherwise. 

**Reimplemented by**: [Circle::containsPoint](/Classes/class_circle/#function-containspoint), [Polygon::containsPoint](/Classes/class_polygon/#function-containspoint)


### function containedByCircle

```cpp
virtual bool containedByCircle(
    const Vector2D & center,
    double radius
) const =0
```

Checks whether the shape is fully contained within a circle. 

**Parameters**: 

  * **center** Center of the circle. 
  * **radius** Radius of the circle. 


**Return**: True if the shape lies entirely within the circle. 

**Reimplemented by**: [Circle::containedByCircle](/Classes/class_circle/#function-containedbycircle), [Polygon::containedByCircle](/Classes/class_polygon/#function-containedbycircle)


### function intersectsCircle

```cpp
virtual bool intersectsCircle(
    const Vector2D & center,
    double radius
) const =0
```

Checks whether the shape intersects a circle. 

**Parameters**: 

  * **center** Center of the circle. 
  * **radius** Radius of the circle. 


**Return**: True if the shape and circle overlap. 

**Reimplemented by**: [Circle::intersectsCircle](/Classes/class_circle/#function-intersectscircle), [Polygon::intersectsCircle](/Classes/class_polygon/#function-intersectscircle)


### function perimeter

```cpp
virtual double perimeter() const =0
```

Returns the perimeter of the shape. 

**Return**: Perimeter. 

**Reimplemented by**: [Circle::perimeter](/Classes/class_circle/#function-perimeter), [Polygon::perimeter](/Classes/class_polygon/#function-perimeter), [RegularPolygon::perimeter](/Classes/class_regular_polygon/#function-perimeter)


### function area

```cpp
virtual double area() const =0
```

Returns the area of the shape. 

**Return**: Area. 

**Reimplemented by**: [Circle::area](/Classes/class_circle/#function-area), [Polygon::area](/Classes/class_polygon/#function-area), [RegularPolygon::area](/Classes/class_regular_polygon/#function-area)


### function rotate

```cpp
virtual void rotate(
    double angle
) =0
```

Rotates the shape by a specified angle around its centroid. 

**Parameters**: 

  * **angle** Rotation angle in degrees. 


**Reimplemented by**: [Circle::rotate](/Classes/class_circle/#function-rotate), [Polygon::rotate](/Classes/class_polygon/#function-rotate)


### function move

```cpp
virtual void move(
    const Vector2D & offset
) =0
```

Moves the shape by an offset vector. 

**Parameters**: 

  * **offset** The offset vector. 


**Reimplemented by**: [Circle::move](/Classes/class_circle/#function-move), [Polygon::move](/Classes/class_polygon/#function-move)


### function getBoundingBox

```cpp
virtual BoundingBox getBoundingBox() const =0
```

Returns the bounding box of the shape. 

**Return**: [BoundingBox](/Classes/struct_bounding_box/). 

**Reimplemented by**: [Circle::getBoundingBox](/Classes/class_circle/#function-getboundingbox), [Polygon::getBoundingBox](/Classes/class_polygon/#function-getboundingbox)


### function generateSVG

```cpp
virtual string generateSVG() const =0
```

Generates an SVG string representation of the shape. 

**Return**: A string containing SVG markup for the shape. 

**Reimplemented by**: [Circle::generateSVG](/Classes/class_circle/#function-generatesvg), [Polygon::generateSVG](/Classes/class_polygon/#function-generatesvg)


### function clone

```cpp
virtual Shape * clone() const =0
```

Creates a deep copy of the shape. 

**Return**: A pointer to a new [Shape](/Classes/class_shape/) object. 

**Reimplemented by**: [Circle::clone](/Classes/class_circle/#function-clone), [Polygon::clone](/Classes/class_polygon/#function-clone), [RegularPolygon::clone](/Classes/class_regular_polygon/#function-clone)


### function ~Shape

```cpp
virtual ~Shape() =default
```

Virtual destructor. 

### function getFillColor

```cpp
string getFillColor()
```

Getter for fill color. 

**Return**: Fill color as a string. 

### function getBorderColor

```cpp
string getBorderColor()
```

Getter for border color. 

**Return**: Border color as a string. 

## Protected Functions Documentation

### function Shape

```cpp
Shape()
```

Protected default constructor. 

### function Shape

```cpp
Shape(
    string fillColor,
    string borderColor
)
```

Constructs a shape with specific fill and border colors. 

**Parameters**: 

  * **fillColor** Fill color of the shape. 
  * **borderColor** Border (stroke) color of the shape. 


## Protected Attributes Documentation

### variable fillColor

```cpp
string fillColor;
```


Fill color for SVG rendering 


### variable borderColor

```cpp
string borderColor;
```


Border color for SVG rendering 


-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200