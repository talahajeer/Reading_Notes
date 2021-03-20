# Responsive Web Design

### What does Responsive mean?
 Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

 <br>
 <br>
Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. 

### Flexible Layouts
 Flexible layouts is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

 <br>
 <br>

### Media Queries
 Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.
 
 <br>
 <br>

### Flexible Media
The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.


# CSS Float
 There are four valid values for the float property:
 <br>
 Left and Right float elements those directions respectively.
 <br>
 None (the default) ensures the element will not float
 <br>
 Inherit which will assume the float value from that elements parent element.


### Clearing the Float
 Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.



 ##### Quoting from https://learn.shayhowe.com/advanced-html-css/responsive-web-design/     and    https://css-tricks.com/all-about-floats/