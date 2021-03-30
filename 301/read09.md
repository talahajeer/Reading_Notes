# What is functional programming?
 Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

# Functional programming concepts
 <br>
 Those concepts are big advantages to build side-effect-free functions, so it is easier to maintain systems — with some other benefits.
 <br>
 1. Pure Functions:
     <br>
     So how do we know if a function is pure or not? Here is a very strict definition of purity:
     <br>
     It returns the same result if given the same arguments (it is also referred as deterministic)
     <br>
     It does not cause any observable side effects
     <br>
     It returns the same result if given the same arguments
     <br>
 2. Immutability:
   <br>
     When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
 <br>
 3. Referential transparency:
     Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
     (pure functions + immutable data = referential transparency)
     <br>
     With this concept, a cool thing we can do is to memoize the function.
 <br>
 4. Functions as first-class entities:
     The idea of functions as first-class entities is that functions are also treated as values and used as data.
     Functions as first-class entities can:
         refer to it from constants and variables
         pass it as a parameter to other functions
         return it as result from other functions
         The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.
         <br>
 5. Higher-order functions:
     A function that either:
         takes one or more functions as arguments, or
         returns a function as its result
 <br>
 6. Filter
     Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection. Basically, if the callback expression is true, the filter function will include the element in the result collection. Otherwise, it will not.         