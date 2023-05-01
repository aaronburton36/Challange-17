# Title (replace with your title)

Regular expressions, also known as regex, is a powerful tool used for pattern matching and substitution. This markdown document will cover the varrious components of regex, from anchors to look-ahead and look-behind.

## Summary

In this guide, we will be describing a regular expression that matches email addresses. it willcontain explanations and code snippets of the different regex components in action.

email_regex = /^[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$/i

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

### Anchors
Anchors let you specify the position of the match within the string. in our email regex, we use the ^ and $ anchors to ensure that the entire string is matched.

### Quantifiers

Quantifiers allow you to specify how many times a character or group should be matched. in our email regex, we use the + quantifier to match one or more characters.

### OR Operator
The OR operator (|) allows you to match either one pattern or another. in our email regex, we use it to match either . or - patterns

### Character Classes
Character classeslet you match any one chracter from a list of chracters. in our email regex we use the [a-z] character class to match any lowercase letter

### Flags
Flags modify how the regular expression is intrepreted. the i flag in our email regex makes the match case-sensitive
### Grouping and Capturing
Grouping lets you group multiple chracters or patterns together to apply quantifiers or other operations to them as a whole. Capturing lets you extract the matched groups for later use. in our email regex, we use both grouping () and capturing () to extract the username and domain name of the email.
### Bracket Expressions

Bracket expressions, or character sets,let you match any one character within a range or set of characters. in our email regex, we use the [._%+-] bracket expression to match any one character within the given range.

### Greedy and Lazy Match

Quantifiers are greedy by default, where they match as many characters as posssible. a lazy match will match as few chracters as possible. in our email regex, we use the + quantifier to perform a greedy match.

### Boundaries


boundaries let you match certain positions within a string, such as the beginning or end of a word. in our email regex, we use the /b boundary to ensure the username and domain name of the email do not contain any additional characters before or after the match.


### Back-references

Back-referencing lets you reference captured groups within the same regular expression. in our email regex, we use the back-reference \1 to match the same character that was captured in the first group

### Look-ahead and Look-behind
Look-ahead and look-behind let you match patterns. in our email regex, we use the look-ahead (?=...) to match only if the domain name is followed by a period and two or more letters.
## Author

Hi! i'm Aaron im an full-stack developer checkout my git profile at https://github.com/aaronburton36