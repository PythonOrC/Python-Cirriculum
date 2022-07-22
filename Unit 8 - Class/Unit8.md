# Unit 8 - Class
## 8.0 - Tables of Contents
[TOC]

![img](assets/AG5ZnWT42VK1J6wk8S957s3fAeQMtBl-zrcLQSQWFzMAhFPKNBVfUb7BGgTISOCimeP3AVpJn0egxugwuUQUkYW78STtlZ8gcj0DkZbklR9b7N9wBijHXWz2dthF3OQtIV1Zm1XirV2-hr33UPgO.png)

## 8.1 - Create and Use Class

 - By using class you can simulate almost everything
 - a class is a template
 - it stores the general structure of something

### 8.1.1 - Create Class
 - `class class_name():`
 - everything is defined by functions
 - functions must include `self` as the first parameter
 - `class_name` must be titled
 - `__init__()`
 - automatically called when a class is created
 - `self.`

### 8.1.2 - Instantiate Class
 - class is a general structure
 - `object` is a specific example of a class
 - it contains specific data
 - `obj = Class(param)`
 - attributes
   - use `object.attribute` to access an attribute
   - it shows that this attribute belongs to the object
 - functions
   - to call functions that belong to the class
   - `.`
   - `object.function()`
 - infinite number of instances can be created with one class
 - all data stored in that instance only appears in that instance (scope)
## 8.2 - Use Class and Object
 - OOP (Object Oriented Programming)
 - class is very commonly used
 - after instantiating a class, you will also need to modify attributes to the class
### 8.2.1 - Default Value for Attributes
 - not all attributes must be a parameter
 - some don't need an argument for values
 - defined in `__init__()`

### 8.2.2 - Default Values for Parameters
 - just like normal functions, you can have param with default values

### 8.3.2 - Edit Value of Attribute
 - there are three ways to edit a value
 - edit the attribute directly
 - use a function
 - offset the value
 1. Edit the Value
   - simple edit the attribute as how you would edit normal variables
   - `obj.attr = val`
 2. Edit with a Method
   - usually called an "update method"
   - changes the value with a function
   - it is sometimes a safer way to update
   - more functionality to just edit
 3. offset value
   - you can offset the values by adding a value to the attribute
   - useful when you don't know the original data
   - don't care about the original data
   - difference is all that matters
## 8.3 - Inheritance
 - Writing a class doesn’t always have to start blank
 - write a variation or special version of a preexisting class
 - by inheriting a class, the child class contains everything the parent class has.
 - a child class can then define and alter the original structure
### 8.3.1 - `__init__()` for child class
 - the parent class must be accessible
 - must be in front of child class
 - child class must indicate the parent class
 - `super().`
 - anything in the parent class can be called with `super()`

### 8.3.2 - Add New Functions
 - to add a new function that the parent class doesn't have, simply define it in the child class
 - this only belongs to the child class
 - parent class can't see these newly defined functions

### 8.3.3 - Overwrite Parent Functions
 - the function has the same name as the one in the parent class
 - use `super()` to reuse the code in the parent class and then write under it to add new features


### 8.3.4 - Instance as Attribute
 - a feature of the class gets too complicated
 - create an individual class
 - save an instance with an attribute
 - piecing pieces together just like the real world
 - it is a better representation of the real-world object

## 9.4 - Import Class
 - keep the main code file clean
 - separate classes into files according to functionality

### 9.4.1 - import single class
 - always write a comment on what the code does on the first line
 - `from file_name import Class_name`
 - then use it just like normal
 - `Class_name.function()`

### import Multiple Classes

 - when certain classes are closely related, they might be stored in the same file
 - each file can store an infinite number of classes
 - separate classes from the same file with a comma (`,`)
 - `from module import Class1, Class2`

### 9.4.2 - Import the entire module

 - to import everything in a module
 - `module.class` to access class
 - `module.class.function()`


### 9.4.3 - Import Every Class
 - to import every class in a module
 - `from module import *`
 - `*` represents everything

### 9.4.4 - Chain Imports
 - the module imported can also import other modules
 - don't need to import the modules used in other modules

## 9.5 - Standard Library
 - python has a set of standard functions and classes
 - e.g. `OrderedDict`
 - `orderedDict` functions just like a dictionary
 - it also stores the order of the key-value pairs being added

## 9.6 - Class Code Style
 - class names are conventionally named with "camel case"
 - camel case means that the first letter of every word is capitalized
 - there are no spaces or underscores present in the name
 - instance names are all lowercase with each word separated with an underscore
