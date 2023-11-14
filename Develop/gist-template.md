# Regex Tutorial - Computer Science for Javascript
 A brief Regular Expression (Regex) tutorial for matching an email

## Summary

This tutorial is going to explain the use of regex to match emails using the common expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. This expression can be used to ensure an email's validity.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
Anchors match a position within a string. In our case and the regex  /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ , the ^ and $ characters are our anchors, indicating both the starting position and the ending position. 

### Quantifiers
Quantifiers indicate that the preceding token must be matched a certain number of times. By default, quantifiers are greedy and will match as many characters as possible.

    Our Regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

    Quantifiers used: + , {2,6} 

The + operator matches 1 or more of the preceding item, and the {2,6} in this case will allow a match range of 2-6 characters for the character set of [a-z\.].

### Character Classes
The character class in the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is \d. This matches any digit character between 0-9.

### Grouping and Capturing
There are 3 capturing groups in this expression. The first is ([a-z0-9_\.-]+) , which matches the email name. ([\da-z\.-]+) matches the email service while ([a-z\.]{2,6}) captures the .com .

### Bracket Expressions
A bracket Expression encloses a list of character classes within square brackets. Examples of this in our regex are [a-z0-9_\.-], [\da-z\.-], [a-z\.].

### Greedy and Lazy Match
Greedy Matching will attempt to match anything it can. Lazy matching will match as few characters as possible. 

## Author

This tutorial was written by Tommy Merniez, a student of the Edx Full Stack Web Development Bootcamp provided through the University of Utah. Github: https://github.com/merniez10

