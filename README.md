# RegEx-Tutorial

In this you will learn about a regular expression for an email address. A regular expression is a collection of characters that are defined in a pattern that typcally match the pattern of a string. These are used throughout almost all programming languages for example a few are C++, Javascript, Java, and Python. They are often used for searching and replacing in many softwares.

## Summary

The example of an expression that I will be using is an email address. An email has many different components in order for it to function properly. I will be using tommytest@gmail.com for this example. The "tommytest" in an email is typacally the local part of the email often being the username that is provided by the user. The "@" dictates the end of the so called username and the start of the domain that is being used. For this example the domain that is being used is "gmail.com". This is an account that is hosted by Google and utilizing their services.

Example:

    ^([a-zA-Z0-9_\-\.]+)@([a-zA-Z0-9_\-\.]+)\.([a-zA-Z]{2,5})$

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

- Repeaters
- Plus symbol
- Curly Bracket
- Wildcard
- Optional Characters
- Caret
- Dollar
- Character Classes
- Escape Symbol
- Grouping
- Vertical bar
- \Number
- Comment
- End of line

### Anchors

The anchor in this example is the caret or (^). This is stating that where ever there is a pattern that begins with the proceeding charaters are that is what will be the match. For example: ^star it will match stars@gmail.com, starrrs@gmail.com starz@gmail.com or any other variation after the star component.

### Quantifiers

The quantifiers specify how many characters are in the pattern we are trying to match. Quantifiers can be specified by a minimum value, a maximum value or even both. They are typically inside the curly brackets {}. If you are trying to specify a min it will be the first number followed by a "," and a "}". IF you wanted to have a max value amount then it would be "{ ," foollowed by a number. For an email the last part uses these to specify the length of it so that it is between 2 and 5 characters.

### Grouping Constructs

Grouping is done when you are trying to include characters as a one set by adding different types into it. For example: ([a-z]\w+) this will match a pattern that has and letter from the declared range next to another character of the same value. In the email these are used quite a few times. In the firs part when you are trying to match the local value it has all letters capital and lower case and all numbers. The domain listing is the same specifications and finally the final part only uses the letter both capital and lower case.

### Bracket Expressions

The bracket express for the email is matching a collection of multiple characters with the specified characters that are inside it. For this email it is stating that it is using all letters both upper and lower cas along with the numbers ranging from 0-9. this is being used in multiple locations such as the local name and the domain that is being used.

### Character Classes

This is the matching of any of the enclosed characters that are found between the 2 brackets. For example [abc-] with look for matching with and a or b or c or - in them.

### The OR Operator

The or operator functions very similar to the way it is used in other programming languages. It is a conditional that finds matches that have either of the conditions in the search. To use this we would use the | character. For example abc|xyz this is defining a pattern of either abc or xyz.

### Flags

These are filters that you can pass that will affect the way that it is searched. There are multiple options that you can use that will help you narrow your search to help you find the match that will be returned. For example "flag i" is one that will nullify the difference between A and a in the search.

### Character Escapes

This is how you can find the special characters that may hold a different meaning then the one you expected. If you wanted to find a "." in the document without using it has the any character that is associated with it in regex. A character escape will allow you to search for that "." without the meaning that it holds. To do this what you will do is include a \ before the character that you are trying to search for.

## Author

- [@marshallrizzuto](https://github.com/Zoot83)
