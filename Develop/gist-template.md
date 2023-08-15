# Regex-Tutorial

Introductory paragraph (replace this with your text)

## Summary

The following line of code /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is a regular expression, basically a pattern thats read to match items. This particular code is used to match emails. 

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
Regular expressions are made of many different parts that work in conjunction to define a search pattern. The most common componenets include anchors, quantifiers, character classes, and character escapes. There are two different ways of writing a regular expression, one way is through using a regular expression literal which consists of a pattern enclosed between slashes. The other way is through calling a constructor function of the RegExp obect. The example from above utilizes a forward slash both at the start and the end making it a regular expression literal. 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors
Anchors match the starting and ending points of a string or line in our example each ^ marks the beginning while the $ means the end of our line. 

### Quantifiers
Quantifiers allow the user to dictate how many of a character or character class should be matched. One example of a quantifier is + to match one or more occurances of the preceeding character or character class. This particular symbol is found in our example doing just that.  


### Grouping Constructs
Grouping is used to make a section of the expression to work as one. By placing part of a regular expression inside round brackets or parentheses, you can group that part of the regular expression together. This allows you to apply a quantifier to the entire group or to restrict alternation to part of the regex.Only parentheses can be used for grouping. Square brackets define a character class, and curly braces are used by a quantifier with specific limits.

### Bracket Expressions
A bracket expression is a regular expression that shall match a specific set of single characters and may match a specific set of multi-character collating elements, based on the non-empty set of list expressions contained in the bracket expression.

### Character Classes
Character classes distinguish kinds of characters such as distinguishing between letters and digits. One example that can be found in our code braket [\da-z\.-] from within our example. The \d represents any number from 0-9, a-z means we want all lowercase letters from a through z. The backslash shows us we want to use the literal characters for the peroid and dash which are usually dealt as special characters. The period usually Matches any single character except line terminators: \n, \r, \u2028 or \u2029. For example, /.y/ matches "my" and "ay", but not "yes", in "yes make my day", as there is no character before "y" in "yes".

### The OR Operator
Alternation is the term in regular expression that is actually a simple OR. In a regular expression it is denoted with a vertical line character. We dont have that in our example however a simple snippit would look like, -- I love HTML|CSS -- ,which matches I love HTML or CSS.

### Flags
As with the OR Operator, we do not contain any flags however. Flags affect the search functions of regular expressions one such flag is i. With this flag the search looks for all matches, without it -only the first match is returned. 

### Character Escapes
A characer escapes represents a character that may not be able to be conveniently represented in its literal form. An example from our code would be \., the forward slash before the peroid causes the character afterword to mean itseld literally. So in this case instead of being a special character the period is translated as a normal period.

## Author
My name is Daniel Pacheco, I am currently studying as a student at the University of Arizona to become a full-stack web developer. You can reach me by my github, https://github.com/Daniel-0117

