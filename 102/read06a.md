# JavaScript Functions:

## What is a function?
 Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). 

## Declaring a function:
 To create a function you give it a name then write the statements needed to achieve its task inside the curly braces.
    
    function funName(){
        code;
    }

## calling a function:
 Having declared the function you can the execute all of the statements between its curly braces with just one line of code wich known as CALLING a function.

    funName();     

## Declaring functions that need information:
  Sometimes a function needs a specific information to perform its task. In such case you declare a function and give it PARAMETERS.
   
   function area(width,height){
        code;
        return width*height;
    }
### To call such function:
     area(3,5);



# CSS:
 CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look. Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like). CSS rules usually appear in a separate document, although they may appear within an HTML page.
  

## Colors in CSS:
 Color not only brings your site to life, but also helps convey the mood and evokes reactions.

## color specificartion:
There are three ways to specify colors in CSS: 
  1. RGB values background-color: rgb(0,160,230);
  2. hex codes background-color: #ffffff;
  3. color names color: white;

## Color pickers:
Color pickers can help you find the color you want. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).

CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.

CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.