# HTML Lists
 There are three types of HTML lists: ordered using tag ol, unordered using tag ul, and definition dl. 

  1. Ordered lists:
     <br>
     The ordered list is created with the ol element. Each item in the list is placed between an opening li tag and a closing li tag.

  2. Unorderes lists:
     <br>
     The unordered list is created with the ul element. Each item in the list is placed between an opening li tag and a closing li tag.

  3. Definition Lists:
     <br>
     The definition list is created with the dl element and usually consists of a series of terms and their definitions.

# CSS Boxes
 You can set several properties that affect the appearance of these boxes.
 
 1.  Control the dimensions of your boxes:
     <br>
     By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties. You can use pixels, percentage or ems. Pixels are more commen to use due to its accuracy.

 2. Create borders around boxes:
     <br>
      Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

 3. Set margins and padding for boxes:
     <br>
     Margins: Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
     <br>
     Padding: Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

 4. Show and hide boxes:
     <br>
     The visibility property allows you to hide boxes from users but It leaves a space where the element would have been. This property can take two values:
     1. Hidden
     2. Visible

# JavaScript Array
 An array is a special type of variable. It doesn't just store one value; it stores a list of values.    
 <br> 
 You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array. 
 <br>
 var names;
 names = [Tala,Adel,Bana];
 <br>
 Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).
 <br>
 var numName; 
 numName = names[0]; 
 This will output the value of 0 index : Tala
 <br>
 Each array has a property called length, which holds the number of items in the array. 
 <br>
var lengthName;
lengthName = names.length;
This will output the count of the values in this array: 3