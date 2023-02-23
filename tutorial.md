## SSN Validator Regex

## Introduction
What is a regex and why do we use them? A regex is a string sequence of numbers, special characters, and letters that define filters. They are used to enforce that text/data complies with the the defined regex. In this article, I will be explaining the functionality and why to use a Social Security Number Regex in your code. 

## Summary
Social Security Numbers follow a small set of rules. Some websites/organizations need to validate and use your SSN for many different reasons (you should always be careful about giving out your SSN). For example, if you are contacting your bank about your account balance, they need your SSN to verify it is you that is trying to get into your account and not someone else. Therefore, many banking companies will use a regex similar or identical to this one for their website:
regex = "^(?!666|000|9\\d{2})\\d{3}-(?!00)\\d{2}-(?!0{4})\\d{4}$";
In this article, I will talk about the functionality of the characters within this expression.

## Table of Contents
[link text](#Qualifications) 

[link text](#Anchors) 

[link text](#Quantifiers) 

[link text](#OR-Operator) 

[link text](#Back-references) 

[link text](#Look-ahead) 

## Regex Components

# Qualifications: 
The SSN is 9 digits long. It's broken up into 3 sections by -. Section 1 has 3 numbers, section 2 has 2 numbers, and section 3 has 4 numbers.

# Anchors: 
The ^ and $ are the anchors in a regex. The ^ is at the beginning and $ is at the end.

# Quantifiers: 
{x} says it has to have x number of digits present. The "d" before the bracket means it has to be a numeric-digit.

# OR-Operator: 
| means the "or" in a statement. !666|000| means it can't have 666 or 000.

# Back-references: 
\\ are used to refer to a previous matched expression. The \\ says that the previous rule is no longer used in the next part of the expression

# Look-ahead: 
?! is the negative look-ahead which enforces the absence of the following expression. ?!666|000| makes sure the SSN doesn't have 666 or 000.


Clay Andemar
[link]()