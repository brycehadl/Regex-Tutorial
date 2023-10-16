# Regex-Tutorial For Hex Value

Character combinations in strings can be matched using regular expressions, which are patterns. "Not" is indicated by the metacharacter ^ in a regular expression. Hence, "^a" denotes "do not match lowercase a," whereas "a" signifies "match lowercase a."

## Summary

I'll go over and dissect the parts of a regular expression that match hex values. A computer may be accurately informed about any particular color using the hexadecimal coding method, which guarantees precision and consistency in electronic displays. A six-digit number that comes before the # symbol in hexadecimal represents a color that can be utilized in a computer program or webpage.    Example /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

### Anchors

Anchors don't remotely fit any character. Rather, they align a place prior to, following, or in between characters. The regex match can be "anchored" at a certain point using them. The caret ~ corresponds to the string's initial character's position. Using ^a to match an ABC to a. Since the b cannot be matched by ^ immediately after the string's start, \b does not match any of the letters in the alphabet. The innards of the regex engine can be shown below. Likewise, $ matches immediately following the string's final character. In the ABC, c$ and c match, but a$ does not match at all.

### Quantifiers

The number of characters expected is expressed using quantifiers. The number of occurrences of a character, group, or character class that must exist in the input for a match to be found is indicated by quantifiers. Quantifiers match as many characters as they can by default because they are greedy. Regular expressions that contain the characters ",+,?,{}" are regarded as quantifiers. To match 0 or 1 times, the expression is indicated by the? As stated in the summary above, in order to differentiate between the two types of formats, we will use the or operator. The hex triplet format {6} and the shorthand hex format {3} in our Hex Value regular expression mean that the component preceding these quantifiers should have a length of 6 for {6} and 3 for {3}. 

### OR Operator
The `|` element is used in regular expressions to define the "or" operator. It could be any of the two parts that we are using the `|` to separate, according to the `or` operator. We have `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` for our hex value regular expression. Observe how the or operator divides these two parts. This implies that there are two possible values for our hex value: six characters `[a-f0-9]{6}` or three characters `[a-f0-9]{3}`.

### Character Classes

Character classes are parts of our regular expression that provide us with character type information. Our character classes are contained inside brackets [] in this example. We have two character classes in our example: `[a-f0-9]` and `[a-f0-9]`, and they both look for the same values. Within these character classes, we will analyze the searches that the characters are conducting. A to F looks for letters A to F, while 0 to 9 looks for numbers 0 to 9.

### Bracket Expressions

Bracket Expressions correspond to any character enclosed in square bracket. For instance, no, nO, No, and NO match [nN] [oO]. The word "grey" is spelled "gra[ae]y," which is the same as both gray and grey.

### Greedy and Lazy Match

An element is matched as many times as possible in a greedy match. In contrast, a lazy match makes an effort to match an element as infrequently as feasible. The lazy quantifier in our example is denoted by? The reason this is called a lazy quantifier is that it makes the regular expression engine match the fewest possible occurrences. All we need to do is add a? to this indolent match to make it greedy.

## Author

I'm Bryce Hadl and I'm currently a student at KU studying Software Development my Github link for this repository is: `https://github.com/brycehadl/Regex-Tutorial/tree/main`
