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

Bracket expressions in regular expressions are used to define a set of characters that can match a single character at a specific position in the text being searched. They allow you to specify a range or group of characters from which one character must be matched. An example of this in our regex would be `[\/\w \.-]`.

### Greedy and Lazy Match

In regex, greedy matching tries to match as much text as possible while lazy matching tries to match as little text as possible while still allowing the overall pattern to match. In our example, the `*` is greedy because it is trying to match as much text as possible. This is important because it will use the entire path. We do not have any instances of lazy matching in our specific example.

### Boundaries

Boundaries in regular expressions are important for making sure that matches occur at specific positions within the text and for defining the scope of the search. They help control where and how the pattern should match. Examples of these are `\n` and `\r` even though these are not used in our regex.

### Back-references

Back-references in regular expressions (regex) are references to previously captured groups within the same regex pattern. They allow you to match repeated occurrences of the same text or to enforce consistency within a pattern. We do not have any instances of back-references in our regex example.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions are zero-width assertions in regular expressions that allow you to check for patterns without consuming characters in the string being matched. While they are powerful tools for creating complex regex patterns, we do not use them in our example.

## Author

This regex tutorial on URL matching is brought to you by Nick Bruggeman. As a current coding boot camp student that has struggled in different phases throughout my course, I wanted to create a tutorial that could assist in helping others understand the structure of a regular expression while also explaining the many different components of said regular expression. I hope this has helped and if you have any questions please reach out to me or view more of my projects at https://github.com/nbruggeman92. Thank you!