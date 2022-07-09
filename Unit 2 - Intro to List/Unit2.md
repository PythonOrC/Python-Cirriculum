#  Unit 2 - Intro to List

## 2.0 Table of Contents

[TOC]

## 2.1 - What Is a List
- A series of elements arranged in a certain order
- can store (basically) infinite number of data
- data stored inside can be of different data types
- represented with `[]` and the elements are separated with `,`

Example: <u>[`seasons_1.py`](####`seasons.py`)</u>

### 2.1.1 - Access Elements in List
- List is stored in a certain order
- to access an element you need a location, or index
- insert the index of the element in the `[]` after the list variable to get that element
  - `list[index]`
- index starts at `0`
  - e.g. the index of the third element of the list is `2`

Example: <u>[`seasons_1_1.py`](####`seasons_1_1.py`)</u>
### Sample Code
#### `seasons_1.py`
```python
seasons = ["Srping", "Summer","Autumn/Fall","Winter"]
print(seasons)
```
__Output:__ 
```
['Srping', 'Summer', 'Autumn/Fall', 'Winter']
```
#### `seasons_1_1.py`
```python
seasons = ["Srping", "Summer","Autumn/Fall","Winter"]
print(seasons[0])
```
__Output:__ 
```
['Srping', 'Summer', 'Autumn/Fall', 'Winter']
```
## Homework