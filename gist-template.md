# Regex - Matching an Email Summary

In this project I will be breaking down a regular expression that is used to identify email address.

## Summary

* Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The above code is a regular expression or regex that will identify email addresses. There are various components in this expression that make it work. I will explain the how the regex functions, its different pieces and their role in the expression.

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

### Anchors

<!-- The carat symbol " ^ " and dollar sign " $ " are anchors. The carat anchor is used to match the starting text and the dollar sign is used to match the ending text.

^ - matches the sequence's starting text

$ - matches the sequence's ending text -->

### Quantifiers

Examples of quantifiers include asterisks " * ", a plus sign " + ", a question mark " ? ", and a set of curly brackets with an integer in between " { Number } ". 

* - used to find 0 or more occurrences of a character

+ - used to find 1 or more occurrences of a character

? - used to find 0 or 1 occurrences of a character

{3} - used to a specified number of occurrences of a character, in this example we are looking for instances where the character occurs three consecutive times

{2, 6} - used to find instances where a character is used consecutively in the range specified range, in this example we are looking for a character that is used 1 to 3 threes in a row

### Grouping Constructs

Grouping contructs in regex are what allow you group specific parts of the text together. We use parentheses.

In our regex ([a-z0-9_\.-]+),([\da-z\.-]+), ([a-z\.]{2,6}) are examples of grouping constructs. The first is referring to the email username, the second is the hosting site and the third is domain name (.com, .net, etc).


### Bracket Expressions

Bracket expressions allow you to specify which characters can be used at a particular point in the text.

In our regex the [a-z0-9_\.-] represents the characters one can input username part of an email address and [\da-z\.-] is referring to the name of the hosting site.

### Character Classes

" [ ] " is where you insert the input for the regex engine

" \ . " is used as a linebreaker to end the character class set 

### The OR Operator

" | " the OR operator is used when you would like to pull results with different user selections, for example "(apples | oranges)"

### Flags

N/A

### Character Escapes

" \." In our regex above this is looking to match with a period character, " \da-z" is matching with any digit or a - z character

## Author

Anthony Vaquer

Email Address: anthonymark126@gmail.com
GitHub ID: AnthonyVaquer
Repository Link: https://github.com/AnthonyVaquer/Regex-Tutorial
