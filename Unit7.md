---
title: Unit 7 Functions
permalink: /unit7/
---

## 7.0 - Table of Contents<!-- omit from toc -->

- [7.1 - Define Function](#71---define-function)
  - [7.1.1 - Local Variables](#711---local-variables)
  - [7.1.2 - Pass Info to Function](#712---pass-info-to-function)
  - [7.1.3 - Paramter vs Argument](#713---paramter-vs-argument)
- [7.2 - Pass in Arguments](#72---pass-in-arguments)
  - [7.2.1 - Positional Argument](#721---positional-argument)
  - [7.2.2 - Keyword Argument](#722---keyword-argument)
  - [7.2.3 - Default Value](#723---default-value)
  - [7.2.4 - Mixing Arugment Types](#724---mixing-arugment-types)
  - [7.2.5 - Avoid Argument Errors](#725---avoid-argument-errors)
- [7.3 - Return](#73---return)
  - [7.3.1 - Simple Return](#731---simple-return)
  - [7.3.2 - Multiple Returns](#732---multiple-returns)
- [7.4 - Pass in List](#74---pass-in-list)
  - [7.4.1 - Edit List in Function](#741---edit-list-in-function)
  - [7.4.2 - Stop Permanent Edits](#742---stop-permanent-edits)
  - [7.5 - Any number of Positional Arguments](#75---any-number-of-positional-arguments)
  - [7.5.1 - Combine with Positional Arguments](#751---combine-with-positional-arguments)
  - [7.5.2 - Any number of Keyword Arguments](#752---any-number-of-keyword-arguments)
- [7.6 - Store Function in Module](#76---store-function-in-module)
  - [7.6.1 - Import Entire Module](#761---import-entire-module)
  - [7.6.2 - Import Specific Function](#762---import-specific-function)
  - [7.6.3 - Rename](#763---rename)
  - [7.6.4 - Import all](#764---import-all)
- [7.7 - Formatting Guide](#77---formatting-guide)

![img](assets/0q3DaCuR2zlbh4RmdqVgQ-LaemxkBTjxKPu75tBSCjJ4eoHZzqZOzRzAzKPKYYHFVoIp4mDAWVzedzMEwZBAVZubm11TEp4XgX1sYeGTvy5FDVAqeEbnHciR9-4_MapBLB-k5x4XkvrfEGgs1hPn.png)

## 7.1 - Define Function

- `def`
- function name
- parameters
- `:`
- body of the function
- call function with function name and the needed parameters

### 7.1.1 - Local Variables

- variables in function only exist in function
- main code can't access the local variables
- the local variables are removed after functions runs

### 7.1.2 - Pass Info to Function

- all variables can be a parameter
- must be passed if specified
- can only pass the asked amount of parameter

### 7.1.3 - Paramter vs Argument

- `parameter` is the placeholder that recieves the data
- `argument` is the actual data passed into a `parameter`.

## 7.2 - Pass in Arguments

- a function can be defined with multiple paramters
- can accept multiple arguments
- positional argument
- keyword argument

### 7.2.1 - Positional Argument

- order is very important
- the order of the paramter defines the order or arguments
- corresponding order
- infinite number of positional arguments
- might mismatch when position is incorrect

### 7.2.2 - Keyword Argument

- send arugments by specifying the parameter
- order doesn't matter
- points out purpose of each argument

### 7.2.3 - Default Value

- can define parameter with a default value
- when argument for a parameter is not specified, function uses default value
- avoid error
- shorter function call
- points out conventional uses

### 7.2.4 - Mixing Arugment Types

- you can define a function with a mixture of the different types of paramter
- parameters with default value have to come after the paramters without to avoid confusion

### 7.2.5 - Avoid Argument Errors

- when the number of parameters reqired and the number of arguments dont match
- `TypeError`
- points out the required arguments

## 7.3 - Return

- not all function prints out something
- process data and then send it back
- the data sent back from the function is called `return value`
- this makes the main code simpler to read
- `return variable`
- return any type of data
- return statements marks the end of the code
- anything after return will not be ran

### 7.3.1 - Simple Return

- one return at the end
- functions exits at return
- anything after return is ignored

### 7.3.2 - Multiple Returns

- multiple returns in the code for different conditions
- can return different content
- only 1 return will execute
- everything else will be ignored and function exist on that return

## 7.4 - Pass in List

- sometimes passing in a list will increase efficiency
- function can directly access those data

### 7.4.1 - Edit List in Function

- you can edit the list just like in the main code
- all edits are permanent
- list variables are pointers to the list
- don't need to return the edited list

### 7.4.2 - Stop Permanent Edits

- use slicing to avoid permanent edits to the list
- pass in the argument list with `[:]`
- a copy of the original data instead of just a pointer

### 7.5 - Any number of Positional Arguments

- accept individual arguments as an entire list
- use `*variable`
- accepts all excess arguments
- always placed at the end
- only 1 of this can exist in a function
- creates a list

### 7.5.1 - Combine with Positional Arguments

- all parameter that accepts a single argument must be placed at beginning

### 7.5.2 - Any number of Keyword Arguments

- creates a dictionary
- key as the keyword
- value as the argument
- `**variable`
- similar to `*varaible`

## 7.6 - Store Function in Module

- seperate function into a package
- seperate file
- `import filename`
- hides trivial details
- highlights the main logic of code
- shorter
- easier to read

### 7.6.1 - Import Entire Module

- `import filename`
- `filename.functionmname()`
- use `.` to show location

### 7.6.2 - Import Specific Function

- `from filename import functionname`
- `functionname()`
- no need for `.` as the function itself is imported

### 7.6.3 - Rename

- rename module to shorten the length
- avoid collision
- keyword `as`
- `from module import function as alias`
- `import module as alias`

### 7.6.4 - Import all

- to import all functions in a module and avoid using `.`
- `*`
- `from module import *`
- large modules might slow down the program
- might collide with functions of the same name in the main code

## 7.7 - Formatting Guide

- name everything to a short yet descriptive name
- use space to separate functions
- all imports should be at the beginning
