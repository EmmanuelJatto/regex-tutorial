# Regex Tutorial

Regular expressions, also known as regex, are a series/sequence of special characters that defines a pattern in a text string.  It can be used to match, locate, and manage text.

## Summary

The regex I will be describing is the regular expression for Matching An Email.  
Code snippet: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This tutorial will explain how this string applies to matching an email. 

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
A regex is a literal so the pattern has to be wrapped in a slash character. 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
### Anchors
The anchors in this regular expression are ^ and $.  The ^ anchor signifies a string that begins with characters that follow it.  The $ anchor signifies the end of the string
### Quantifiers
The quantifiers in this regular expression are {2,6} and the + operator.  The {2,6} in this expression limits the match range to 2-6 characters for the last character set of [a-z\.].  The + operator connects the separate character sets.  So in this example the the email name ([a-z0-9_\.-]) will be connected to the @, then connected to email service ([\da-z\.-]), then it connects to the top level domain ([a-z\.]{2,6}).
### Grouping Constructs
You group regex expressions by using a parentheses ().  Every section in the parentheses is called a subexpression. ([a-z0-9_\.-]+) This is the first group in the Matching An Email Regex. 
### Bracket Expressions
Whatever is inside a set of square brackets are known as a bracket expression.  Bracket expressions represent a range of characters that we want to match.  
The first bracket expression in Matching An Email is [a-z0-9_\.-].  The a-z means that the string can contain any lowercase letter between a-z.  0-9 means that the string can contain any number between 0-9.  [_\.-] means that that the expression can contain underscore, hyphens, slashes, and periods.  
### Character Classes
A character class in a regular expression defines a set of characters.  The character class in this regular expression is \d it will match any numeral digit, specifically in this expression it will be [0-9].
### The OR Operator
An OR operator is represented by two vertical bars ||.  It is typically used outside the bracket expression, between different grouping constructs.  
### Flags
Flags are placed at the end of a regex, after the second slash.  The three most common flags are g, i, and m.  m means multi-line search.  i  ignores case when matching a string.  g is a Global search.
### Character Escapes
The backslash in a regex escapes a character that otherwise be interperted literally.  
## Author

My name is Emmanuel Jatto and I am a software developer.  The coding languages I have experience with are Javascript, HTML, CSS, SQL, NoSQL.  I am also have some limited experience  with Java and C#.  
Github Link: https://github.com/Emmanueljatto

