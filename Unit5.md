---
title: Unit 5 - Dictionary
permalink: /unit5/
---

## 5.0 - Table of Contents<!-- omit from toc -->

- [5.1 - Simple Dictionary](#51---simple-dictionary)
- [5.2 - Using Dictionary](#52---using-dictionary)
  - [5.2.1 - Access Values](#521---access-values)
  - [5.2.2 - Add Key-Value Pair](#522---add-key-value-pair)
  - [5.2.3 - Empty Dictionary](#523---empty-dictionary)
  - [5.2.4 - Delete Key Value Pair](#524---delete-key-value-pair)
- [5.3 - Dictionary Traversal](#53---dictionary-traversal)
  - [5.3.1 - Traverse all Keys and Values](#531---traverse-all-keys-and-values)
  - [5.3.2 - Traverse all Keys](#532---traverse-all-keys)
  - [5.3.3 - Traverse Sorted Keys](#533---traverse-sorted-keys)
  - [5.3.4 - Traverse Values](#534---traverse-values)
- [6.4 - Nesting](#64---nesting)

![Dictionaries in Python – Real Python](assets/Dictionaries-in-Python_Watermarked.3656a2293c00.jpg)

## 5.1 - Simple Dictionary

- a dictionary is just like a dictionary in real life
- just like a list, a dictionary can store an almost infinite amount of data
- it is a more complicated structure than a list

## 5.2 - Using Dictionary

- a dictionary is a series of key-value pairs.
- every key corresponds to a value
- think of keys as indexes, but can be anything
- think of value as the element stored in the list
- you can access the value with the key
- `{}`, `:`, and `,`
- anything can be the value

### 5.2.1 - Access Values

- specify the dictionary name and the key
- `dictionary[key]`

### 5.2.2 - Add Key-Value Pair

- just define as a variable
- `dictionary[key] = value`
- modifies existing key is key already exist
- order of the key-value pair is different from the order you added them
- python doesn't care about the position of the key-value pair
- only the link between the key and the value matters

### 5.2.3 - Empty Dictionary

- to create an empty dictionary, just define with `{}`
- a repeated code that adds information to a dictionary
- emptying a dictionary
- initializing a dictionary

### 5.2.4 - Delete Key Value Pair

- dictionary name and key name
- `del dictionary[key]`

## 5.3 - Dictionary Traversal

- just like list
- visit all keys, values, or values and keys

### 5.3.1 - Traverse all Keys and Values

- use for loop to traverse dictionary
- `for key, value in dictionaryitems():`
- `.items()` returns a list of key and value

### 5.3.2 - Traverse all Keys

- use function `.keys()` to get all keys
- `.keys()` returns a list of keys
- `for key in dictionary.keys():`
- can be removed
- `for key in dictionary:`
- same functionality
- dictionary returns all keys on default
- `.keys()` makes code more readable

### 5.3.3 - Traverse Sorted Keys

- python returns keys in an unpredictable order
- either sort after gettings all keys or sort before getting the keys
- to sort the keys use `sorted()`
- `for key in sorted(dictionary.keys()):`

### 5.3.4 - Traverse Values

- to only traverse values
- ".values()"
- returns a list of only values and no keys
- `for value in dictionary.values():`
- to filter out repeated values, use `set()`
- for value in `set(dictionary.values()):`
- set is a data type
- like a list but stored only unique values in a sorted order.

## 6.4 - Nesting

- you can store a list or a dictionary in another list or dictionary.
- This is called nesting
- useful in many situations
- list in list
- list in dictionary
- dictionary in list
- dictionary in dictionary
