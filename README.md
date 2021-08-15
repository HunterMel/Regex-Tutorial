
Email Validation: Regex for Dummies

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

QUANTIFIERS IN REGULAR EXPRESSIONS
Greedy quantifier	Lazy quantifier	Description
*	*?	Match zero or more times.
+	+?	Match one or more times.
?	??	Match zero or one time.
{ n }	{ n }?	Match exactly n times.
{ n ,}	{ n ,}?	Match at least n times.
{ n , m }	{ n , m }?	Match from n to m times.

For email validation, we use the qualifiers + and {}.
### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author
Hunter Johnson 

Please, contact Hunter Johnson to request any further details or questions at https://github.com/Trayehunter1 . Thank you! 
