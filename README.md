Regex Tutorial

This is a short tutorial on regular expressions (Regex) as a programming language. This tutorial will explain how this language is used and how it can be read. Along with understanding the language, one will understand how this method can be efficient and flexible. 

## Summary

Regular expressions (Regex) is an expression that uses various different kind of symbols the represent charcters or patterns in text. Regex can be used in almost all  programming languages used today and serves as an efficient search tool for programmers. Regex uses literal characters to represent numbers or letters and meta charcters to indicate a pattern such as positions, quantifers and classes.

For example: 
Here is an expression that is used to verify an email address:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

. = any character
* = 0 or more

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
Regex expressions are made up of components that are also referred to as atoms. Some of these components include single characters such ()?+$ and / which for example is used to wrap the expression in. Other stype of components include bracket expressions, anchors, control characters and etc. 
### Anchors
Anchors are components that match an empty substring.
^ and $ are considered anchors.

^ targets string that matches characters in the beginning of string

$ targets string that matches characters in the end of string

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

Bracket Expressions [] represent a series of characters that are going to be match. Any single character inside the bracket expression is matched with the target string.

For example we have this bracket expression [jkl], it will look for a string that includes any of those letters in the bracket expression. 

Another example, we have this bracket expression [3-5], it will search for any number between 3-5. 

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

[GitHub Profile](https://github.com/Celeste3140)
