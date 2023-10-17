# Regex-Tutorial For Hex Value

Character combinations in strings can be matched using regular expressions, which are patterns. "Not" is indicated by the metacharacter ^ in a regular expression. Hence, "^a" denotes "do not match lowercase a," whereas "a" signifies "match lowercase a."

## Summary

I'll go over and dissect the parts of a regular expression that match hex values. A computer may be accurately informed about any particular color using the hexadecimal coding method, which guarantees precision and consistency in electronic displays. A six-digit number that comes before the # symbol in hexadecimal represents a color that can be utilized in a computer program or webpage.    Example /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Your Task](#your-task)
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Author](#author)

## Your Task

Developers write code, but they also *write about code*. Take a moment to search the web for tutorials about any of the subjects you’ve learned so far in this course. You’re likely to find thousands of tutorials written by developers of all skill levels, including junior developers&mdash;like yourself!

Your assignment this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. You'll use the template provided in the starter code to create your walkthrough.

## User Story

```md
AS A web development student
I WANT a tutorial explaining a specific regex
SO THAT I can understand the search pattern the regex defines
```

## Acceptance Criteria

```md
GIVEN a regex tutorial
WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile
WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial
WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does
WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile
```


## Author

I'm Bryce Hadl and I'm currently a student at KU studying Software Development my Github link for this repository is: `https://github.com/brycehadl/Regex-Tutorial/tree/main`
