# URL Regex Tutorial

* Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

## Summary

A regular expression is defined as a string representing a pattern used for matching some portion(s) of a target string. Regular expressions are very general and as a consequence, very complex with many different types of operations represented as special characters, or meta-characters. For example a regular expression can be used to verify an e-mail by checking each character of a string to see if there are any which don't belong and therefore concluding that the string is not an e-mail. The regular expression that I will be discussing here is used to verify URLs.


## Table of Contents

- [Regex Components](#regex-components)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

- '^'

- '$'

Anchors are used inorder to mark the beggining and the end of the expression. In the case of this regex, the carrot symbol, '^' marking the beggining of the statement and the dollar sign '$', marking the end of the expression. 

### Quantifiers

- '?'

- (*)

- (+)

- {2,6}

Quantifiers are used to identify the amount of time an expression will be identified. The question mark '?' indicates that the previous character will occur once optionally. '(https?:\/\/)?' contains two question marks '?'. The first instance of a question mark '?' is in reference to the 's' meaning that a URL can begin with either 'http' or 'https'. the second question mark '?' which comes after all of the characters in the parentheses '()' indicates that a URL can begin with neither. i.e. 'www'. 


### Grouping Constructs

- '(https?:\/\/)?'

### Bracket Expressions

- '[a-z\.]'

### Character Classes

- '[\da-z\.-]+'

- '[\/\w \.-]'


### The OR Operator

- '[]'

### Flags

- 

### Character Escapes

## Author

Jonah Lewis

(GitHub URL) [https://github.com/jonahscottlewis]