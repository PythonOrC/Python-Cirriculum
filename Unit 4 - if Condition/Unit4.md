# Unit 4 - If Condition

## 4.0 - Table of Contents
[TOC]

![img](assets/ao6O1cnSREPEwCH-FJ47N8MxgcISPfqfgwDE7NYYVUcKP-8YUDdOj28oi7zCDd64VgWtWKbjz1-YhWizINL5IAH48oz6LyObPN24DdI_l7qE6VrdWXcqcsUIzde00AtzlbmG9RI93jXvCRhoWLCk.png)

## 4.1 - Example

 - some code on runs on certain conditions
 - e.g. check if person is over 18

Example: <u>[`if_intro.py`](####`if_intro.py`)</u>

### 4.1.1 - Combine with Traversal
 - this can be combined with list traversal to increase efficiancy of code
Example: <u>[`for_if.py`](####`for_if.py`)</u>

## 4.2 - Conditions
 - the core of an `if` statement is in its conditional statement
 - Code in `if` will only run when the condition is `True`
 - Boolean value
 - if the condition is `False`, the code in `else` will run
 - `else` is optional

### 4.2.1 - Check if Equal
 - to check if two values are the same, use `==` and palce the two values to check on each side. 
 - if the two values are identical then it returns `True` else `False`
 - `=` is define while `==` is comapre
Example: <u>[`double_equal.py`](####`double_equal.py`)</u>
### 4.2.2 - To Check Letter Cases or Not
 - when comapring two strings, they have to be identical in order to return `True`
 - even letter cases
 - to ignore letter cases, unify them with `.lower()`, `.upper()`, or `.title()`
Example: <u>[`letter_cases.py`](####`letter_cases.py`)</u>
### 4.2.3 - Check if Unequal
 - use `!=` to check if they are unequal
 - `!` means `not`
Example: <u>[`not_equal.py`](####`not_equal.py`)</u>

### 4.2.4 - Compare Numbers
 - numbers follows the same rules
 - `True` if the two numbers are the same and `False` if not
 -  `>`, `>=`, `<`, `<=`
Example: <u>[`compare_numbers.py`](####`compare_numbers.py`)</u>

### 4.2.5 - Multiple Conditions
 - sometimes you may want to check multiple conditions
 - `and` and `or` is useful in connecting these conditions

1. `and`
   - To check if both conditions are `True`
   - only `True` if both are `True`
   - if one is `False` then it is `False`
   - Truth Table
     |    `A`    |    `B`    | `A and B` |
     |  :-----:  |  :-----:  |  :-----:  |
     |  `True`   |  `True`   |  `True`   |
     |  `True`   |  `False`  |  `False`  |
     |  `False`  |  `True`   |  `False`  |
     |  `False`  |  `False`  |  `False`  |
     Example: <u>[`and.py`](####`and.py`)</u>
2. `or`
   - To check if any conditions are `True`
   - returns `True` if either one is `True`
   - if both is `False` then it is `False`
   - Truth Table
     |    `A`    |    `B`    | `A and B` |
     |  :-----:  |  :-----:  |  :-----:  |
     |  `True`   |  `True`   |  `True`   |
     |  `True`   |  `False`  |  `True`   |
     |  `False`  |  `True`   |  `True`   |
     |  `False`  |  `False`  |  `False`  |
     Example: <u>[`or.py`](####`or.py`)</u>

### 4.2.6 - Check if Value is in List
 - before certain actions the values of the list need to be checked
 - e.g. before register a user, check if the username already exists
 - use keyword `in` to check if value is in list
Example: <u>[`in.py`](####`in.py`)</u>
### 4.2.7 - Check if Value is not in List
 - it is also important to check if values are not in a list
 - e.g. ban list for a website
 - key `not in` is used
Example: <u>[`not_in.py`](####`not_in.py`)</u>

## 4.3 - `if` Statements
 - there are many types of `if` statements
 - `if`
 - `if-else`
 - `if-elif-else`
 - ...

### 4.3.1 - Simplest `if` strcture
 - one condition and one action
 - first line includes the condition
 - next indented line includes the action
 - the indented line only runs when the `if` statement is `True`
Example: <u>[`if.py`](####`if.py`)</u>

### 4.3.2 - `if-else` strcture
 - two routes depending on the condition
 - `True` runs the code under the `if`
 - `False` runs the code under the `else`
 - "Do A if condition is true, else do B"
Example: <u>[`if-else.py`](####`if-else.py`)</u>

### 4.3.3 - `if-elif-else` strcture
 - multiple possible actions depending on the cases
Example: <u>[`if-elif-else.py`](####`if-elif-else.py`)</u>

## 4.4 - Process List with `if`
 - combining `for` loop and `if` statement can process special elements in a list
 - making sure the code will work in any conditions

### 4.4.1 - Special Element in List
 - sometimes certain values requires special treatment
Example: <u>[`toppings.py`](####`toppings.py`)</u>
### 4.4.2 - Check if List is empty
 - there was an assumption that there is at least one element in list
 - sometimes something special need to be done when list is empty
Example: <u>[`empty.py`](####`empty.py`)</u>


## 4.5 - Formatting Guide
 - to make the code easier to read, a space (` `) is usually added to either side of the condition
 - does not affect how the code runs
 - asthetic choices
 - `a == b`
 - `a==b`
 - 
## 4.6 - Sample Code
#### `if_intro.py`
```python
age = 30
if age >= 18:
	print("adult")
else:
	print("child")
```
__Output:__ 
```
adult
```

#### `for_if.py`
```python
ages = [17, 18, 32, 68, 2, 10]
for age in ages:
	if age >= 18:
		print("adult")
	else:
		print("child")
```
__Output:__ 
```
child
adult
adult
adult
child
child
```

#### `double_equal.py`
```python
name = "Ava":
print(age == "Ava")
print(age == "Ethan")
```
__Output:__ 
```
True
False
```

#### `letter_cases.py`
```python
name = "Ethan Hu"
print(name == 'ethan hu')
print(name.lower() == 'ethan hu')
```
__Output:__ 
```
False
True
```
#### `not_equal.py`
```python
name = "Ethan Hu"
print(name != 'John')
print("John" != 'John')
```
__Output:__ 
```
True
False
```
#### `compare_numbers.py`
```python
age = 18
if age < 18:
	print("not yet adult")
if age == 18:
	print("just turned adult")
if age >= 18:
	print("adult")

```
__Output:__ 
```
just turned adult
adult
```

#### `and.py`
```python
age1 = 18
age2 = 17
print(age1 >= 18 and age2 >= 18)
```
__Output:__ 
```
False
```

#### `or.py`
```python
age1 = 18
age2 = 17
print(age1 >= 18 or age2 >= 18)
```
__Output:__ 
```
True
```

#### `in.py`
```python
name = "Ethan"
invitations = ["Ethan", "Ava", "John", "Bob"]
print(name in invitations)
```
__Output:__ 
```
True
```

#### `not_in.py`
```python
name = "Dillon"
banned = ["Ethan", "Ava", "John", "Bob"]
print(name not in invitations)
```
__Output:__ 
```
True
```

#### `if.py`
```python
if 10 > 9:
	print("10 is larger than 9")
```
__Output:__ 
```
10 is larger than 9
```

#### `if-else.py`
```python
if 9 > 9:
	print("9 is larger than 9")
else:
	print("9 is not larger than 9")
```
__Output:__ 
```
9 is not larger than 9
```

#### `if-elif-else.py`
```python
age = 12
if age < 4:
	print("baby")
elif age < 12:
	print("kid")
elif age < 18:
	print("teenager")
else:
	print("adult")
```
__Output:__ 
```
teenager
```

#### `toppings.py`
```python
requested_toppings = ["mushrooms","green pepper", "olive","extra cheese"]
stock = ["olive", "extra cheese", "pepperoni"]
for topping in requested_toppings:
	if topping in stock:
		print("Adding" + topping)
	else:
		print("We are out of " + topping)
print("Pizza is finished")
```
__Output:__ 
```
We are out of mushrooms
We are out of green pepper
Adding olive
adding extra cheese
Pizza is finished
```

#### `empty.py`
```python
requested_toppings = []
stock = ["olive", "extra cheese", "pepperoni"]
if requested_toppings:
    for topping in requested_toppings:
        if topping in stock:
            print("Adding" + topping)
        else:
            print("We are out of " + topping)
    print("Pizza is finished")
else:
	print("Just a plain pizza?")
```
__Output:__ 
```
Just a plain pizza?
```