## SSN Validator Regex

# Introduction
What is a regex and why do we use them? A regex is a string sequence of numbers, special characters, and letters that define filters. They are used to enforce that text/data complies with the the defined regex. In this article, I will be explaining the functionality and why to use a Social Security Number Regex in your code. 

# Summary
Social Security Numbers follow a small set of rules. Some websites/organizations need to validate and use your SSN for many different reasons (you should always be careful about giving out your SSN). For example, if you are contacting your bank about your account balance, they need your SSN to verify it is you that is trying to get into your account and not someone else. Therefore, many banking companies will use a regex similar or identical to this one for their website:
regex = "^(?!666|000|9\\d{2})\\d{3}-(?!00)\\d{2}-(?!0{4})\\d{4}$";
In this article, I will talk about the functionality of the characters within this expression.

# Table of Contents
Qualifications

Anchors

Quantifiers

OR Operator

Character Classes

Flags

Grouping and Capturing

Bracket Expressions

Greedy and Lazy Match

Boundaries

Back-references

Look-ahead and Look-behind

# Regex Components


Qualifications: The SSN is 9 digits long. It's broken up into 3 sections by -. Section 1 has 3 numbers, section 2 has 2 numbers, and section 3 has 4 numbers.

Anchors

Quantifiers

OR Operator

Character Classes

Flags

Grouping and Capturing

Bracket Expressions

Greedy and Lazy Match

Boundaries

Back-references

Look-ahead and Look-behind


Author
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)