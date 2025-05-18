---
title: cp

---

# cp



## Functions

|                | Name           |
| -------------- | -------------- |
| std::istream & | **[getline](/Namespaces/namespacecp/#function-getline)**(std::istream & is, std::string & str)<br>Cross-platform version of std::getline.  |


## Functions Documentation

### function getline

```cpp
std::istream & getline(
    std::istream & is,
    std::string & str
)
```

Cross-platform version of std::getline. 

**Parameters**: 

  * **is** The input stream to read from. 
  * **str** The string where the line will be stored. 


**Return**: Reference to the input stream. 

Reads a line from the input stream, handling both Unix (`\n`) and Windows (`\r\n`) line endings.






-------------------------------

Updated on 2025-05-18 at 19:18:06 +0200