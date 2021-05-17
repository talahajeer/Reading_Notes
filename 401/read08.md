# List Comprehensions in Python
 List comprehensions provide a concise way to create lists.

 It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.
 <br>

 ## Syntax

 The list comprehension starts with a ‘[‘ and ‘]’, square brackets, to help you remember that the result is going to be a list.
 
 The basic syntax uses square brackets.

 ```[ expression for item in list if conditional ]```
 
 This is equivalent to:

```
for item in list:
    if conditional:
        expression
```