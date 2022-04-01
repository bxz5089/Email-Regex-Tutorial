# Email Regex Tutorial

According to MDN Web Docs, regex or regular expressions are patterns used to match character combinations in strings. Regex is used to define search patterns with symbols to find matches within strings. Regex is not limited to javaScript as it spans from software engineering to data science and beyond.


## Summary

The regex I will be describing is matching an email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
For this tutorial I will be explaining how to understand a Regular Expression for matching an email. 


## Table of Contents

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
- These two anchors can be seem in the email regex:

    - `^` matches at the beginning of the target string, showing the beginning of the line of data.
    
    - `$` matches at the end of the target string, showing the end of the line of data.

### Quantifiers
- The email regex contains `+` and `{}` which are quantifiers that regular expressions use to generate matching possibilities and specifications.

    - `+` matches the pattern one or more times. For example, ab+c matches "abc", "abbc", "abbbc", and so on, but not "ac".

    - `{2,6}` matches the pattern from a minimum of 2 times to a maximum of 6 times.

- Other quantifiers includes `*` whichi matches the pattern zero or more times and `?` that matches the pattern zero or one time.


### Grouping Constructs

- In the email regex example, there are three groups sections enclosed in round brackets; `([a-z0-9_\.-]+)`, `([\da-z\.-]+)`, and `([a-z\.]{2,6})`. Grouping the regex makes it easier to read and understand. Its main use is to unify strings so that it is matched in a complete block.

### Bracket Expressions

- Bracket Expressions are characters enclosed by a bracket `[]`. The brackets indicate a set of characters to match. Any individual character between the brackets will match, and a hyphen can be used to define a set.

    - For example, `[a-z0-9_\.-]` include two sets of characters to match (case sensitive), letters a to z, and number 0 to 9. So the front portion of the email can match any lowercase letter or digit, plus characters `_`, `.`, and `-`.

    - [\da-z\.-] matches any digit characters, indecated by `\d`, lowercase letter a to z, `.`, and `-`.
    
    - [a-z\.] matches a to z lowercase letter and `.`. 

### Character Classes

- `\d` corresponds to a digit: a character from 0 to 9.

    - `\d` used in the email regex mean its looking for a matches to any digit characters

- `\s` corresponds to a whitespace character: includes spaces.

- `\w` corresponds to a word character: either a letter of the Latin alphabet or a digit or an underscore.

- `.` corresponds to any character except the newline character (\n)

### The OR Operator

- `|` is the OR operator, it matches characters or expression of either the left or right of the OR operator. This email regex does not use any OR Operator. 

### Flags

- A flag is an optional parameter to a regex that modifies its behavior of searching. This email regex does not use any flags. 

    - One example would be `g`, which makes the expression search for all occurrences.



### Character Escapes

- `\` escapes a character from being interpreted literally. In this email regex, `\.` was used to escape `.` so it can match with a period character. 

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
