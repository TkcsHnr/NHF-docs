---
title: Circle

---

# Circle





Inherits from [Shape](/Classes/class_shape/)

## Public Functions

|                | Name           |
| -------------- | -------------- |
| | **[Circle](/Classes/class_circle/#function-circle)**()<br>Default constructor. Creates an empty circle.  |
| | **[Circle](/Classes/class_circle/#function-circle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius)<br>Constructs a circle with a center and radius.  |
| | **[Circle](/Classes/class_circle/#function-circle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius, string fillColor, string borderColor)<br>Constructs a circle with center, radius and colors.  |
| virtual bool | **[containsPoint](/Classes/class_circle/#function-containspoint)**(const [Vector2D](/Classes/class_vector2_d/) & point) const override<br>Checks whether the given point lies within the shape.  |
| virtual bool | **[containedByCircle](/Classes/class_circle/#function-containedbycircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape is fully contained within a circle.  |
| virtual bool | **[intersectsCircle](/Classes/class_circle/#function-intersectscircle)**(const [Vector2D](/Classes/class_vector2_d/) & center, double radius) const override<br>Checks whether the shape intersects a circle.  |
| virtual double | **[perimeter](/Classes/class_circle/#function-perimeter)**() const override<br>Returns the perimeter of the shape.  |
| virtual double | **[area](/Classes/class_circle/#function-area)**() const override<br>Returns the area of the shape.  |
| virtual void | **[rotate](/Classes/class_circle/#function-rotate)**(double angle) override<br>Rotates the shape by a specified angle around its centroid.  |
| virtual void | **[move](/Classes/class_circle/#function-move)**(const [Vector2D](/Classes/class_vector2_d/) & offset) override<br>Moves the shape by an offset vector.  |
| virtual [BoundingBox](/Classes/struct_bounding_box/) | **[getBoundingBox](/Classes/class_circle/#function-getboundingbox)**() const override<br>Returns the bounding box of the shape.  |
| virtual string | **[generateSVG](/Classes/class_circle/#function-generatesvg)**() const override<br>Generates an SVG string representation of the shape.  |
| [Vector2D](/Classes/class_vector2_d/) | **[getCenter](/Classes/class_circle/#function-getcenter)**() const<br>Getter for circle center.  |
| double | **[getRadius](/Classes/class_circle/#function-getradius)**() const<br>Getter for circle radius.  |
| virtual [Shape](/Classes/class_shape/) * | **[clone](/Classes/class_circle/#function-clone)**() const override<br>Creates a deep copy of the shape.  |
| | **[~Circle](/Classes/class_circle/#function-~circle)**() |

## Friends

|                | Name           |
| -------------- | -------------- |
| std::istream & | **[operator>>](/Classes/class_circle/#friend-operator>>)**(std::istream & is, [Circle](/Classes/class_circle/) & circle)  |

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

### function Circle

```cpp
Circle()
```

Default constructor. Creates an empty circle. 

### function Circle

```cpp
Circle(
    const Vector2D & center,
    double radius
)
```

Constructs a circle with a center and radius. 

**Parameters**: 

  * **center** The center point of the circle. 
  * **radius** The radius of the circle. 


### function Circle

```cpp
Circle(
    const Vector2D & center,
    double radius,
    string fillColor,
    string borderColor
)
```

Constructs a circle with center, radius and colors. 

**Parameters**: 

  * **center** The center point of the circle. 
  * **radius** The radius of the circle. 
  * **fillColor** Fill color string. 
  * **borderColor** Border color string. 


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


### function area

```cpp
virtual double area() const override
```

Returns the area of the shape. 

**Return**: Area. 

**Reimplements**: [Shape::area](/Classes/class_shape/#function-area)


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


### function getCenter

```cpp
Vector2D getCenter() const
```

Getter for circle center. 

**Return**: Center point as [Vector2D](/Classes/class_vector2_d/). 

### function getRadius

```cpp
double getRadius() const
```

Getter for circle radius. 

**Return**: Radius. 

### function clone

```cpp
virtual Shape * clone() const override
```

Creates a deep copy of the shape. 

**Return**: A pointer to a new [Shape](/Classes/class_shape/) object. 

**Reimplements**: [Shape::clone](/Classes/class_shape/#function-clone)


### function ~Circle

```cpp
~Circle()
```


## Friends

### friend operator>>

```cpp
friend std::istream & operator>>(
    std::istream & is,

    Circle & circle
);
```


-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200