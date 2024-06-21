# Regex Tutorial

Explaining Regex for email validation. Most websites have some form of email validation for the user sign up itself.

## Summary

I will be summarizing a Regex expression to understand code that explains email validation.

## Regex for Email Validation

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

See below the contents to understanding Regex.

### Anchors

For anchors I use the caret `^` and the dollar sign `$`

- Caret `^` at the begginning of the string means that it is the start of the regex.

- Dollar `$` at the end of the string means that it is the end of the regex.

The purpose of anchors are to guarantee that the whole string complies with email format.

### Quantifiers

There are two quantifiers in the regular expression.

- `+` is being used in the `([a-z0-9_\.-]+)` `([\da-z\.-]+)` part of the Regex meaning that it allows one or more character sets.

- `{2,6}` is being used in the `([a-z\.]{2,6})` part of the Regex to show that only 2-6 chararcters can be used.

### OR Operator

OR operator `|` is being used implicitly in the Regex. It can be applied but in this case isn't.

### Character Classes

Identified three character classes in the Regex

ex. (example@gmail.com)

- `[a-z0-9_\.-]` the username that corresponds to set email
ex. (example)
- `[\da-z\.-]` the domain being used to host the email
ex. (gmail, yahoo, etc.)
- `[a-z\.]` the top level domain being used
ex. (.com, .gov, .edu, etc.)

### Flags

There aren't any flags being used in the Regex.

the flag modifiers are:

- `g modifier` global, or all matches found.
- `m modifier` multiline meaning the anchors `^` and `$` are required.

### Grouping and Capturing

Grouping is the collection of values brought by classes using `()`

- `([a-z0-9_\.-]+)` username
- `([\da-z\.-]+)` domain
- `([a-z\.]{2,6})` top level domain


### Bracket Expressions

Brackets `[]` define a set of characters, or classes, being used. 

- `[a-z0-9_\.-]` username 
- `[\da-z\.-]` domain 
- `[a-z\.]` top level domain 

### Greedy and Lazy Match

There are no greedy or llazy matches being used in the Regex expression.

- `.+` is a greedy mode indicator
- `?` is the lazy mode indicator

### Boundaries

There are no boundaries being used in the Regex Expression

- `\b` is the boundary indicator. In our case only anchor tags are being used.

### Back-references

- https://javascript.info/regexp-anchors

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Quantifiers

- https://support.workiva.com/hc/en-us/articles/4407304269204-Regular-expression-operators

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Character_classes

- https://regex101.com/

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Regular_expressions/Capturing_group

- https://plainenglish.io/blog/regular-expressions-brackets-f2d6f69ffe13

- https://javascript.info/regexp-greedy-and-lazy

- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Regular_expressions/Lookahead_assertion

### Look-ahead and Look-behind

There are no look-aheads or look-behinds being used in the Regex expression.

Look-ahead indicators
- `?=` 
- `?!`

Look-behind indicators
- `?<=`
- `?<!`
## Author

Tristan Magee

UCF Bootcamp student from FLorida working to become a web developer.

GitHub: SaltyCowrie

https://github.com/SaltyCowrie