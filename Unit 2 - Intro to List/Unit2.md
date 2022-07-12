#  Unit 2 - Intro to List



## 2.0 Table of Contents

[TOC]



## 2.1 - What Is a List

- A series of elements arranged in a certain order
- can store (basically) an infinite number of data
- data stored inside can be of different data types
- represented with `[]` and the elements are separated with `,`

Example: <u>[`seasons.py`](####`seasons.py`)</u>

<img src="assets/sPZmw20MjHKTu4QIMcupuLDQA-BfEDX51KIG63H-CYiYsTRQyLmMxPYE3Pr8qd9DfxfuoZJrP6tdDyI5p6Jnq0lpSNrZ8rSPX9444GoIZKY-kKpT2cKljK_qBAnUCHSCwU31x0mExUh7TZCTzHYw.png" alt="img" style="zoom:50%;" />

### 2.1.1 - Access Elements in List

- The list is stored in a certain order
- to access an element you need a location, or index
- insert the index of the element in the `[]` after the list variable to get that element
  - `list[index]`
- index starts at `0`
  - e.g. the index of the third element of the list is `2`
- each element should be treated like an individual variable
  - actions of a variable can also be performed on a list
  Example: <u>[`seasons_index.py`](####`seasons_index.py`)</u>
- negative index will count elements backwards
Example: <u>[`seasons_reverse_index.py`](####`seasons_reverse_index.py`)</u

## 2.2 Add, Edit, Remove Elements

- list is dynamic
  - can be edited as code runs
  - use cases
    - inventory of character
    - users of a website

### 2.2.1 Edit an Element
- similar to variables and accessing element
  - list name
  - index
  - new vlaue
  Example: <u>[`seasons_edit.py`](####`seasons_edit.py`)</u>

### 2.2.2 Add an Element
 - There are two major ways to add values to a list
1. Add to the end
   - `list.append(value)`
2. Add to the middle
   - `list.insert(index, value)`
   - all values after will increase `index` by `1`
   Example: <u>[`seasons_add.py`](####`seasons_add.py`)</u>

### Remove an Element

 - There are three ways to delete an value, each with their use cases
1. `del`
   - `del list[index]`
   - used when knowing the index
   Example: <u>[`seasons_del.py`](####`seasons_del.py`)</u>
2. `pop()`
   - `list.pop()` or `list.pop(index)`
   - used when the value is needed for operations
   Example: <u>[`seasons_pop.py`](####`seasons_pop.py`)</u>
3. `remove()`
   - `lis.remove(element)`
   - used when knowing the value of the element
   Example: <u>[`seasons_remove.py`](####`seasons_remove.py`)</u>

## 2.3 Order the Elements

 - order of elements sometimes need to be changed
 - there are two major ways to sort a list

1. Permanent Sorting
   - `list.sort()`
   - permanently change the order
   - irreversible
   - `list.sort(reverse=True)` to reverse the order
   Example: <u>[`seasons_sort.py`](####`seasons_remove.py`)</u>

2. Temporary Sorting
   - `sorted(list)`
   - temporarily reorder the list
   - can be reversed with `reverse=True` as well
   Example: <u>[`seasons_sorted.py`](####`seasons_remove.py`)</u>
 - There are also two very useful tools for ordering lists

1. Reverse the List
   - `list.reverse()`
   - permanently reverse the order of the list
   - to restore just reverse again
   Example: <u>[`seasons_reverse.py`](####`seasons_remove.py`)</u>
2. Check the Length
   - `len(list)`
   - produces the length of the list provided
   Example: <u>[`seasons_len.py`](####`seasons_remove.py`)</u>
## 2.3 Index Error
 - a common error when manipulating lists is `IndexError: List index out of range`
   - accessing index that does not exist
   - only `index` from `-1 * len(list)` to `len(list) - 1` exist
   Example: <u>[`seasons_error.py`](####`seasons_error.py`)</u>
## 2.5 Sample Code

#### `seasons.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons)
```
__Output:__ 
```
['spring', 'summer', 'autumn', 'winter']
```
#### `seasons_index.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[0])
print("It is now " + seasons[1].title() = ".")
```
__Output:__ 
```
spring
It is now summer.
```
#### `seasons_reverse_index.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[-1])
print(seasons[-2])
```
__Output:__ 
```
winter
autumn
```
#### `seasons_edit.py`
```python
seasons = ["spring", "summer","autumn","winter"]
seasons[2] = "fall"
print(seasons)
```
__Output:__ 
```
['spring', 'summer', 'autumn', 'winter']
```
#### `seasons_add.py`
```python
seasons = ["spring", "autumn"]
seasons.append("winter")
print(seasons)
season.insert(1, "summer")
print(seasons)
```
__Output:__ 
```
['spring', 'fall', 'winter']
['spring', 'summer', 'fall', 'winter']
```

#### `seasons_del.py`
```python
seasons = ["spring", "summer","autumn","winter"]
del seasons[2]
print(seasons)
```
__Output:__ 
```
['spring', 'summer', 'winter']
```

#### `seasons_pop.py`
```python
seasons = ["spring", "summer","autumn","winter"]
seasons.pop(1)
print(seasons)
seasons.pop()
print(seasons)
```
__Output:__ 
```
['spring', 'autumn', 'winter']
['spring', 'autumn']
```

#### `seasons_remove.py`
```python
seasons = ["spring", "summer","autumn","winter"]
szn = "summer"
seasons.remove(szn)
print(seasons)
```
__Output:__ 
```
['spring', 'autumn', 'winter']
```
#### `seasons_sort.py`
```python
seasons = ["spring", "summer","autumn","winter"]
seasons.sort()
print(seasons)
seasons.sort(reverse=True)
print(seasons)
```
__Output:__ 
```
['autumn', 'spring', 'summer', 'winter']
['winter', 'summer', 'spring', 'autumn']
```
#### `seasons_sorted.py`
```python
seasons = ["spring", "summer","autumn","winter"]
print(sorted(seasons))
print(sorted(seasons, reverse=True))
print(seasons)
```
__Output:__ 
```
['autumn', 'spring', 'summer', 'winter']
['winter', 'summer', 'spring', 'autumn']
['spring', 'summer', 'autumn', 'winter']
```
#### `seasons_reverse.py`
```python
seasons = ["spring", "summer","autumn","winter"]
seasons.reverse()
print(seasons)
```
__Output:__ 
```
['winter', 'autumn', 'summer', 'spring']
```
#### `seasons_len.py`
```python
seasons = ["spring", "summer","autumn","winter"]
print(len(seasons))
```
__Output:__ 
```
4
```
#### `seasons_error.py`
```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[4])
print(seasons[-5])
```
__Output:__ 
```
File "<seasons_error>", line 2, in <module>
IndexError: list index out of range
```
## Homework

TBD