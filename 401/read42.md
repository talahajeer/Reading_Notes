# Enriching Your Python Classes With Dunder (Magic, Special) Methods
 What Python’s “magic methods” are and how you would use them to make a simple account class more Pythonic.

## What Are Dunder Methods?
 In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__.

 As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”

 These “dunders” or “special methods” in Python are also sometimes called “magic methods.” But using this terminology can make them seem more complicated than they really are—at the end of the day there’s nothing “magical” about them. You should treat these methods like a normal language feature.

 Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string').

## Special Methods and the Python Data Model
 This elegant design is known as the Python data model and lets developers tap into rich language features like sequences, iteration, operator overloading, attribute access, etc.

 You can see Python’s data model as a powerful API you can interface with by implementing one or more dunder methods. If you want to write more Pythonic code, knowing how and when to use dunder methods is an important step.

 For a beginner this might be slightly overwhelming at first though. No worries, in this article I will guide you through the use of dunder methods using a simple Account class as an example.

## Enriching a Simple Account Class
 Throughout this article I will enrich a simple Python class with various dunder methods to unlock the following language features:

 - Initialization of new objects
 - Object representation
 - Enable iteration
 - Operator overloading (comparison)
 - Operator overloading (addition)
 - Method invocation
 - Context manager support (with statement)
 - You can find the final code example here. I’ve also put together a Jupyter notebook so you can more easily play with the examples.