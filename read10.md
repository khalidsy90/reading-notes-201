# JavaScript error handling and debugging

Because JavaScript is a loosely and weakly typed language, it has always been its weakness in error debugging. If the script makes a mistake, the error message given to us is often a clueless hint; the good news is that due to the continuous upgrade of the browser, JavaScript The debugging ability is getting better and better.

1.try...catch debugging

```javascript
try{
   window.dddd();
}catch(e){
   alert(e);
```
> * This non-existent method, if there is an error, directly print it out in catch, e and js have two attributes of name and message, you can directly print out the name and information of e.name or e.message;

### Error type

1. #### SyntaxError
A SyntaxError is a type of error that is thrown when there is a typo in the code, creating invalid code - code which cannot be interpreted by the compiler.

Some common causes of a SyntaxError are:

   * Missing opening or closing brackets, braces, or parentheses
   * Missing or invalid semicolons
   * Misspelling of variable names or functions
2. #### TypeError
A TypeError is a type of error thrown when an attempt is made to perform an operation on a value of the incorrect type.

One example of a TypeError is using a string method on a numerical value.

3. ##### Javascript error stack trace

An error stack trace tells a developer that it has detected an error within the code. Along with, which line to find the error, what type of error has occurred and a description of the error.

4. #### Javascript documentation
Many times we can track down bugs, but still, be confused about how to solve it. During these situations, we can look at documentation. For JavaScript, the MDN JavaScript web docs is a powerful resource. If we are still confused after looking at this we can go to StackOverflow - a question and answer forum where programmers post issues and other programmers discuss and vote for solutions.

5. #### Runtime Error in JavaScript
A JavaScript runtime error is an error that occurs within code while its being executed. Some runtime errors are built-in objects in JavaScript with a name and message property. Any code after a thrown runtime error will not be evaluated.
6. #### Javascript Error Function
The JavaScript Error() function creates an error object with a custom message. This function takes a string argument which becomes the value of the error’s message property. An error created with this function will not stop a program from running unless the throw keyword is used to raise the error.

7. #### The throw Keyword in JavaScript
The JavaScript throw keyword is placed before an Error() function call or object in order to construct and raise an error. Once an error has been thrown, the program will stop running and any following code will not be executed.
8. #### Javascript try catch
A JavaScript try…catch statement can anticipate and handle thrown errors (both built-in errors as well as those constructed with Error()) while allowing a program to continue running. Code that may throw an error(s) when executed is written within the try block, and actions for handling these errors are written within the catch block.

### Common error types
Because JavaScript is a loosely typed language, many errors occur during runtime. Generally speaking,

1. Type conversion error;

Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
var foo = {}
foo.bar // undefined
foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined
This is probably the most frequent error in JS, trying to access a property/method thinking that bar is of the type object when in reality, since it hasn’t been declared yet, it’s undefined which doesn’t have any baz available.
The fix is simple, just make sure that bar exists before trying to access it, either by creating bar or by checking for undefined.

```javascript
var foo = { bar: {} }
foo.bar.baz // undefined but you avoid the error
or
var foo = {}
if (typeof foo.bar !== 'undefined') {
  foo.bar.baz // this will never be executed while bar does not exist
}
```
There are also warnings, for instance telling you about a deprecated method, which can be found more frequently in firefox developer tools.

2. The data type is wrong;

3. Communication error

