---
title: Unit 6 - User Input and `while` Loop
permalink: /unit6/
---

## 6.0 - Table of Contents<!-- omit from toc -->

- [6.1 - Principle of Input](#61---principle-of-input)
  - [6.1.1 - Writing Clear Instructions](#611---writing-clear-instructions)
  - [6.1.2 - Getting Integer Input](#612---getting-integer-input)
  - [6.1.3 - Mod Operation](#613---mod-operation)
- [6.2 - `while` Loop Intro](#62---while-loop-intro)
  - [6.2.1 - Using `while` loop](#621---using-while-loop)
  - [6.2.2 - User Chooses Stop](#622---user-chooses-stop)
  - [6.2.3 - Using Flags](#623---using-flags)
  - [6.2.4 - Using `break`](#624---using-break)
  - [6.2.5 - continue](#625---continue)
  - [6.2.6 - Avoid Infinite Loops](#626---avoid-infinite-loops)
- [6.3 - `while` Loops and Lists and Dictionaries](#63---while-loops-and-lists-and-dictionaries)
  - [6.3.1 - Moving Elements Across List](#631---moving-elements-across-list)
  - [6.3.2 - Delete Elements of Certain Value](#632---delete-elements-of-certain-value)
  - [6.3.3 - User Input Fills Dictionary](#633---user-input-fills-dictionary)

## 6.1 - Principle of Input

![img](https://lh3.googleusercontent.com/VaUKTKmgrI_fMgR36qDs7N5gH770bDsQtweeCGkm5AM3gs2Y1f4GVQYjs_hJ4K3fFHO4-xVypq_oFYoRu6RKp58xnGwB6kaRgElwoFWlkScUURCmALCFdzURJjC5cqQDzpcDCjo6lua1ffW51GLp)

- stop the program
- waits for user input
- input as string
- return the string
- `var = input(message)`
- the message to print before asking for input
- wait until `return` or `enter` key press

### 6.1.1 - Writing Clear Instructions

- before asking for an input, always be sure to print out a reminder/message
- clear instruction allows for meaningful input
- to print multiple lines, either use separate `print()` or `\n`

### 6.1.2 - Getting Integer Input

- python converts content into a string
- if want to compare two numbers, but one is user input
- `TypeError` because `str` cannot be compared with `int`
- use `int()` to convert `string` to `int`
- `var1 = int(var2)`

### 6.1.3 - Mod Operation

- mod (`%`) is used to find the remainder of a division
- e.g. `7 % 3 = 1`, `3 % 5 = 3`
- useful to find even or odd
- combined use with integer division to get digits from a num

## 6.2 - `while` Loop Intro

![img](https://lh4.googleusercontent.com/j2eYG_H1-W1_6xXsE__IW6TReJID21cSqB5QpY115ppdm5mve_YvAL0NJExzr0efuAcV33qJdzBoZpwMxYo55s54rwkb9eIwFS4_hX9BeSB1kW1Vgbo_JwNjVGFWd22ZgUKOe2MbEzf6koefUouG)

- for loop repeat for a predetermined number of times
- while loop repeats until the condition are no longer met

### 6.2.1 - Using `while` loop

- `while condition:`
- equivalent to `for` loops in certain cases

### 6.2.2 - User Chooses Stop

- combine while loop with user input

### 6.2.3 - Using Flags

- a flag is a Boolean value
- changes values on certain conditions
- multiple conditions can change the same flag
- used somewhere to change how code runs
- combine with a while loop
- reduces the complexity of code as now only checks one condition

### 6.2.4 - Using `break`

- to exit immediately
- does not execute the rest of the code
- ignore condition
- `break`
- `while True`

### 6.2.5 - continue

- to go back to the header
- ignore the rest of the code
- goes through the conditions
- go past certain cases in the while loop

### 6.2.6 - Avoid Infinite Loops

- every while loop must have a method to stop to prevent an infinite loop
- at least one place that `break` or sets the flag to `False`

## 6.3 - `while` Loops and Lists and Dictionaries

- to store the input somewhere
- list
- dictionary
- for loop is efficient in traversing
- while loop can handle edits while traversing

### 6.3.1 - Moving Elements Across List

- move everything into one list
- while the list is not empty, move elements out

### 6.3.2 - Delete Elements of Certain Value

- a repeatedly occurring value needs to be removed
- while this element still exists, remove an instance of it

### 6.3.3 - User Input Fills Dictionary

- Poll
- repeat until the flag is `False`
- get two inputs per round
- ask if the user want to continue
