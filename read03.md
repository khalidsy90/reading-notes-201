# HTML Lists

**1. ```<ul>``` − An unordered list. This will list items using plain bullets.**
```html
     <ul>
         <li>Beetroot</li>
         <li>Ginger</li>
         <li>Potato</li>
         <li>Radish</li>
      </ul>
```
**2. ```<ol>``` − An ordered list. This will use different schemes of numbers to list your items.**
```html
  <ol>
         <li>Beetroot</li>
         <li>Ginger</li>
         <li>Potato</li>
         <li>Radish</li>
      </ol>
```
**3. ```<dl>``` − A definition list. This arranges your items in the same way as they are arranged in a dictionary.**
```html
   <dl>
         <dt><b>HTML</b></dt>
         <dd>This stands for Hyper Text Markup Language</dd>
         <dt><b>HTTP</b></dt>
         <dd>This stands for Hyper Text Transfer Protocol</dd>
      </dl>
```

### *A Nested List*
Lists can be nested (list inside list):
```html
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```

-------------------------------
# Boxes

+ **height** and **width** properties are used to set the height and width of an element.
![width_height](https://hackernoon.com/hn-images/1*KJU8PVgacXera7VUarSNkQ.png)
+ **max-width** property is used to set the maximum width of an element.
+ **min-width** property defines the minimum width of an element.
![min_max_width](https://ishadeed.com/assets/min-max/use-case-5.png)
+ **min-height** property defines the minimum height of an element.  
+ + **max-height** property defines the maximum height of an element.
![min_max_height](https://i.stack.imgur.com/72445.png)

# The CSS Box Model
![css box modal](https://s1.o7planning.com/en/12495/images/51081143.gif)
Explanation of the different parts:

+ Content - The content of the box, where text and images appear
+ Padding - Clears an area around the content. The padding is transparent
+ Border - A border that goes around the padding and content
+ Margin - Clears an area outside the border. The margin is transparent
--------------
+ **overflow** property controls what happens to content that is too big to fit into an area.
    + The overflow property only works for *block* elements with a specified height.
+ **display** property specifies the display behavior (the type of rendering box) of an element.
    + **inline** : Displays an element as an inline element (like <span>). Any height and width properties will have no effect
    + **Block** : Displays an element as a block element (like <p>). It starts on a new line, and takes up the whole width.
    + **inline-block** : Displays an element as an inline-level block container. The element itself is formatted as an inline element, but you can apply height and width values 

--------------
# JavaScript Notes

+ The statements are executed, one by one, in the same order as they are written.
+ JAVASCRIPT IS CASE SENSITIVE
+ A script is made up of a series of statements. Each
statement is like a step in a recipe.
+ JavaScript distinguishes between numbers (0-9),
strings (text), and Boolean values (true or false).
+ Arrays are special types of variables that store more
than one piece of related information.

# Javascript Decision Making

     + Decision Making statements are if, else, elseif and switch these statements are used in making decisions.
  
  In JavaScript we have the following conditional statements:

+ Use ```if``` to specify a block of code to be executed, if a specified condition is true
+ Use ```else``` to specify a block of code to be executed, if the same condition is false
+ Use ```else if``` to specify a new condition to test, if the first condition is false
+ Use ```switch``` to specify many alternative blocks of code to be executed

# For Loop

* A ```for``` loop repeats until a specified condition evaluates to false
```javascript
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```
* The While Loop
  
The while loop loops through a block of code as long as a specified condition is true.
```javascript
while (i < 10) {
  text += "The number is " + i;
  i++;
}
```