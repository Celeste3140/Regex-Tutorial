Regex Tutorial

This is a short tutorial on regular expressions (Regex) as a programming language. This tutorial will explain how this language is used and how it can be read. Along with understanding the language, one will understand how this method can be efficient and flexible. 

## Summary

Regular expressions (Regex) are expressions that use various different kind of symbols the represent charcters or patterns in text. Regex can be used in almost all  programming languages used today and serves as an efficient search tool for programmers. Regex uses literal characters to represent numbers or letters and meta charcters to indicate a patterns such as positions, quantifers and classes.

For example: 
Here is a regular expression that is used to verify an email address:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
Regex expressions are made up of components that are also referred to as atoms. Some of these components include single characters such "()", "?", "+", "$" and "/". Other stype of components include bracket expressions, anchors, control characters and etc. 

### Anchors
Anchors are components that match an empty substring.
"^" and "$" are considered anchors.

* "^" targets string that matches characters in the beginning of string

* "$" targets string that matches characters in the end of string

### Quantifiers
Quantifiers helps regex matches by setting limits to the searches. Quantifiers are greedy so they indicate that the match be maximal. A "?" can be added to the quantifier to make it non-greedy (can also be refered to as lazy) and changes the match to be more minimal. 
Here are some quantifiers: 

* "+" matches 1 or more occurrences of the pattern

* "?" matches 0 or 1 occurrences of the pattern 

* "*" matches 0 or more occurrences of the pattern

{} can also set limits for matches. For example:
* {6} indicates exactly 6 occurrences of the pattern will be match. 
* {6, } indicates that at least 6 occurrences of the pattern will be match.
* {6, 10} indicates between 6 and 10 occurences of the pattern will be match. 

### OR Operator
OR Operators (|) require the string to meet all requirements in the pattern. For example: 

* (123) : (abc) we have this expression that will match each character individually 

* (1|2|3) : (a|b|c) using the or operator this expression will match every character 

### Character Classes
Character classes matches a single character out of several ones. 

* "." matches any single character 

* "\d" matches any numerical digit, same as [0-9]

* "\s" matches any whitespace character 

* "\w" any numerical or alpanumeric character including "_"

### Flags
Flags changes regex searches by changing the default searching behavior. Flags are added at the end of an expression and define how these searches will be changes. 

* "g" - Global: search for all occurances 

* "i" - Ignore Casing: Letter casing is ignored in match

* "s" - Dot All: makes "." character match everything, including newlines

* "m" - Multi-line: makes boundary tokens to match beginning and end of each line instead of string 

* "y" - Sticky: Match starts from position that is specified in its lastIndex

* "u" - Unicode: assumes test string as code points, this flag is used with characters outside normal UTF-16 character set range

### Grouping and Capturing
Grouping and capturing groups matches multiple characters as a single unit, doing so by putting desired group in a set of parentheses. This is useful when we need to match only a portion of the search.

### Bracket Expressions

Bracket Expressions [] represent a series of characters that are going to be match. Any single character inside the bracket expression is matched with the target string.

For example we have this bracket expression [jkl], it will look for a string that includes any of those letters in the bracket expression. 

Another example, we have this bracket expression [3-5], it will search for any number between 3-5. 

### Greedy and Lazy Match
* Greedy searches will search all and every occurances. A negative to this is that a greedy search will result in a large group of results. Greedy searches is usually the default behaviour of regular expression. 

* Lazy Matches outputs a much smaller match group. The matching is repeated until condition is satisfied. Lazy matches can be used by adding "?" at the end of the expression. 

### Boundaries
Boundaries (\b) in regex is an anchor and matches positions for a side or whole word in a string or word character. For example:
\bmat\b would only match the word mat so words such as maths or mates would not work

\bmat with just one boundary in the front, we can match mat in words such as matte or mater

mat\b with the boundary just at the end we can match mat in words such as format or hazmat 

### Back-references
Back-refrences in regex allows one to find repeated occurances of a character in a string. Such as, if we match an occurance in a group we can use back-referencing to match succeeding occurrences in a string. Back-refrences use "\1" to refer back to a previous part of the expression.

### Look-ahead and Look-behind
Look-ahead and look-behind is also referend to as "lookaround". This a specific syntax that matches patterns that are before or not followed by another pattern.

*Look-ahead: 
C(?=B) match for C only if followed by B

*Look-behind:
(?<=B)C match for C only if there's B before

## Author

[GitHub Profile](https://github.com/Celeste3140)
