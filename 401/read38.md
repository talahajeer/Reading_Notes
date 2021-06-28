# Conditional Rendering
 In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

 Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

## Element Variables
 You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.

## Rendering Multiple Components
 You can build collections of elements and include them in JSX using curly braces {}.

 Below, we loop through the numbers array using the JavaScript map() function. We return a <li> element for each item. Finally, we assign the resulting array of elements to listItems

## Basic List Component
 Usually you would render lists inside a component.

 We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

## Forms
 HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state

## Controlled Components
 In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

 We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.