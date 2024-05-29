# Regex Tutorial For URL Matching /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

Regular expressions are powerful tools for pattern matching and the manipulation of text. Understanding how regex expressions work is important when defining search patterns. Once a search pattern is identified, tasks such as searching, validating, extracting, replacing, and formatting become possible.

## Summary

In this tutorial, we will be exploring the regular expression /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ for matching a URL. This regex is used specifically to match and validate URLs with optional HTTP or HTTPS protocols. Each component in this example has a unique purpose which is what we will be diving into now.

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

Anchors are regex components that assert something about the string or matching process. In our example `^` asserts the start of the string and makes sure that our URL starts at the very beginning. `$` also functions as an anchor but at the very end of our expression, signaling the end of our URL.

### Quantifiers

Quantifiers in regular expressions specify the number of occurrences of a character or a group of characters that the pattern should match. In our example `?` makes the protocol optional. (`http://` or `https://`)

### OR Operator

In regular expressions, the "or" operator allows you to specify alternatives within a pattern. It is represented by the `|` character. The "or" operator will match either the pattern on the right or the pattern on the left. We do not have the "or" operator in our specific regex example.

### Character Classes

Character classes provide a powerful way to specify patterns in regex, allowing you to match a wide range of characters with concise syntax. They are fundamental building blocks for creating complex regex patterns for text processing tasks. In our example, `[\da-z\.-]` matches any digit (`\d`), lowercase letter a-z (`a-z`), dot (`.`), or dash (`-`).

### Flags

Flags in regular expressions are optional parameters that modify the behavior of the regex pattern matching. Flags provide additional control over how the pattern is applied to the text being searched or manipulated. In our case we do not have any flags, which usually are appended with a `/` after the closing delimiter.

### Grouping and Capturing

Parentheses are used to group parts of a regular expression together. This is useful for applying quantifiers, alternation, and other regex operators to multiple characters or subpatterns as a single unit. We have several instances of this in our regex such as `(https?:\/\/)` which is allowing us to identify a specific part of our URL as a group.

### Bracket Expressions



### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
