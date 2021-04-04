# EJS Partials

 Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.
### Example The same navigation bar and footer appear in both the home and post view. This makes them perfect candidates for partials!
<br>
<br>
<br>

## Create:
 create those partials. Under the views/partials/ directory create a file for example:  callednavbar.ejs which will contain only the HTML for the navigation bar at the top of the home and post pages.
<br>
<br>
<br>

## Locate:
 Including a partial in EJS is quite straightforward. You use `<%- include( PARTIAL_FILE ) %>` where the partial file is relative to the template you use it in. 