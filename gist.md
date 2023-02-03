# Regex for Dummies

Hello Dummy! This is a tutorial to make you not a dummy on the subject of regex.

## Summary

Regular Expression or regex is used for finding patterns in a string. It has two main use cases; to validate text, and search through text. Regex start and end with forward slashes / /, and you would type the string you are looking for in between those forward slashes. The following is an example.

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

    A regex would typically look like the following  " /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ " and is a string saved as a hex value. The following sections will be a break down of the components.

### Anchors

    Anchors are used to match a character in a position of a string.

    Caret anchor "^": Match beginning of string.

    Dollar anchor "$": Match end of string.

### Quantifiers

    Quantifiers are used to dictate how many times a pattern is allowed to occur. A question mark "?" allows for 0-1, asterisk "*" allows for 0 or multiple times, and plus sign "+" allows for 1 or more. Braces "{}" allow the enclosed to set an exact value or min max value, as an example {2,6}.

### Grouping Constructs

    Parenthesis "()" are used to for grouping constructs together. With this the enclosed expression is separated from what is outside the parenthesis, allowing for capturing of substrings.

### Bracket Expressions

    Backets "[]" the enclosed defines its own characters sets, for example [A-Z]. Adding a caret "^" to the front excludes the enclosed.

### Character Classes

    Examples backslash d "\d" or backslash "\w", and is used to distinguish between kinds of characters such as numeric digits and letters respectively for the previously shown. Capital letters indicater that is not searching.

### The OR Operator

    The OR operator is the "|" special character. It is used to find one or the another string but not all at once.

### Flags

    Changes the default search behavior of a regex. There are 6 g,i,m,u,s,y.

    g = global: Makes the expression search for all occurrences.

    i = ignore casing: Makes the expression search case-insensitively.

    m = multiline: Makes the boundary characters ^ and $ match the beginning and ending of      every single line instead of the beginning and ending of the whole string.

    u = unicode: Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

    s = dot all: Makes the wild character . match newlines as well

    y = sticky: Makes the expression start its searching from the index indicated in its lastIndex property.

### Character Escapes

    Backslash "\" allow for special characters to be entered into the string for seraching.

## Author

    Author: Derrick Harris
    Github:https://github.com/takubmf
    Email: https://takubmf@gmail.com