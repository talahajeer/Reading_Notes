# JavaScript objects
 Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names. 

 ## Lets say we have a project about a hotel
 
 | PROPERTIES: |      KEY    |    VALUE    |
 | ------------|-------------|-------------|
 |-------------|    name     |   string    |
 |-------------|   rooms     |    number   |
 |-------------|   booked    |    number   |
 |-------------|     gym     |   Boolean   |
 |-------------|  room Types |    array    |
 |  METHODS:   |checkAvailability| function|
 <br>

## Creating an Object
 Here is an example of how to create an object in literal notation.
 <br>
 var objectName {
     <br>
     porperty1: value,
     <br>
     porperty2: value,
     <br>
     porperty3: value,
    <br>
     methodName: function(){
        <br>
        code ...
        <br>
     }
     <br>
     };

## Accessing an Object

 var something = objectName .propety OR mrthod;

# DOM tree
 DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes. You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
 <br>
 From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques. 