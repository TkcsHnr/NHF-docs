---
title: test.cpp

---

# test.cpp



## Functions

|                | Name           |
| -------------- | -------------- |
| void | **[testVector2D](/Files/test_8cpp/#function-testvector2d)**()<br>Tests the functionality of the [Vector2D](/Classes/class_vector2_d/) class.  |
| void | **[testCustomVector](/Files/test_8cpp/#function-testcustomvector)**()<br>Tests the custom vector implementation.  |
| void | **[testCpGetline](/Files/test_8cpp/#function-testcpgetline)**()<br>Tests the custom getline function cp::getline.  |
| void | **[testCircle](/Files/test_8cpp/#function-testcircle)**()<br>Tests the [Circle](/Classes/class_circle/) class.  |
| void | **[testPolygon](/Files/test_8cpp/#function-testpolygon)**()<br>Tests the [Polygon](/Classes/class_polygon/) class.  |
| void | **[testRegularPolygon](/Files/test_8cpp/#function-testregularpolygon)**()<br>Tests the [RegularPolygon](/Classes/class_regular_polygon/) class.  |
| void | **[testCollection](/Files/test_8cpp/#function-testcollection)**()<br>Tests the [ShapeCollection](/Classes/class_shape_collection/) class.  |
| int | **[main2](/Files/test_8cpp/#function-main2)**() |

## Defines

|                | Name           |
| -------------- | -------------- |
|  | **[_USE_MATH_DEFINES](/Files/test_8cpp/#define--use-math-defines)**  |


## Functions Documentation

### function testVector2D

```cpp
void testVector2D()
```

Tests the functionality of the [Vector2D](/Classes/class_vector2_d/) class. 

This function verifies constructors, operators, and methods like addition, subtraction, scalar multiplication, magnitude, distance, dot product, rotation, closest point calculation, and stream extraction. 


### function testCustomVector

```cpp
void testCustomVector()
```

Tests the custom vector implementation. 

Verifies constructors, push_back, resizing, copy and assignment, access, exception safety, clearing, and iteration functionality. 


### function testCpGetline

```cpp
void testCpGetline()
```

Tests the custom getline function cp::getline. 

Checks handling of different line endings including CR, LF, CRLF, empty lines, and multiple lines. 


### function testCircle

```cpp
void testCircle()
```

Tests the [Circle](/Classes/class_circle/) class. 

Tests constructors, clone, point containment, circle intersection and circle containment, perimeter, area, transformations (rotate, move), bounding box calculation, SVG generation, and stream extraction. 


### function testPolygon

```cpp
void testPolygon()
```

Tests the [Polygon](/Classes/class_polygon/) class. 

Tests constructors, adding points, cloning, point containment, containment and intersection with circles, perimeter, area, transformations, bounding box, SVG generation, and stream extraction. 


### function testRegularPolygon

```cpp
void testRegularPolygon()
```

Tests the [RegularPolygon](/Classes/class_regular_polygon/) class. 

Tests constructors, cloning, perimeter and area calculations, stream extraction, and vertex generation for known polygons. 


### function testCollection

```cpp
void testCollection()
```

Tests the [ShapeCollection](/Classes/class_shape_collection/) class. 

Verifies push_back, size, capacity, operator access, deep copy (copy constructor and assignment operator), and SVG printing. 


### function main2

```cpp
int main2()
```




## Macros Documentation

### define _USE_MATH_DEFINES

```cpp
#define _USE_MATH_DEFINES 
```




-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200
