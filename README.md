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

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

QUANTIFIERS IN REGULAR EXPRESSIONS: There are different types of qualifiers, which are either defined as a "greedy qualifier" or "lazy qualifier". Below are the various versions that could be seen in regular expressions.  *, +, ?, { n }, { n ,}, { n , m}


For email validation, we use the qualifiers + and {}.


### Character Classes

Character classes allow you to tell the regex engine to match only one out of several characters. This is accomplished by placing the characters you want to match between square brackets.

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

Regular expressions allow us to match text and also to pull information that might be available. This is done by defining groups of characters and capturing them using the special parentheses ( and ) metacharacters. Any subpattern inside a pair of parentheses will be captured as a group. This can be used to extract information like phone numbers or emails.

### Bracket Expressions

A bracket expression is either a matching list expression or a non-matching list expression. It consists of one or more expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions.The <right-square-bracket> ( ']' ) shall lose its special meaning and represent itself in a bracket expression if it occurs first in the list (after an initial <circumflex> ( '^' ), if any). Otherwise, it shall terminate the bracket expression, unless it appears in a collating symbol (such as "[.].]" ) or is the ending <right-square-bracket> for a collating symbol, equivalence class, or character class.

### Greedy and Lazy Match

A greedy match will try to match the longest possible string. The lazy mode of quantifiers is an opposite to the greedy mode. It means: “repeat minimal number of times”. We can enable it by putting a question mark '?' after the quantifier, so that it becomes *? or +? or even ?? for '?'.


### Boundaries

There are three different positions that qualify as word boundaries:

1. Before the first character in the string, if the first character is a word character.
2. After the last character in the string, if the last character is a word character.
3. Between two characters in the string, where one is a word character and the other is not a word character.

### Back-references

https://javascript.info/regexp-introduction

https://www.oreilly.com/library/view/regular-expressions-cookbook/9781449327453/ch04s01.html

https://www.javascripttutorial.net/regular-expression-anchors/

https://www.javascripttutorial.net/regular-expression-anchors/

https://docs.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions

https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap09.html

https://regexone.com/lesson/capturing_groups

https://www.regular-expressions.info/wordboundaries.html

https://medium.com/@318097/greedy-lazy-match-in-regular-expression-35ce8eca4060

### Look-ahead and Look-behind

Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors explained earlier in this tutorial. 

## Author
Hunter Johnson 

Please, contact Hunter Johnson to request any further details or questions at https://github.com/Trayehunter1 . Thank you! 
