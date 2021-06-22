# Text in HTML
```html
<h1><h2><h3><h4><h5><h6> 
The <h1> to <h6> tags are used to define HTML headings.
```
```html
<p> : The <p> tag defines a paragraph
```
```html
<b> : The <b> tag specifies bold text without any extra importance.
<i> : The <i> tag defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic.
```
```html
<sup> : Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW
<sub> : Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H2O.
```
```html
<br> :
The <br> tag inserts a single line break.

The <br> tag is useful for writing addresses or poems.

The <br> tag is an empty tag which means that it has no end tag.
<hr> : The <hr> tag defines a thematic break in an HTML page (e.g. a shift of topic).
```
```html
<strong> : The <strong> tag is used to define text with strong importance. The content inside is typically displayed in bold.
<em> : The <em> tag is used to define emphasized text. The content inside is typically displayed in italic.
```
```html
<blockquote>: The <blockquote> tag specifies a section that is quoted from another source.
<q> : The <q> tag defines a short quotation.
```
```html
<abbr>:The <abbr> tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".
Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element.
```
```html
<cite> : The <cite> tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.).
<dfn> : The <dfn> tag stands for the "definition element", and it specifies a term that is going to be defined within the content.
```
```html
<address> : The <address> tag defines the contact information for the author/owner of a document or an article.
```
```html
<ins> : The <ins> tag defines a text that has been inserted into a document. Browsers will usually underline inserted text.
<del> : The <del> tag defines text that has been deleted from a document. Browsers will usually strike a line through deleted text.
<s> : The <s> tag specifies text that is no longer correct, accurate or relevant. The text will be displayed with a line through it.
```

--------------------------------------
# CSS
 ### External CSS
**CSS3 supports external style sheets. This technique allows you to define a style sheet as a separate document and import it into your web pages**

we should be uses the ```<link>``` tag on every pages and the ```<link>``` tag should be put inside the head section.
```html
<head>  
<link rel="stylesheet" type="text/css" href="mystyle.css">  
</head>  
```

### Internal CSS
+ You can integrate internal CSS stylesheets by placing the ```<style>``` element in the ```<head>``` section of a page.
Internal styles apply to whole pages but not to multiple HTML documents.
Several pages can be styled by repeating the same block of internal styles in them.
+ Internal styles apply to whole pages but not to multiple HTML documents.
+ Several pages can be styled by repeating the same block of internal styles in them.

### CSS Selectors

* **Universal selector**
Selects all elements. Optionally, it may be restricted to a specific namespace or to all namespaces.
Syntax: * ns|* *|*
Example: * will match all the elements of the document.

* **Type selector**
Selects all elements that have the given node name.
Syntax: elementname
Example: input will match any <input> element.

* **Class selector**
Selects all elements that have the given class attribute.
Syntax: .classname
Example: .index will match any element that has a class of "index".

* **ID selector**
Selects an element based on the value of its id attribute. There should be only one element with a given ID in a document.
Syntax: #idname
Example: #toc will match the element that has the ID "toc".

* **Attribute selector**
Selects all elements that have the given attribute.
Syntax: [attr] [attr=value] [attr~=value] [attr|=value] [attr^=value] [attr$=value] [attr*=value]
Example: [autoplay] will match all elements that have the autoplay attribute set (to any value).

------------------------------------
# javaScript

* Javascript reads code one-by-one line
* you can add comment by ```//```
* you cane declare variable with Let,Var,Const
* We have 3 data types : Numric,String,Boolean
* using QUOTES inside a string by using ```\```
* we can use shorthand for creating variables by using ```,```
* we can assign value by using```=```
* JavaScript is a Casesensitve 
* JavaScript arrays are used to store multiple values in a single variable
* JavaScript includes following categories of operators
  * Arithmetic Operators
 ```javascript
 var x = 5, y = 10, z = 15;

x + y; //returns 15

y - x; //returns 5

x * y; //returns 50

y / x; //returns 2

x % 2; //returns 1

x++; //returns 6

x--; //returns 4
 ```
  * Comparison Operators
   ```javascript
   var a = 5, b = 10, c = "5";
var x = a;

a == c; // returns true

a === c; // returns false

a == x; // returns true

a != b; // returns true

a > b; // returns false

a < b; // returns true

a >= b; // returns false

a <= b; // returns true

a >= c; // returns true

a <= c; // returns true
   ```
  * Logical Operators
   ```javascript
var a = 5, b = 10;

(a != b) && (a < b); // returns true

(a > b) || (a == b); // returns false

(a < b) || (a == b); // returns true

!(a < b); // returns false

!(a > b); // returns true
   ```
  * Assignment Operators
     ```javascript
    var x = 5, y = 10, z = 15;

    x = y; //x would be 10

    x += 1; //x would be 6

    x -= 1; //x would be 4

    x *= 5; //x would be 25

    x /= 5; //x would be 1

    x %= 2; //x would be 1

    ```

   * Conditional Operators
   ```javascript
   Ternary Operator
    var a = 10, b = 5;

    var c = a > b? a : b; // value of c would be 10
    var d = a > b? b : a; // value of d would be 5
   ```
