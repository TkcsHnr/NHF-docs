---
title: Polygon
summary: Represents a polygon shape defined by a list of 2D vertices. 

---

# Polygon



Represents a polygon shape defined by a list of 2D vertices. 


`#include <polygon.h>`

Inherits from [Shape](/Classes/class_shape/)

Inherited by [RegularPolygon](/Classes/class_regular_polygon/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**()<br>Default constructor. Creates an empty polygon.  |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**([vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > vertices)<br>Constructs a polygon with a list of vertices.  |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**([vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > vertices, string fillColor, string borderColor)<br>Constructs a polygon with vertices and color settings.  |
| virtual bool | **[addPoint](/Classes/class_polygon/#function-addpoint)**(const [Vector2D](/Classes/class_vector2_d/) & point)<br>Adds a new vertex to the polygon.  |
| const [vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > | **[getPoints](/Classes/class_polygon/#function-getpoints)**() const<br>Getter for vertices (const).  |
| virtual bool | **[containsPoint](/Classes/class_polygon/#function-containspoint)**(const [Vector2D](/Classes/class_vector2_d/) & point) const override<br>Checks whether the given point lies within the shape.  |
| virtual bool | **[containedByCircle](/Classes/class_polygon/#function-containedbycircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape is fully contained within a circle.  |
| virtual bool | **[intersectsCircle](/Classes/class_polygon/#function-intersectscircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape intersects a circle.  |
| virtual double | **[perimeter](/Classes/class_polygon/#function-perimeter)**() const override<br>Returns the perimeter of the shape.  |
| virtual double | **[area](/Classes/class_polygon/#function-area)**() const override<br>Returns the area of the shape.  |
| virtual void | **[rotate](/Classes/class_polygon/#function-rotate)**(double angle) override<br>Rotates the shape by a specified angle around its centroid.  |
| virtual void | **[move](/Classes/class_polygon/#function-move)**(const [Vector2D](/Classes/class_vector2_d/) & offset) override<br>Moves the shape by an offset vector.  |
| [Vector2D](/Classes/class_vector2_d/) | **[centroid](/Classes/class_polygon/#function-centroid)**() const<br>Computes the centroid (geometric center) of the polygon.  |
| virtual [BoundingBox](/Classes/struct_bounding_box/) | **[getBoundingBox](/Classes/class_polygon/#function-getboundingbox)**() const override<br>Returns the bounding box of the shape.  |
| virtual string | **[generateSVG](/Classes/class_polygon/#function-generatesvg)**() const override<br>Generates an SVG string representation of the shape.  |
| virtual [Shape](/Classes/class_shape/) * | **[clone](/Classes/class_polygon/#function-clone)**() const override<br>Creates a deep copy of the shape.  |
| | **[~Polygon](/Classes/class_polygon/#function-~polygon)**() |

## Protected Attributes

|                | Name           |
| -------------- | -------------- |
| [vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > | **[vertices](/Classes/class_polygon/#variable-vertices)**  |

## Friends

|                | Name           |
| -------------- | -------------- |
| std::istream & | **[operator>>](/Classes/class_polygon/#friend-operator>>)**(std::istream & is, [Polygon](/Classes/class_polygon/) & polygon)  |

## Additional inherited members

**Public Functions inherited from [Shape](/Classes/class_shape/)**

|                | Name           |
| -------------- | -------------- |
| virtual | **[~Shape](/Classes/class_shape/#function-~shape)**() =default<br>Virtual destructor.  |
| string | **[getFillColor](/Classes/class_shape/#function-getfillcolor)**()<br>Getter for fill color.  |
| string | **[getBorderColor](/Classes/class_shape/#function-getbordercolor)**()<br>Getter for border color.  |

**Protected Functions inherited from [Shape](/Classes/class_shape/)**

|                | Name           |
| -------------- | -------------- |
| | **[Shape](/Classes/class_shape/#function-shape)**()<br>Protected default constructor.  |
| | **[Shape](/Classes/class_shape/#function-shape)**(string fillColor, string borderColor)<br>Constructs a shape with specific fill and border colors.  |

**Protected Attributes inherited from [Shape](/Classes/class_shape/)**

|                | Name           |
| -------------- | -------------- |
| string | **[fillColor](/Classes/class_shape/#variable-fillcolor)**  |
| string | **[borderColor](/Classes/class_shape/#variable-bordercolor)**  |


## Public Functions Documentation

### function Polygon

```cpp
Polygon()
```

Default constructor. Creates an empty polygon. 

### function Polygon

```cpp
Polygon(
    vector< Vector2D > vertices
)
```

Constructs a polygon with a list of vertices. 

**Parameters**: 

  * **vertices** A vector of points defining the polygon. 


### function Polygon

```cpp
Polygon(
    vector< Vector2D > vertices,
    string fillColor,
    string borderColor
)
```

Constructs a polygon with vertices and color settings. 

**Parameters**: 

  * **vertices** A vector of polygon points. 
  * **fillColor** The fill color of the polygon. 
  * **borderColor** The border color of the polygon. 


### function addPoint

```cpp
virtual bool addPoint(
    const Vector2D & point
)
```

Adds a new vertex to the polygon. 

**Parameters**: 

  * **point** The point to add. 


**Return**: True if added, false if not (repeated). 

**Reimplemented by**: [RegularPolygon::addPoint](/Classes/class_regular_polygon/#function-addpoint)


### function getPoints

```cpp
const vector< Vector2D > getPoints() const
```

Getter for vertices (const). 

**Return**: A vector of 2D points. 

### function containsPoint

```cpp
virtual bool containsPoint(
    const Vector2D & point
) const override
```

Checks whether the given point lies within the shape. 

**Parameters**: 

  * **point** The point to test. 


**Return**: True if the point is inside the shape, false otherwise. 

**Reimplements**: [Shape::containsPoint](/Classes/class_shape/#function-containspoint)


### function containedByCircle

```cpp
virtual bool containedByCircle(
    const Vector2D & center,
    double radius
) const override
```

Checks whether the shape is fully contained within a circle. 

**Parameters**: 

  * **center** Center of the circle. 
  * **radius** Radius of the circle. 


**Return**: True if the shape lies entirely within the circle. 

**Reimplements**: [Shape::containedByCircle](/Classes/class_shape/#function-containedbycircle)


### function intersectsCircle

```cpp
virtual bool intersectsCircle(
    const Vector2D & center,
    double radius
) const override
```

Checks whether the shape intersects a circle. 

**Parameters**: 

  * **center** Center of the circle. 
  * **radius** Radius of the circle. 


**Return**: True if the shape and circle overlap. 

**Reimplements**: [Shape::intersectsCircle](/Classes/class_shape/#function-intersectscircle)


### function perimeter

```cpp
virtual double perimeter() const override
```

Returns the perimeter of the shape. 

**Return**: Perimeter. 

**Reimplements**: [Shape::perimeter](/Classes/class_shape/#function-perimeter)


**Reimplemented by**: [RegularPolygon::perimeter](/Classes/class_regular_polygon/#function-perimeter)


### function area

```cpp
virtual double area() const override
```

Returns the area of the shape. 

**Return**: Area. 

**Reimplements**: [Shape::area](/Classes/class_shape/#function-area)


**Reimplemented by**: [RegularPolygon::area](/Classes/class_regular_polygon/#function-area)


### function rotate

```cpp
virtual void rotate(
    double angle
) override
```

Rotates the shape by a specified angle around its centroid. 

**Parameters**: 

  * **angle** Rotation angle in degrees. 


**Reimplements**: [Shape::rotate](/Classes/class_shape/#function-rotate)


### function move

```cpp
virtual void move(
    const Vector2D & offset
) override
```

Moves the shape by an offset vector. 

**Parameters**: 

  * **offset** The offset vector. 


**Reimplements**: [Shape::move](/Classes/class_shape/#function-move)


### function centroid

```cpp
Vector2D centroid() const
```

Computes the centroid (geometric center) of the polygon. 

**Return**: The centroid point as a [Vector2D](/Classes/class_vector2_d/). 

### function getBoundingBox

```cpp
virtual BoundingBox getBoundingBox() const override
```

Returns the bounding box of the shape. 

**Return**: [BoundingBox](/Classes/struct_bounding_box/). 

**Reimplements**: [Shape::getBoundingBox](/Classes/class_shape/#function-getboundingbox)


### function generateSVG

```cpp
virtual string generateSVG() const override
```

Generates an SVG string representation of the shape. 

**Return**: A string containing SVG markup for the shape. 

**Reimplements**: [Shape::generateSVG](/Classes/class_shape/#function-generatesvg)


### function clone

```cpp
virtual Shape * clone() const override
```

Creates a deep copy of the shape. 

**Return**: A pointer to a new [Shape](/Classes/class_shape/) object. 

**Reimplements**: [Shape::clone](/Classes/class_shape/#function-clone)


**Reimplemented by**: [RegularPolygon::clone](/Classes/class_regular_polygon/#function-clone)


### function ~Polygon

```cpp
~Polygon()
```


## Protected Attributes Documentation

### variable vertices

```cpp
vector< Vector2D > vertices;
```


List of polygon vertices 


## Friends

### friend operator>>

```cpp
friend std::istream & operator>>(
    std::istream & is,

    Polygon & polygon
);
```


-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200