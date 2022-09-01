# Title (What is Regex)

What is Regex and how do you use it?  Regex is short for regular expression.  It is used to create patterns that you can use to match, find, and manage text.  It uses anchors, quantifiers, operators, classes, and flags to help parse text data to search for what you ask it to.  Let's dive in and learn how to use it.

## Summary

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
### Here are some examples of Regex Components 

* Anchors $ ^
* Quantifiers ? {} * +
* Grouping and Capturing ()
* Character classes . \d \w
* Greedy match *
* Bracket expressions []

### Anchors

Anchors look for what you ask it to look for.  Take the ^ symbol, you can place it before a word you want to look for, and it will return the string that starts with the word you searched for.  the $ symbol will match a string that ends with the word you placed the $ symbol behind.  you can use them together also.  For an example, you can have ^The and end$ and it will return the string that stars with "The" and ends with "end".

### Quantifiers

abc*       matches a string that has ab folllowed by zero or more c

abc+       matches a string that has ab folllowed by one or more c

abc?       matches a string that has ab folllowed by zero or one c

abc{2}     matches a string that has ab folllowed by 2 c

abc{2, }   matches a string that has ab folllowed by 2 or more c

abc{2,5}   matches a string that has ab folllowed by 2 up to 5 c

a(bc)*     matches a string that has a folllowed by zero or more copies of the sequence bc

a(bc){2,5} matches a string that has a folllowed by 2 up to 5 copies of the sequence bc

### OR Operator

a(b|c)    matches a string that has a folllowed by b or c (and captures b or c)

a[bc]     matches a string that has a folllowed by b or c 

### Character Classes

\d    matches a single character that is a digit

\w    matches a word character (alphanumeric and underscore)

\s    matches a whitespace character (tabs and line breaks)

.     matches any character

capitalizing the letter will give you the opposite. Example- \D matches a single non-digit character

### Flags

when you write regex, you place what you are looking for inside slash characters.  after the slash you can use a flag to be more specific.

### Grouping and Capturing

for grouping, parentheses are used to define the scope and precedence of the operators. gr(a|e)y  will search for gray or grey.

for capturing, parentheses create a capturing group. example a(bc) will create a group with value bc

### Bracket Expressions

brackets [] matches one character that is inside the bracket.  example- [a-z] will match any character that is lowercase and is between a-z including a and z

### Greedy and Lazy Match

greedy match will expand the match as far as it can through the provided text.  while lazy match, will only match what you tell it to.  you add a ? to make it a lazy match

### Boundaries

a boundary is an anchor that matches a position where one side is a word character

### Back-references

using the \1 will match the same text that was matched by the first capturing group

### Look-ahead and Look-behind

you match a character if followed by the character you specify. example- d(?=r) will match a d followed by an r but doesn't include the r in the match.  you can look behind by adding a <.  example d(?<=r) will look for a d that has an r infront of it.

## Author

I am Keith Williams.  I am currently a student working towards my certification in a full stack development program.  you can check out my other work at my GitHub profile https://github.com/keithmw5597
