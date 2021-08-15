# Email Validation: Regex for Dummies

The following tutorial is meant to help guide you into Regular Expressions. In JavaScript, regular expression are patturns used to match character combinations in strings. Several components define the building blocks to which we'll break down and evaluate in greater detail.

## Summary

Today I'll be walking through an indepth description and tutorial of regular expressions (RegEx), specifically we'll be creating an email regex. The following regular expression below is used to verify the validation of email address inputs that are submitted by the user. 

Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

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
- [Back-references](#back-references)-
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

We'll begin by discussing anchors, which are used to match a position before or after characters.

Use the ^ anchor to match the beginning of the text.
Use the $ anchor to match the end of the text.
Use the m flag to enable the multiline mode that instructs the ^ and $ anchors to match the beginning and end of the text as well as the beginning and end of the line.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. The following table lists the quantifiers supported by .NET.

QUANTIFIERS IN REGULAR EXPRESSIONS: There are different types of qualifiers, which are either defined as a "greedy qualifier" or "lazy qualifier". Below are the various versions that could be seen in regular expressions.  

*
+ 
?
{ n }
{ n ,}
{ n , m}


For email validation, we use the qualifiers + and {}.


### Character Classes

Character class allow you to tell the regex engine to match only one out of several characters. Simply place the characters you want to match between square brackets.

Example: Character Classes
‹[A-Z0-9.-]› 

‹[A-Z0-9_!#$%&'*+/=?`{|}~^.-]›
 
### Flags

Flags are used to alert specific sequences in regression expressions.

Flag Types: 

i - With this flag the search is case-insensitive: no difference between A and a.
g - With this flag the search looks for all matches, without it only the first match is returned.
m - Multiline mode
s - Enables “dotall” mode, that allows a dot . to match newline character \n
u - Enables full Unicode support
y - “Sticky” mode: searching at the exact position in the text

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

https://javascript.info/regexp-introduction

https://www.oreilly.com/library/view/regular-expressions-cookbook/9781449327453/ch04s01.html

https://www.javascripttutorial.net/regular-expression-anchors/

https://www.javascripttutorial.net/regular-expression-anchors/

https://docs.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions

### Look-ahead and Look-behind

Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors explained earlier in this tutorial. 

## Author
Hunter Johnson 

Please, contact Hunter Johnson to request any further details or questions at https://github.com/Trayehunter1 . Thank you! 
