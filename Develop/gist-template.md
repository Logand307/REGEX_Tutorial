# Logan's Regex: Email Matching Tutorial

Check out my tutorial below on matching email Regex style!
## Summary

Regex is a shorthand term used to describe the concept of regular expressions within the world of coding. Regular expressions are sequences of characters that specify a search pattern within text, and are particularly useful for defining filters. 

I will explain how the Regex expression below will be used to specificy a pattern for a email address. An example of an email address that meets these requirements is ldavis0123-_3@email.test.com

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Back-references](#back-references)


## Regex Components

### Anchors

Anchors help to specify where the expression begins and ends, as well that designating what is between the start and finish.

* ^ - can be referred to as hat or caret marks the start of the expression

* $ - marks the end of the expression

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

As you can see in our username Regex above, the ^ signifies the beginning of the expression, the requirements are between the parenthesis and $ signifies the ending of the expression.

### Quantifiers

* Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

* The first group within our example above includes the quantifier "+" at the end. What this snippet is doing is confirming that the input has letters that are only lowercase, numbers that are only 0-9, and only include "-" or "_". If these requirements are not met, the test for the expression will not pass.

```
([a-z0-9_\.-]+)
```

### Character Classes

* Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits.

```
/^([a-z0-9_\.-]+)@
([\da-z\.-]+)\.
([a-z\.]{2,6})$/
```

* In the our email example above, I have split the expression across three lines for better undertstanding. Each line signifies a character set denoted by []. This is ensuring that the input matches any character within the set (i.e. lowercase letters a-z, or any digit character \d).



### Grouping and Capturing

* Grouping and Capturing is the act of using () to capture part of a group with the specific pairing for an ID. This allows you to add quantifiers to the search and matches all that is enclosed within that group.

Our email address example includes three groups, which I have designated below:

```
([a-z0-9_\.-]+)
([\da-z\.-]+)
([a-z\.]{2,6})
```

### Bracket Expressions

* Brackets indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a hyphen to define a set. Our email address example includes a set of brackets within each group, which I have designated below:

```
[a-z0-9_\.-]
[\da-z\.-]
[a-z\.]
```

### Back-references

https://www.regular-expressions.info/

https://javascript.info/

https://www.javascripttutorial.net/

https://developer.mozilla.org/en-US/



## Author

Hello! My name is Logan Davis - I have been passionate about technology from a young age, and recently made the decision to change careers from my current field within commercial banking and shift into a technical position. As we near the end of our coding bootcamp, I can confidently say that I know I made the right decision. For more information on me or to see my other projects, please see the link to my github profile here: https://github.com/Logand307
