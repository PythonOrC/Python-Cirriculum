---
title: Unit 2 - Intro to List
permalink: /unit2/
---

## 2.0 - Table of Contents<!-- omit from toc -->

- [2.1 - What Is a List](#21---what-is-a-list)
  - [2.1.1 - Access Elements in List](#211---access-elements-in-list)
- [2.2 Add, Edit, Remove Elements](#22-add-edit-remove-elements)
  - [2.2.1 Edit an Element](#221-edit-an-element)
  - [2.2.2 Add an Element](#222-add-an-element)
  - [2.2.3 Remove an Element](#223-remove-an-element)
- [2.3 Order the Elements](#23-order-the-elements)
- [2.4 Index Error](#24-index-error)
- [2.5 Sample Code](#25-sample-code)
  - [`seasons.py`](#seasonspy)
  - [`seasons_index.py`](#seasons_indexpy)
  - [`seasons_reverse_index.py`](#seasons_reverse_indexpy)
    - [`seasons_edit.py`](#seasons_editpy)
    - [`seasons_add.py`](#seasons_addpy)
    - [`seasons_del.py`](#seasons_delpy)
    - [`seasons_pop.py`](#seasons_poppy)
    - [`seasons_remove.py`](#seasons_removepy)
    - [`seasons_sort.py`](#seasons_sortpy)
    - [`seasons_sorted.py`](#seasons_sortedpy)
    - [`seasons_reverse.py`](#seasons_reversepy)
    - [`seasons_len.py`](#seasons_lenpy)
    - [`seasons_error.py`](#seasons_errorpy)
- [Homework](#homework)

## 2.1 - What Is a List

- A series of elements arranged in a certain order
- can store (basically) an infinite number of data
- data stored inside can be of different data types
- represented with `[]` and the elements are separated with `,`

Example: [`seasons.py`](#seasonspy)

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
    Example: [`seasons_index.py`](#seasons_indexpy)
- negative index will count elements backwards
  Example: [`seasons_reverse_index.py`](#seasons_reverse_indexpy)

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
    Example: [`seasons_edit.py`](#seasons_editpy)

### 2.2.2 Add an Element

- There are two major ways to add values to a list

1. Add to the end
   - `list.append(value)`
2. Add to the middle
   - `list.insert(index, value)`
   - all values after will increase `index` by `1`
     Example: [`seasons_add.py`](#seasons_addpy)

### 2.2.3 Remove an Element

- There are three ways to delete a value, each with their use cases

1. `del`
   - `del list[index]`
   - used when knowing the index
     Example: [`seasons_del.py`](#seasons_delpy)
2. `pop()`
   - `list.pop()` or `list.pop(index)`
   - used when the value is needed for operations
     Example: [`seasons_pop.py`](#seasons_poppy)
3. `remove()`
   - `lis.remove(element)`
   - used when knowing the value of the element
     Example: [`seasons_remove.py`](#seasons_removepy)

## 2.3 Order the Elements

- order of elements sometimes need to be changed
- there are two major ways to sort a list

1. Permanent Sorting

   - `list.sort()`
   - permanently change the order
   - irreversible
   - `list.sort(reverse=True)` to reverse the order
     Example: [`seasons_sort.py`](#seasons_removepy)

2. Temporary Sorting
   - `sorted(list)`
   - temporarily reorder the list
   - can be reversed with `reverse=True` as well
     Example: [`seasons_sorted.py`](#seasons_removepy)

- There are also two very useful tools for ordering lists

1. Reverse the List
   - `list.reverse()`
   - permanently reverse the order of the list
   - to restore just reverse again
     Example: [`seasons_reverse.py`](#seasons_removepy)
2. Check the Length
   - `len(list)`
   - produces the length of the list provided
     Example: [`seasons_len.py`](#seasons_removepy)

## 2.4 Index Error

- a common error when manipulating lists is `IndexError: List index out of range`
  - accessing index that does not exist
  - only `index` from `-1 * len(list)` to `len(list) - 1` exist
    Example: [`seasons_error.py`](#seasons_errorpy)

## 2.5 Sample Code

### `seasons.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons)
```

**Output:**

```text
['spring', 'summer', 'autumn', 'winter']
```

### `seasons_index.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[0])
print("It is now " + seasons[1].title() = ".")
```

**Output:**

```text
spring
It is now summer.
```

### `seasons_reverse_index.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[-1])
print(seasons[-2])
```

**Output:**

```text
winter
autumn
```

#### `seasons_edit.py`

```python
seasons = ["spring", "summer","autumn","winter"]
seasons[2] = "fall"
print(seasons)
```

**Output:**

```text
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

**Output:**

```text
['spring', 'fall', 'winter']
['spring', 'summer', 'fall', 'winter']
```

#### `seasons_del.py`

```python
seasons = ["spring", "summer","autumn","winter"]
del seasons[2]
print(seasons)
```

**Output:**

```text
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

**Output:**

```text
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

**Output:**

```text
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

**Output:**

```text
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

**Output:**

```text
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

**Output:**

```text
['winter', 'autumn', 'summer', 'spring']
```

#### `seasons_len.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(len(seasons))
```

**Output:**

```text
4
```

#### `seasons_error.py`

```python
seasons = ["spring", "summer","autumn","winter"]
print(seasons[4])
print(seasons[-5])
```

**Output:**

```text
File "<seasons_error>", line 2, in <module>
IndexError: list index out of range
```

## Homework

TBD
