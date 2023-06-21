# Title (Dynashia's Regex Tutorial)

Introductory paragraph (replace this with your text)

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
A regex is considered a literal, so the pattern must be wrapped in slash characters (/). If we examine the “Matching a Username” regex, you'll see that this is true:

/^[a-z0-9_-]{3,16}$/

### Anchors
Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line.

The characters ^ and $ are both considered to be anchors.

The ^ anchor signifies a string that begins with the characters that follow it. This could be in one of two formats:

An exact string match, such as ^The, where the strings "The" or "The person" match, but "the" and "the person" do not. This is because a regex is case-sensitive.

A range of possible matches, displayed using bracket expressions. We'll discuss this in the next section.

The $ anchor signifies a string that ends with the characters that precede it. Just as with the ^ character, it can be preceded by an exact string or a range of possible matches.

So in our “Matching a Username” regex, the string must start and end with something that matches the pattern [a-z0-9_-]. You'll notice that we didn't include the pattern {3,16}, which precedes the $ character. Why? Because this is a special component called a quantifier. We'll come back to quantifiers in a moment.

Let's take a look at the pattern [a-z0-9_-] and see what it mean

### Quantifiers
What are quantifiers used for regex?
How Do Regular Expression Quantifier Work?
Quantifiers are used to quantify how many times a part of your regular expression should be repeated. Every time you want to repeat something in a regex (an individual character, a character class or a sub-expression) you can write a quantifier after it to specify how many times it should be repeated.

### OR Operator
The Range Operator ( - )
Regex recognizes range expressions inside a list. They represent those characters that fall between two elements in the current collating sequence. You form a range expression by putting a range operator between two characters.

### Character Classes
What is character classes in regex?
In the context of regular expressions, a character class is a set of characters enclosed within square brackets. It specifies the characters that will successfully match a single character from a given input string.

Construct	Description
[abc]	a, b, or c (simple class)
[^abc]	Any character except a, b, or c (negation)
[a-zA-Z]	a through z, or A through Z, inclusive (range)
[a-d[m-p]]	a through d, or m through p: [a-dm-p] (union)
[a-z&&[def]]	d, e, or f (intersection)
[a-z&&[^bc]]	a through z, except for b and c: [ad-z] (subtraction)
[a-z&&[^m-p]]	a through z, and not m through p: [a-lq-z] (subtraction)

### Flags
A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way. A flag is denoted using a single lowercase alphabetic character.

### Grouping and Capturing
What is group capturing in regex?
Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. For example, the regular expression (dog) creates a single group containing the letters "d" "o" and "g" .

### Bracket Expressions
A bracket expression (an expression enclosed in square brackets, "[]" ) is an RE that shall match a specific set of single characters, and may match a specific set of multi-character collating elements, based on the non-empty set of list expressions contained in the bracket expression.

### Greedy and Lazy Match
'Greedy' means match longest possible string. 'Lazy' means match shortest possible string. For example, the greedy h. +l matches 'hell' in 'hello' but the lazy h.

### Boundaries
What is a boundary in regex?
What is a word boundary in regex? - Stack Overflow
A word boundary, in most regex dialects, is a position between \w and \W (non-word char), or at the beginning or end of a string if it begins or ends (respectively) with a word character ( [0-9A-Za-z_] ).who i

### Back-references
back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are specified with backslash and a single digit (e.g. ' \1 '). The part of the regular expression they refer to is called a subexpression, and is designated with parentheses.

### Look-ahead and Look-behind
What is look ahead and look behind in regex?
Lookahead allows to add a condition for “what follows”. Lookbehind is similar, but it looks behind. That is, it allows to match a pattern only if there's something before it.

## Author

Dynashia Lewis Resides in Florida.

https://github.com/Dynashia