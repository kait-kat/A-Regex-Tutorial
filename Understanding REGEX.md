# Matching Hex Values

## Summary

Regular Expressions (regex), are special characters used to define a specific search pattern. To the typical user it may look like a random mixture of characters, but behind the screen it has key components that help the system identify and locate it quickly.    

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Character Escapes](#character-escapes)

## Regex Components

The hexadecimal, or Hex, is a positional numeral system that uses 16 specific symbols which consist of "0"-"9" to represent its same number values and "A"-"F" or "a"-"f" to represent the values of 10-15. A common use of the hex system is the hex color codes that a represent a color in RGB format. RGB format is what defines the amount of red, green and blue are used to make the color.
The following line of code is a regular expression that is used to match hex values.
```
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
```
To further understand what it does we must understand the representation of each character here.

### Anchors

Anchors are what represents the beginning and end of the string, in which they consist of ```^``` as the beginning and ```$``` as the end. Everything in between will be what the search is meant for.

### Quantifiers

Quantifiers are used to to indicate the number of characters or expressions to match. In the hex value expression we see the ```?``` as our first quantifier. 

### Grouping Constructs

Grouping can be show by using ```()```, this acts as a separation between meta characters and literal characters. Grouping is alos used to isolate data in a program. In the hex value expression, we are only seeing literal values, a meta search is not specified.

### Bracket Expressions

Character classes indentify the kinds of characters used such as letters and digits. The ```[a-f0-9]``` which we see twice, is a bracket expression specifying the range of characters using the hyphen. 

### The OR Operator

The ```|``` is our OR operator for this expression. The OR operator is meant to tell the regex to look for the numeric character hex value, in this case it is looking for the {6} or the {3}. With ```|``` in the middle it is making it possible to be the value of either 6 or 3. 

## References

> - [Mozilla Dev Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)
> - [W3 Schools](https://www.w3schools.com/js/js_regexp.asp)

## Author
[kait-kat](https://github.com/kait-kat)

