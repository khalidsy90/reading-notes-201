# links in HTML

**HTML Links - Hyperlinks**
**HTML links are hyperlinks.**
+ You can click on a link and jump to another document.

The HTML ```<a>``` tag defines a hyperlink. It has the following syntax:

```html
<a href="url">link text</a>
```

+ **Mailto** link is a type of HTML link that activates the default mail client on the computer for sending an e-mail.
```html
<a href="mailto:name@email.com">Link text</a>
```
* Opening Links in a *New Window* : just set the target attribute to ```_blank```:
```html
<p>Check out <a href="https://www.freecodecamp.org/" target="_blank">freeCodeCamp</a>.</p>
```
----------------
**How to create links to sections on the same page in HTML ?**
1. set a target
   ```html
    <a name="targetname"></a>
   ```
2. create a link to the target you just set
```html
    <a href="#targetname">Your Link Text</a>
```

# JavaScript Functions
JavaScript provides **functions similar** to most of the scripting and programming languages.

In JavaScript, a **function** allows you to define a block of code, give it a name and then execute it as many times as you want.

A JavaScript function can be defined using **function** keyword.
```javascript
//defining a function
function <function-name>()
{
    // code to be executed
};

//calling a function
<function-name>();
```
* A function can have one or more parameters, which will be supplied by the calling code and can be used inside a function. JavaScript is a dynamic type scripting language, so a function parameter can have value of any data type.
* A function can return zero or one value using return keyword.
* JavaScript allows us to assign a function to a variable and then use that variable as a function. It is called **function expression**.
Ex :
```javascript
var add = function sum(val1, val2) {
    return val1 + val2;
};

var result1 = add(10,20);
```
> * Points to Remember :
*  ##### JavaScript a function allows you to define a block of code, give it a name and then execute it as many times as you want.
* ##### A function can be defined using function keyword and can be executed using () operator.
* ##### A function can include one or more parameters. It is optional to specify function parameter values while executing it.
* ##### JavaScript is a loosely-typed language. A function parameter can hold value of any data type.
* ##### You can specify less or more arguments while calling function.
* ##### All the functions can access arguments object by default instead of parameter names.
* ##### A function can return a literal value or another function.
* ##### A function can be assigned to a variable with different name.
* ##### JavaScript allows you to create anonymous functions that must be assigned to a variable.

# JavaScript Scope
Scope determines the accessibility (visibility) of variables.

JavaScript has 3 types of scope:

1. ## Block scope

   > Variables declared inside a { } block cannot be accessed from outside the block:
```javascript   
{
  let x = 2;
}
// x can NOT be used here
```
2. ## Function scope

> * javaScript has function scope: Each function creates a new scope.

> * Variables defined inside a function are not accessible (visible) from outside the function.

> * Variables declared with var, let and const are quite similar when declared inside a function.

They both have Function Scope:
```javascript
function myFunction() {
  var carName = "Volvo";   // Function Scope
}
function myFunction() {
  let carName = "Volvo";   // Function Scope
  ```
3.  ## Global scope
 A variable declared outside a function, becomes GLOBAL.

```javascript
let carName = "Volvo";
// code here can use carName

function myFunction() {
// code here can also use carName
}
```

-------------
# Pair programming
**Pair programming** : consists of two programmers sharing a single workstation (one screen, keyboard and mouse among the pair). The programmer at the keyboard is usually called the “driver”, the other, also actively involved in the programming task but focusing more on overall direction is the “navigator”; it is expected that the programmers swap roles every few minutes or so.

###### *There are several compelling reasons you should consider this strategy:*
##### 1. Two heads are better than one
##### 2. More efficient
##### 3. Fewer coding mistakes
##### 4. An effective way to share knowledge
##### 5. Develops your staff’s interpersonal skills

###### *Why is pair programming important ?*
##### 1. Produce better solutions
##### 2. Share knowledge and context on the fly
##### 3. Mutual learning and skill development