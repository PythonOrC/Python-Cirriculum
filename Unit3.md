---
title: Unit 3 - List Manipulation
permalink: /unit3/
---

## 3.0 - Table of Contents<!-- omit from toc -->

- [3.1 - List Traversal](#31---list-traversal)
  - [3.1.1 - Dig Deeper](#311---dig-deeper)
- [3.2 - Indentation Error](#32---indentation-error)
  - [3.2.1 - Forgot to Indent](#321---forgot-to-indent)
  - [3.2.2 - Extra Indentation](#322---extra-indentation)
  - [3.2.3 - Missing `:`](#323---missing-)
- [3.3 - Number List](#33---number-list)
  - [3.3.1 - `Range()`](#331---range)
  - [3.3.2 - Number List with `range()`](#332---number-list-with-range)
  - [3.3.3 - Statics](#333---statics)
  - [3.3.4 - List Comprehension](#334---list-comprehension)
- [3.4 - Slicing](#34---slicing)
  - [3.4.1 - Slice](#341---slice)
  - [3.4.2 - Traversing Slice](#342---traversing-slice)
  - [3.4.3 - Copy List](#343---copy-list)
- [3.4 - Tuple](#34---tuple)
  - [3.4.1 - Define Tuple](#341---define-tuple)
  - [3.4.2 - Tuple Traversal](#342---tuple-traversal)
  - [3.4.3 - Edit a Tuple](#343---edit-a-tuple)
- [3.5 - Code Format](#35---code-format)
  - [3.5.1 - Style Guide](#351---style-guide)
- [3.6 - Sample Code](#36---sample-code)
  - [`magicians.py`](#magicianspy)
    - [`magicians_greeting.py`](#magicians_greetingpy)
    - [`no_indent_error.py`](#no_indent_errorpy)
    - [`no_indent_logic.py`](#no_indent_logicpy)
    - [`extra_indent_error.py`](#extra_indent_errorpy)
    - [`extra_indent_logic.py`](#extra_indent_logicpy)
    - [`missing.py`](#missingpy)
    - [`range.py`](#rangepy)
    - [`range_list.py`](#range_listpy)
    - [`even_numbers.py`](#even_numberspy)
    - [`square.py`](#squarepy)
    - [`stats.py`](#statspy)
    - [`list_comprehension.py`](#list_comprehensionpy)
    - [`slice.py`](#slicepy)
    - [`traverse_slice.py`](#traverse_slicepy)
    - [`copy.py`](#copypy)
    - [`define_tuple.py`](#define_tuplepy)
    - [`traverse_tuple.py`](#traverse_tuplepy)
    - [`edit_tuple.py`](#edit_tuplepy)
- [Homework](#homework)

![img](assets/z0lZt2R_90n3Mmkgvgx8ZWHeTkMUo2UL8Qr4zgohwmEfMChyTh_gGPtQxOr6dxKD8mlbFtwT5SkrpUbr4wn184uizUGKwm0Ka3njQzAiV2W86leEvuGAUEnpz_uayAoQ5XtR70VvgEPWwDA_0mhZ.png)

## 3.1 - List Traversal

- Traversal = going through each element
- modify elements the same way
  - e.g. dispaly all titles
- hard-coded is hard to manage
  - need to be changed when length of list changes
- `for` loop can solve this
  - short
  - simple
  - dynamic
    Example: [`magicians.py`](#magicianspy)

### 3.1.1 - Dig Deeper

- loops are one of the most important concepts in coding
- `for` loop will loop through every element in the list, no matter the length
- execute everything in the loop and then move on
- name variables related to the list
  Example: [`magicians_greeting.py`](#magicians_greetingpy)
- In this example, the indented code ran multiple times
- the code not indented only ran once

## 3.2 - Indentation Error

- Indentation is just 4 spaces
- used to interpret relationship between lines
- indentation shows clear code structure
- the most common error with this is `IndentationError`

### 3.2.1 - Forgot to Indent

- code in a `for` loop must be indented
- if not, an `IndentationError` will occur
  Example: [`no_indent_error.py`](#no_indent_errorpy)
- There is another possible bug, but not error
  - forgot to indent extra lines of code
  - no error
  - but a logical bug
    Example: [`no_indent_logic.py`](#no_indent_logicpy)

### 3.2.2 - Extra Indentation

- python wil also point out extra indentations
- also an `IndentationError`
  Example: [`extra_indent_error.py`](#extra_indent_errorpy)
- there might also be extra indentation after a loop
- no error will be returned
- logic bug exist
  Example: [`extra_indent_logic.py`](#extra_indent_logicpy)

### 3.2.3 - Missing `:`

- an `SyntaxError` will be thrown
  Example: [`missing.py`](#missingpy)

## 3.3 - Number List

- managing stats of a character
- monitoring a region

### 3.3.1 - `Range()`

- range can be used to generate a list of numbers
- `range(start, end)`

Example: [`range.py`](#rangepy)

### 3.3.2 - Number List with `range()`

- `list()` can convert the result of `range()` into a list
  Example: [`range_list.py`](#range_listpy)
- `range(start, end, step)`
- the step is the increment
  Example: [`even_numbers.py`](#even_numberspy)
- almost all number list can be generated with `range`
  Example: [`square.py`](#squarepy)

### 3.3.3 - Statics

- find the smallest number
  - `min()`
- find the largest number
  - `max()`
- find the sum of the numbers
  - `sum()`
    Example: [`stats.py`](#statspy)

### 3.3.4 - List Comprehension

- code to generate a list can be shortened to one line with List Comprehension
- comapct
- combines list and for loop

Example: [`list_comprehension.py`](#list_comprehensionpy)

## 3.4 - Slicing

- manage all elements in the list at once

### 3.4.1 - Slice

- specify the beginning, the end, and the step
- with `[]` and `:`
  Example: [`slice.py`](#slicepy)

### 3.4.2 - Traversing Slice

- only visits the elements surrounded by the slice
- use cases
  - top three player
  - multi-page in website
    Example: [`traverse_slice.py`](#traverse_slicepy)

### 3.4.3 - Copy List

- slicing is needed to create a seperate list
- normally list variables are linked
- they are the same list

Example: [`copy.py`](#copypy)

## 3.4 - Tuple

- static
- immutable

### 3.4.1 - Define Tuple

- defined just like list but with `()`
- everything works just as a list
  Example: [`define_tuple.py`](#define_tuplepy)

### 3.4.2 - Tuple Traversal

- identical to lists
- for loop
  Example: [`define_tuple.py`](#traverse_tuplepy)

### 3.4.3 - Edit a Tuple

- only way is to redefine
  Example: [`define_tuple.py`](#edit_tuplepy)

## 3.5 - Code Format

- conventional format
- easy to read
- easy to understand
- followed by professionals

### 3.5.1 - Style Guide

- Python Enhancement Proposals
- PEP8: <https://peps.python.org/>
- indentation should be 4 spaces
- a line of code should be < 80 characters
- empty lines can seperate function of a code

## 3.6 - Sample Code

### `magicians.py`

```python
magicians = ['alice','david','carolina']
for magician in magicians:
  print(magician)
```

**Output:**

```text
alice
david
carolina
```

#### `magicians_greeting.py`

```python
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
  print("Greetings, " + magician + ".")
  print("Welcome.")
print("Welcome, everyone!")
```

**Output:**

```text
Greetings, alice.
Welcome.
Greetings, david.
Welcome.
Greetings, carolina.
Welcome.
Welcome, everyone!
```

#### `no_indent_error.py`

```python
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
print("Greetings, " + magician + ".")
print("Welcome.")
print("Welcome, everyone!")
```

**Output:**

```error
  File "<stdin>", line 3
    print("Greetings, " + magician + ".")
    ^
IndentationError: expected an indented block after 'for' statement on line 2
```

#### `no_indent_logic.py`

```python
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
  print("Greetings, " + magician + ".")
print("Welcome.")
print("Welcome, everyone!")
```

**Output:**

```text
Greetings, alice.
Greetings, david.
Greetings, carolina.
Welcome.
Welcome, everyone!
```

#### `extra_indent_error.py`

```python
  print("Welcome, everyone!")
```

**Output:**

```error
  File "<stdin>", line 1
    print("Welcome, everyone!")
IndentationError: unexpected indent
```

#### `extra_indent_logic.py`

```python
magicians = ['alice', 'david', 'carolina']
for magician in magicians:
  print("Greetings, " + magician + ".")
  print("Welcome.")
  print("Welcome, everyone!")
```

**Output:**

```text
Greetings, alice.
Welcome.
Welcome, everyone!
Greetings, david.
Welcome.
Welcome, everyone!
Greetings, carolina.
Welcome.
Welcome, everyone!
```

#### `missing.py`

```python
magicians = ['alice', 'david', 'carolina']
for magician in magicians
  print("Greetings, " + magician + ".")
  print("Welcome.")
print("Welcome, everyone!")
```

**Output:**

```error
File "<stdin>", line 1
    for magician in magicians
                             ^
SyntaxError: expected ':'
```

#### `range.py`

```python
for i in range(1,5):
  print(i)

for i in range(5):
    print(i)
```

**Output:**

```text
1
2
3
4
0
1
2
3
4
```

#### `range_list.py`

```python
print(list(range(1,6)))
```

**Output:**

```text
[1, 2, 3, 4, 5]
```

#### `even_numbers.py`

```python
print(list(range(0,10,2)))
```

**Output:**

```text
[0, 2, 4, 6, 8]
```

#### `square.py`

```python
numbers = []
for i in range(5):
  numbers.append(i**2)
print(numbers)
```

**Output:**

```text
[0, 1, 4, 16]
```

#### `stats.py`

```python
numbers = [0,1,2,3,4,5,6,7,8,9]
print(min(numbers))
print(max(numbers))
print(sum(numbers))
```

**Output:**

```text
0
8
45
```

#### `list_comprehension.py`

```python
numbers = [i**2 for i in range(11)]
print(numbers)
```

**Output:**

```text
[0, 1, 4, 9, 16, 25, 36, 59, 64, 81, 100]
```

#### `slice.py`

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
print(numbers[0:4])
print(numbers[1:4])
print(numbers[4:])
print(numbers[1:4:2])
print(numbers[-3:])
```

**Output:**

```text
[0, 1, 2, 3]
[1, 2, 3]
[4, 5, 6, 7, 8, 9]
[1, 3]
[7, 8, 9]
```

#### `traverse_slice.py`

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
for i in numbers[:3]:
  print(numbers[i])
```

**Output:**

```text
0
1
2

```

#### `copy.py`

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
digits = numbers
numbers.append(10)
print(digits)
print(numbers)
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
digits = numbers[:]
numbers.append(10)
print(numbers)
print(digits)
```

**Output:**

```text
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

```

#### `define_tuple.py`

```python
dimensions = (1920, 1080)
print(dimensions[0])
print(dimensions[1])
dimensions[0] = 720
dimensions.append(10)
```

**Output:**

```error
1920
1080
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment
```

#### `traverse_tuple.py`

```python
dimensions = (1920, 1080)
for dimension in dimensions:
  print(dimension)
```

**Output:**

```text
1920
1080
```

#### `edit_tuple.py`

```python
dimensions = (1920, 1080)
print(dimensions)
dimensions = (1080, 720)
print(dimensions)
```

**Output:**

```text
(1920, 1080)
(1080, 720)
```

## Homework

TBD
