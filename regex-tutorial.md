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

- '^(https?:\/\/)?'

- '([\da-z\.-]+)\'

- '([a-z\.]{2,6})'

- '([\/\w \.-]*)*'

Grouping Constructs seperate characters in a RegEx into groups. These characters are grouped inbetween '()'. In this ReGex, there are 4 different groups seen above.

### Bracket Expressions

- '[\da-z\.-]'

- '[a-z\.]'

- '[\/\w \.-]'

Bracket expressions contain the range of characters being searched for in an expression. Within this RegEx, there are 3 bracket expressions seen in order of appearance above. The first, '[\da-z\.-]' includes a lowercase a-z, a '.', and a '-'. Next, '[a-z\.]' will include a lowercase a-z and a '.'. Last, '[\/\w \.-]' has a '/', any character 'a-z, A-Z, 0-9' a '.' and a '-'.

### Character Classes

- '[\da-z\.-]'

- '[\/\w \.-]'

Character classes define a set of characters that can occur within a string in a regular expression. '/d' defines any digit '0-9' and is used in the first bracket expression '[\da-z\.-]. '/w' defines any word character 'a-z, A-Z, 0-9' and is used in the second bracket expression '[\/\w \.-]'.

### Flags

- '//'

The regex is enclosed by two / characters with no flags. Since multi-line is not enabled (by following the ending / with an m), the anchors match a string instead of the start and end of a line.

### Character Escapes

- '/'

- '.'

Character escapes are characters followed by a `\` to indicate that they are interpreted literally and not part of an expression.  In this RegEx, `.` and `/` are used several times as escaped characters, indicating that they are used literally as a `.` and a `/`.In the first group `(https?:\/\/)`, `/` is used twice at the end literally. In the second group `([\da-z\.-]+)`, `.` is used literally. between the second and the third group, `\.` is included to use a `.` literally. In the third group `([a-z\.]{2,6})`, `.` is used literally. In the fourth group, `([\/\w \.-]*)`, both `/` and `.` are used literally. After the fourth group, a `/` is used literally.

## Author

Jonah Lewis

(GitHub URL) [https://github.com/jonahscottlewis]