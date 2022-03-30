# Email Regex Tutorial

According to MDN Web Docs, regex or regular expressions are patterns used to match character combinations in strings. Regex is used to define search patterns with symbols to find matches within strings. Regex is not limited to javaScript as it spans from software engineering to data science and beyond.


## Summary

The regex I will be describing is matching an email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
For this tutorial I will be explaining how to understand a Regular Expression

and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
- The email regex contains `+` which is one of the quantifiers that regular expressions use to generate matching possibilities and specifications.

    - `+` indicates one or more occurrences of the preceding element. For example, ab+c matches "abc", "abbc", "abbbc", and so on, but not "ac".

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
