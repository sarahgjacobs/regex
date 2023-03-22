# Regex Explained

## Summary

This summary of Regex will explain the different components of regex and how to use each. This is the regex expression we will use as our example: /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

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

### Anchors
An Anchor expression is everything included between the opening caret (^) and the closing dollar sign ($).

### Quantifiers
Quantifies define the parameters of the regex, so here the numbers 2 and 6 are specifying there should be a minimum of 2 characters and maximum of 6. In addition, the + symbol is used as a quanitfier.


### OR Operator
The OR symbol is represented with these symbols: ||

There is no OR operator in this regex.

### Character Classes
Character classes are defined charcater sets within regex. In the example regex, \d is used which represents a match of digits between 0 and 9. Other classes include but are not limited to \s and \t. 

### Flags
Flags define parameters when searching. This regex example does not have any flags. Some common flags are i (ignore capitalization) or g (sesarch all occurances)

### Grouping and Capturing
Grouping is achieved through the use of paranthesis and splits necessary portions of the expression. Our expression has three sections:

([a-z0-9_.-]+) user's email

([\da-z.-]+) email provider

([a-z.]{2,6}) domain name

### Bracket Expressions
Brackets expressions indicate parameters to meet, either letters or numbers, and will define the parameters. Our expression has parameters of anything a to z or 0 to 9.

### Greedy and Lazy Match
/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/
A greedy quantifier is shown as + and {}. A lazy quantifier is shown as +? and {}?. Our expression only has greedy quantifiers which will search for all matches whereas lazy quantifiers will only search for the shortest match. 

### Boundaries
Boundaries are denoted by \b and are not present in this example.

### Back-references
Back-references research previously matched groups. They use a backslash and a single digit and are not present in this example.

### Look-ahead and Look-behind
These functions define parameters where the match should include a component that comes before or behind another. Exmaples include: X(?=Y) 

This is not used in the given example.

## Author

[Sarah Jacobs](https://github.com/sarahgjacobs)
