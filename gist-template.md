# Regex Explanation

Introductory paragraph (replace this with your text)

## Summary

Regex (or Regular Expression) allows user to search any types of characters (letter(s), number(s), word(s), etc.) through a string of text order to apply function, such as advance replace, find and many more. 

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

open slash + character in question + close slash + flag

ex: /a/g

### Anchors

"^" = The match located at the beginning of the string

Ex: /^\w+/g

"$" = The match located at the end of the string

Ex: /\.$/g

### Quantifiers

"+" = Match 1 or more of the preceding token
"?" = Match none or 1 of the preceding token
"*" = Match none or more of the preceding token
"." = match any characters before or after the token(except a new line)

### OR Operator

| or "OR Operator" allows the surrounding tokens to match separately

Ex: /e|E/g means it'll match e or E

### Character Classes
[] = Match any character in the set.

ex: /[ab]/g will match every "a" and/or every "b"

"\w" = match every characters.
"\W" = match everything but the characters (whitespace).
"\s" = match every whitespaces.
"\S" = match everything but the whitespace (characters).

### Flags
g = global
i = case insensitive
m = multiline
s = single line
u = unicode
y = sticky

### Grouping and Capturing
() =Capturing Group allows multiples tokens to be individually combined with the token to be matched separately

ex: /(e|E)x/g means it'll look for "ex" or "Ex"

### Bracket Expressions
{} = allows for a minimum and a maximum number for how large the match need

ex: /{4}/g =  any word with 4 characters
### Greedy and Lazy Match

### Boundaries

\b = word Boundary selects all characters of a word matching the token but the last character of a word string

ex: /e\b/g

\B = not word Boundary selects all the last character of a word matching the token

ex: /e\B/g

### Back-references
\1 = back-reference allows to a repeated that being matched with the code preceding the backreference code

ex: /(s)\1/g

### Look-ahead and Look-behind

"(?< =(token))" = look-behind

Ex:(?< =/([tT]he))./g look for anything after the matched characters

(?=(token)) = look-ahead

Ex: /.(?=ex)/g Look for anything before the matched characters

to invert the result, change "=" to "!"

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
