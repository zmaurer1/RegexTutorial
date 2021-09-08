Regex Tutorial: Matching a URL

Today we're going to look at matching a URL

## Summary

Today we are going to be going over the regex of matching a URL
(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?
It's almost like taking the end of validating an email and putting it after "http//" and before file structure.

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
Below you'll find a list of components explained and the snippets that are used in the regex of matching a URL.

### Anchors
Anchors are members of the family of regex tokens that don't match any characters, but they assert something involving the string or the matching process. They assert that the current position in a string matches a well determined location.

^abc$   start / end of the string
\b	    word boundary

### Quantifiers
Quantifiers are used to specify how many instances of an element are to be matched.

a* a+ a? 	0 or more, 1 or more, 0 or 1
a{5} a{2,}	exactly five, two or more
a{1,3}	    between one & three
a+? a{2,}?	match as few as possible
ab|cd	    match ab or cd

### Grouping Constructs/Lookaround
Grouping constructs describe the subexpressions of a regular expression and hold the substrings of an input string.

abc)	capture group
\1	    backreference to group #1
(?:abc)	non-capturing group
(?=abc)	positive lookahead
(?!abc)	negative lookahead

### Bracket Expressions
Most characters are valid in URLs, even parenthesis even though they are rarely seen. They are rare as you have to determine if a closing parenthesis is a part of the URL or used as punctuation.

### Character Classes
Character classes define a set of characters, any of which can occur in an input string for a match to succeed.

.	        any character except newline
\w \d \s	word, digit, whitespace
\W \D \S	not word, digit, whitespace
[abc]	    any of a, b, or c
[^abc]	    not a, b, or c
[a-g]	    character between a & g

### Flags
Flagging URL patterns are an alternative to flagging views with decorators.

### Character Escapes
A character escape is a character that invokes an alternative interpretation on certain characters in a character sequence. It is a version of a metacharacter.

\. \* \\	escaped special characters
\t \n \r	tab, linefeed, carriage return
\u00A9	    unicode escaped ©

## Author
I am Zach Maurer and I am a writer and producer who is excited to jump into technical writing, web development and cyber-security! The link to my github is https://github.com/zmaurer1