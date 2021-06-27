# JSX
 JSX is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

## Why JSX?
 React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

 Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

 React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

## JSX is an Expression Too
 After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

 This means that you can use JSX inside of if statements and for loops, assign it to variables, accept it as arguments, and return it from functions.

## Rendering Elements
 Elements are the smallest building blocks of React apps.

 An element describes what you want to see on the screen:

 const element = <h1>Hello, world</h1>;
 Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.