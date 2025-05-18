---
title: RegularPolygon
summary: Represents a regular polygon with equal-length sides and equal angles. 

---

# RegularPolygon



Represents a regular polygon with equal-length sides and equal angles.  [More...](#detailed-description)


`#include <regular_polygon.h>`

Inherits from [Polygon](/Classes/class_polygon/), [Shape](/Classes/class_shape/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[RegularPolygon](/Classes/class_regular_polygon/#function-regularpolygon)**()<br>Default constructor. Creates an empty [RegularPolygon](/Classes/class_regular_polygon/).  |
| | **[RegularPolygon](/Classes/class_regular_polygon/#function-regularpolygon)**(size_t n, double radius, const [Vector2D](/Classes/class_vector2_d/) & center)<br>Constructs a regular polygon.  |
| | **[RegularPolygon](/Classes/class_regular_polygon/#function-regularpolygon)**(size_t n, double radius, const [Vector2D](/Classes/class_vector2_d/) & center, string fillColor, string borderColor)<br>Constructs a regular polygon with color options.  |
| void | **[generateVertices](/Classes/class_regular_polygon/#function-generatevertices)**(const [Vector2D](/Classes/class_vector2_d/) & center)<br>Generates the vertices of the regular polygon based on center, radius, and number of sides.  |
| virtual double | **[perimeter](/Classes/class_regular_polygon/#function-perimeter)**() const override<br>Returns the perimeter of the shape.  |
| virtual double | **[area](/Classes/class_regular_polygon/#function-area)**() const override<br>Returns the area of the shape.  |
| virtual [Shape](/Classes/class_shape/) * | **[clone](/Classes/class_regular_polygon/#function-clone)**() const override<br>Creates a deep copy of the shape.  |
| | **[~RegularPolygon](/Classes/class_regular_polygon/#function-~regularpolygon)**() |

## Friends

|                | Name           |
| -------------- | -------------- |
| std::istream & | **[operator>>](/Classes/class_regular_polygon/#friend-operator>>)**(std::istream & is, [RegularPolygon](/Classes/class_regular_polygon/) & polygon)  |

## Additional inherited members

**Public Functions inherited from [Polygon](/Classes/class_polygon/)**

|                | Name           |
| -------------- | -------------- |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**()<br>Default constructor. Creates an empty polygon.  |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**([vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > vertices)<br>Constructs a polygon with a list of vertices.  |
| | **[Polygon](/Classes/class_polygon/#function-polygon)**([vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > vertices, string fillColor, string borderColor)<br>Constructs a polygon with vertices and color settings.  |
| const [vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > | **[getPoints](/Classes/class_polygon/#function-getpoints)**() const<br>Getter for vertices (const).  |
| virtual bool | **[containsPoint](/Classes/class_polygon/#function-containspoint)**(const [Vector2D](/Classes/class_vector2_d/) & point) const override<br>Checks whether the given point lies within the shape.  |
| virtual bool | **[containedByCircle](/Classes/class_polygon/#function-containedbycircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape is fully contained within a circle.  |
| virtual bool | **[intersectsCircle](/Classes/class_polygon/#function-intersectscircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape intersects a circle.  |
| virtual void | **[rotate](/Classes/class_polygon/#function-rotate)**(double angle) override<br>Rotates the shape by a specified angle around its centroid.  |
| virtual void | **[move](/Classes/class_polygon/#function-move)**(const [Vector2D](/Classes/class_vector2_d/) & offset) override<br>Moves the shape by an offset vector.  |
| [Vector2D](/Classes/class_vector2_d/) | **[centroid](/Classes/class_polygon/#function-centroid)**() const<br>Computes the centroid (geometric center) of the polygon.  |
| virtual [BoundingBox](/Classes/struct_bounding_box/) | **[getBoundingBox](/Classes/class_polygon/#function-getboundingbox)**() const override<br>Returns the bounding box of the shape.  |
| virtual string | **[generateSVG](/Classes/class_polygon/#function-generatesvg)**() const override<br>Generates an SVG string representation of the shape.  |
| | **[~Polygon](/Classes/class_polygon/#function-~polygon)**() |

**Protected Attributes inherited from [Polygon](/Classes/class_polygon/)**

|                | Name           |
| -------------- | -------------- |
| [vector](/Classes/classvector/)< [Vector2D](/Classes/class_vector2_d/) > | **[vertices](/Classes/class_polygon/#variable-vertices)**  |

**Public Functions inherited from [Shape](/Classes/class_shape/)**

|                | Name           |
| -------------- | -------------- |
| virtual bool | **[containsPoint](/Classes/class_shape/#function-containspoint)**(const [Vector2D](/Classes/class_vector2_d/) & point) const =0<br>Checks whether the given point lies within the shape.  |
| virtual bool | **[containedByCircle](/Classes/class_shape/#function-containedbycircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const =0<br>Checks whether the shape is fully contained within a circle.  |
| virtual bool | **[intersectsCircle](/Classes/class_shape/#function-intersectscircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const =0<br>Checks whether the shape intersects a circle.  |
| virtual void | **[rotate](/Classes/class_shape/#function-rotate)**(double angle) =0<br>Rotates the shape by a specified angle around its centroid.  |
| virtual void | **[move](/Classes/class_shape/#function-move)**(const [Vector2D](/Classes/class_vector2_d/) & offset) =0<br>Moves the shape by an offset vector.  |
| virtual [BoundingBox](/Classes/struct_bounding_box/) | **[getBoundingBox](/Classes/class_shape/#function-getboundingbox)**() const =0<br>Returns the bounding box of the shape.  |
| virtual string | **[generateSVG](/Classes/class_shape/#function-generatesvg)**() const =0<br>Generates an SVG string representation of the shape.  |
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


## Detailed Description

```cpp
class RegularPolygon;
```

Represents a regular polygon with equal-length sides and equal angles. 

This class inherits from [Polygon](/Classes/class_polygon/) and defines a polygon with 'n' sides and a fixed radius, centered at a given point. 

## Public Functions Documentation

### function RegularPolygon

```cpp
RegularPolygon()
```

Default constructor. Creates an empty [RegularPolygon](/Classes/class_regular_polygon/). 

### function RegularPolygon

```cpp
RegularPolygon(
    size_t n,
    double radius,
    const Vector2D & center
)
```

Constructs a regular polygon. 

**Parameters**: 

  * **n** Number of sides. 
  * **radius** Radius of the circumcircle. 
  * **center** Center of the polygon. 


### function RegularPolygon

```cpp
RegularPolygon(
    size_t n,
    double radius,
    const Vector2D & center,
    string fillColor,
    string borderColor
)
```

Constructs a regular polygon with color options. 

**Parameters**: 

  * **n** Number of sides. 
  * **radius** Radius of the circumcircle. 
  * **center** Center of the polygon. 
  * **fillColor** Fill color string. 
  * **borderColor** Border color string. 


### function generateVertices

```cpp
void generateVertices(
    const Vector2D & center
)
```

Generates the vertices of the regular polygon based on center, radius, and number of sides. 

**Parameters**: 

  * **center** Center of the polygon. 


### function perimeter

```cpp
virtual double perimeter() const override
```

Returns the perimeter of the shape. 

**Return**: Perimeter. 

**Reimplements**: [Polygon::perimeter](/Classes/class_polygon/#function-perimeter)


### function area

```cpp
virtual double area() const override
```

Returns the area of the shape. 

**Return**: Area. 

**Reimplements**: [Polygon::area](/Classes/class_polygon/#function-area)


### function clone

```cpp
virtual Shape * clone() const override
```

Creates a deep copy of the shape. 

**Return**: A pointer to a new [Shape](/Classes/class_shape/) object. 

**Reimplements**: [Polygon::clone](/Classes/class_polygon/#function-clone)


### function ~RegularPolygon

```cpp
~RegularPolygon()
```


## Friends

### friend operator>>

```cpp
friend std::istream & operator>>(
    std::istream & is,

    RegularPolygon & polygon
);
```


-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200