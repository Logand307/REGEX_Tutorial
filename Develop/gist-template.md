# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Regex is a shorthand term used to describe the concept of regular expressions within the world of coding. Regular expressions are sequences of characters that specify a search pattern within text, and are particularly useful for defining filters. 

I will explain how the Regex expression below will be used to specificy a pattern for a email address. An example of an email address that meets these requirements is ldavis0123-_3@email.test.com

```

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

```



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

Anchors help to specify where the expression begins and ends, as well that designating what is between the start and finish.

^ - can be referred to as hat or caret marks the start of the expression

$ - marks the end of the expression

```

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

```

As you can see in our username Regex above, the ^ signifies the beginning of the expression, the requirements are between the parenthesis and $ signifies the ending of the expression.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

The first group within our example above includes the quantifier "+" at the end. What this snippet is doing is confirming that the input has letters that are only lowercase, numbers that are only 0-9, and only include "-" or "_". If these requirements are not met, the test for the expression will not pass.

```

([a-z0-9_\.-]+)

```

### OR Operator

The OR Operator is used for a concept known as Alternation within regular expressions. It is denoted with a vertical line character |. Our example of an email address does not include an OR operator, but I have provided the example below for reference.

```
I love MySQL2|MongoDB matches I love MySQL2 or MongoDB.
I love (MySQL2|MongoDB) matches I love MySQL2 or I love MongoDB.

```


### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Hello! My name is Logan Davis - I have been passionate about technology from a young age, and recently made the decision to change careers from my current field within commercial banking and shift into a technical position. As we near the end of our coding bootcamp, I can confidently say that I know I made the right decision. For more information on me or to see my other projects, please see the link to my github profile here: https://github.com/Logand307
