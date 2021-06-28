# HTML - Tables

* The HTML tables allow web authors to arrange data like text, images, links, other tables, etc.
* The HTML tables are created using the <table> tag .
* ```<tr>``` tag is used to create table rows .
*  ```<td>``` tag is used to create data cells .
*  The elements under ```<td>``` are regular and left aligned by default
* Table heading can be defined using ```<th>``` tag.
* There are two attributes called cellpadding and cellspacing which you will use to adjust the white space in your table cells.
```html
 <table border = "1" cellpadding = "5" cellspacing = "5">
 ```

* You will use colspan attribute if you want to merge two or more columns into a single column.
  
```html
<td rowspan = "2">Row 1 Cell 1</td>
```
##### You can set table background using one of the following two ways :

+ bgcolor attribute − You can set background color for whole table or just for one cell.

+ background attribute − You can set background image for whole table or just for one cell.

```html
   <table border = "1" bordercolor = "green" bgcolor = "yellow"
```

-------------------------------
# JavaScript | Object Constructors

* Object is the collection of related data or functionality in the form of key
* This functionalities are usually consists of several functions and variables.
* All JavaScript values are objects except **_primitives_**.
* A **_constructor_** is essentially a function that acts as a blueprint for creating objects. A convention for constructors is to always capitalize its function name.
```javascript
const app = (function(){
  //constructor function
  function Anime(name,type,year,director){
     this.name = name;
     this.type = type;
     this.year = year;
     this.director = director;
   }
```
create an Anime instance object called “trigun” :
```javascript
//new object instance
const trigun = new Anime("Trigun","post-apocalyptic","1998","Satoshi Nishimura");
```
# “new” keyword

* To create a new object instance I used the “new” keyword
  1. Creating an empty JavaScript object
  2. Linking the instantiated object to another object ( inheritance chain )
  3. Making the created empty object “this” ( see 1. )
  4. Returning “this” if a function doesn’t run on the correct object
* Without the “new” keyword, “this” will look to the window object.

# JavaScript this Keyword
In JavaScript, when this keyword is used in a constructor function, this refers to the object when the object is created. For example,
```javascript
// constructor function
function Person () {
    this.name = 'John',
}

// create object
const person1 = new Person();

// access properties
console.log(person1.name);  // John
```
Hence, when an object accesses the properties, it can directly access the property as ```person1.name```

