# JS Charts
 It's easy to get started with Chart.js. All that's required is the script included in your page along with a single canvas node to render the chart. 
 In your HTML page:
 <br>
 canvas id="income" width="600" height="400" canvas
 <br>
 <br>
 There is many types of charts : pie,bar..
 <br>
 <br>
 Declare your chart in JS
 <br>
( var income = document.getElementById("income").getContext("2d");
 new Chart(income).Bar(barData);)

 And then add your chart information.


# Drawing with canvas

 1.The grid:
 Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.
 <br>
 2.Drawing rectangles:
 Unlike SVG, canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

 First let's look at the rectangle. There are three functions that draw rectangles on the canvas:

 fillRect(x, y, width, height)
 Draws a filled rectangle.
 <br>
 strokeRect(x, y, width, height)
 Draws a rectangular outline.
<br>
 clearRect(x, y, width, height)
 Clears the specified rectangular area, making it fully transparent.
 <br>
 Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the ,origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.
 <br>
 3. Drawing text:
 The canvas rendering context provides two methods to render text:

 fillText(text, x, y [, maxWidth])
 Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
 strokeText(text, x, y [, maxWidth])
 Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
