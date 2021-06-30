# HTML Forms

**An HTML form is used to collect user input. The user input is most often sent to a server for processing.**

The HTML ```<form>``` element is used to create an HTML form for user input:
```html
<form>
.
form elements
.
</form>
```

The ```<input>``` Element
|Type|Description|
|-----|-----------|
|```<input type="text">```|	Displays a single-line text input field|
|```<input type="radio">```|Displays a radio button (for selecting one of many choices)|
|```<input type="checkbox">```|Displays a checkbox (for selecting zero or more of many choices)|
|```<input type="submit">```|Displays a submit button (for submitting the form)|
|```<input type="button">```|Displays a clickable button|

### Text Fields
The ```<input type="text">``` defines a single-line input field for text input.
```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>

-------------

### The ```<label>``` Element

The ```<label>``` tag defines a label for many form elements.

The ```<label>``` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

The ```<label>``` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the ```<label>``` element, it toggles the radio button/checkbox.

The for attribute of the ```<label>``` tag should be equal to the id attribute of the ```<input>``` element to bind them together.

### The Name Attribute for ```<input>```

##### If the "_name_" attribute is omitted, the value of the input field will not be sent at all.
----------------
# LISTS, TABLES AND FORMS

* Specifying bullet point styles
* Adding borders and backgrounds to tables
* Changing the appearance of form elements

There are several CSS properties that were created to work with specific types of HTML elements, such as lists, tables, and forms.

list-style-type
The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).

It can be used on rules that apply to the ```<ol>, <ul>, and <li>``` elements.

### UNORDERED LISTS
* none
* disc
* imagecircle
* imagesquare

### ORDER LISTS
* decimal
1 2 3
* decimal-leading-zero
01 02 03
* lower-alpha
a b c
* upper-alpha
A B C
* lower-roman
i. ii. iii.
* upper-roman
I II III

### list-style-image
```css
list-style-image: url("images/star.png");
```

### list-style-position
```css
list-style-position: outside;
list-style-position: inside;
```
### list-style
```css 
list-style: inside circle;
```

# Table Properties

### empty-cells
```css
empty-cells: show/hidden;
```
### border-spacing

### border-collapse

------------
# JavaScript - Events

Developers can use these events to execute JavaScript coded responses, which cause buttons to close windows, messages to be displayed to users, data to be validated, and virtually any other type of response imaginable.

Events are a part of the Document Object Model (DOM) Level 3 and every HTML element contains a set of events which can trigger JavaScript Code

### addEventListener

The addEventListener() is an inbuilt function in JavaScript which takes the event to listen for, and a second argument to be called whenever the described event gets fired. Any number of event handlers can be added to a single element without overwriting existing event handlers. 
Syntax: 
 

element.addEventListener(event, listener, useCapture);
Parameters: 
 

 

event : event can be any valid JavaScript event.Events are used without “on” prefix like use “click” instead of “onclick” or “mousedown” instead of “onmousedown”.
listener(handler function) : It can be a JavaScript function which respond to the event occur.
useCapture: It is an optional parameter used to control event propagation. A boolean value is passed where “true” denotes capturing phase and “false” denotes the bubbling phase.

```javascript
 document.getElementById("try").addEventListener("click", function(){
    document.getElementById("text").innerText = "GeeksforGeeks";
});
```