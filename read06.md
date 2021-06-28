# javaScript Object

* Object is a non-primitive data type in JavaScript.
* It is like any other variable, the only difference is that an object holds multiple
* values in terms of properties and methods. Properties can hold values of primitive data types and methods are functions.

In JavaScript, an object can be created in two ways:

Object literal
Object constructor
Object Literal
The object literal is a simple way of creating an object using ```{ }``` brackets. You can include key-value pair in ```{ },``` where key would be property or method name and value will be value of property of any data type or a function. Use comma ```(,)``` to separate multiple key-value pairs.

Syntax:
```javascript
var <object-name> = { key1: value1, key2: value2,... keyN: valueN};
```
The following example creates an object using object literal syntax.

Example: Create Object using Object Literal Syntax
```javascript
var emptyObject = {}; // object with no properties or methods
```
```javascript
var person = { firstName: "John" }; // object with single property
```

// object with single method
```javascript
var message = { 
                showMessage: function (val) { 
                            alert(val); 
                } 
            }; 
```
// object with properties & method
```javascript
var person = { 
                firstName: "James", 
                lastName: "Bond", 
                age: 15, 
                getFullName: function () { 
                        return this.firstName + ' ' + this.lastName 
                }
            }; 
```
You must specify key-value pair in object for properties or methods. Only property or method name without value is not valid. The following syntax is invalid.

Example: Wrong Syntax
```
var person = { firstName };

var person = { firstName: };
```
Access JavaScript Object Properties & Methods
You can get or set values of an object's properties using dot notation or bracket. However, you can call an object's method only using dot notation.

Example: Access JS Object
```javascript
var person = { 
                firstName: "James", 
                lastName: "Bond", 
                age: 25, 
                getFullName: function () { 
                    return this.firstName + ' ' + this.lastName 
                } 
            };

person.firstName; // returns James
person.lastName; // returns Bond

person["firstName"];// returns James
person["lastName"];// returns Bond

person.getFullName();
```
----------------
Object Constructor
The second way to create an object is with Object Constructor using new keyword. You can attach properties and methods using dot notation. Optionally, you can also create properties using [ ] brackets and specifying property name as string.

Example: Object Constructor
```javascript
var person = new Object();
```
// Attach properties and methods to person object     
```javascript
person.firstName = "James";
person["lastName"] = "Bond"; 
person.age = 25;
person.getFullName = function () {
        return this.firstName + ' ' + this.lastName;
    };

// access properties & methods 
person.firstName; // James
person.lastName; // Bond
person.getFullName(); // James Bond
```
------------

# Document Object Model or DOM

* **Every web page resides inside a browser window which can be considered as an object.**

* **A Document object represents the HTML document that is displayed in that window**

* **The Document object has various properties that refer to other objects which allow access to and modification of document content.**
* **The Objects are organized in a hierarchy. This hierarchical structure applies to the organization of objects in a Web document.**
  * **Window object − Top of the hierarchy. It is the outmost element of the object hierarchy.**
  * **Document object − Each HTML document that gets loaded into a window becomes a document object. The document contains the contents of the page.**
  * **Form object − Everything enclosed in the ```<form>...</form>``` tags sets the form object.**
  * **Form control elements − The form object contains all the elements defined for that object such as text fields, buttons, radio buttons, and checkboxes.**
  
![](https://www.tutorialspoint.com/javascript/images/html-dom.jpg)  