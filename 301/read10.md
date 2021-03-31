# Call Stack
 A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

 * When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
 * Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
 * When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
 * If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
 <br>

## Importance of call stack
 The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

 The understanding of the call stack is vital to Asynchronous programming.

## Asynchronous programming
 In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop. 

## Types OF Error Messages
 1. Reference errors
        This is as simple as when you try to use a variable that is not yet declared you get this type os errors. 
     <br>
 2. Syntax errors
        I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse. 
<br>
 3. Range errors
        Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
<br>
 4. Type errors
        Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.