
# Objects :
a set of variables and functions to create a model of a something you would recognize from the real world and there is 2 important ruls on this:
> VARIABLES BECOME KNOWN AS PROPERTIES IN OBJECTS
> ALSO FUNCTIONS KNOWN AS METHODS
and all looks like:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-1.PNG)

## how to create an object :
there is alot of ways to create an object..one of them is

### The Literal Notation:
witch is the easiest and most popular way, it used when the name of property is number OR a variable is being used in place of the property name, it looks like the object is inside the curly braces as previous example..
you can access this kind of objects with the **dot notation** OR **square brackets**

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-2.PNG)

<br>
<br>

# DOM :
**The Document Object Model** witch is neither part of HTML, nor part of JavaScript, it is a separate set of rules

### DOM tree:
witch is model of the page created by the browser and stored in the browser memory and consists of four main types of nodes:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-3.PNG)

1. THE DOCUMENT NODE "yleow" :
witch is in the top of *DOM Tree* and represents the entire page, It is the starting point for all visits to the DOM tree

2. ELEMENT NODES "blue" :
witch describe the structure of an HTML page

3. ATTRIBUTE NODES "red" :
witch is the attributes that carryied in HTML tags

4. TEXT NODES "purple" :
witch is able to reach within the main element 

```
- Each node is an object with methods and properties.
- Scripts access and update this DOM tree (not the source HTML file).
- Any changes made to the DOM tree are reflected in the browser
```

### WORKING WITH THE DOM TREE :
first you have to 
- ACCESS THE ELEMENTS :
and contains 3 ways to access:

1. SELECT AN INDIVIDUAL ELEMENT NODE
use `getElementByld()` witch takes the *id* attribute for the elemment OR use `querySelector()`

2. SELECT MULTIPLE ELEMENTS (NODELISTS)
use `getElementsByClassName()` witch Selects all elements that have a specific value for their class attribute OR use `getElementsByTagName()` OR `querySelectorAll()`

3. TRAVERSING BETWEEN ELEMENT NODES
parentNode OR previous Sibling/nextSibling OR firstChild/lastChild

- WORK WITH THOSE ELEMENTS :

1. ACCESS/UPDATE TEXT NODES
use `nodeValue` witch lets you access or update contents of text node

2. WORK WITH HTML CONTENT
`innerHTML` will allows you to access to child elements and text content OR `create Element(), createTextNode(), appendChild()/removeChild()` witch called **DOM manipulation**

3. ACCESS OR UPDATE ATTRIBUTE VALUES
use `hasAttribute(), getAttribute(), setAttribute(), removeAttribute()`

### the DOM querys :
witch is the metods that find elements in the DOM tree

> you can store element location in varible when you need to use several times..

### METHODS THAT RETURN A SINGLE ELEMENT NODE:
- `getElementById('id')`
- `querySelector('css selector')`

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-4.PNG)

### METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST):
- `getElementsByClassName('class')`
- `getElementsByTagName('tagName')`
- `querySelectorAll('css selector')`

## Nodelist :
witch is a collection of element nodes, Each node is given an index number, they are a type of object called a **collection** and Like any other object, a Nodelist has properties and methods like :
- The length property
- The item() method
also you can store this nodelist in variable and reused it, example:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-5.PNG)

> `item()` method is preferred, cuse its faster  

***you can easliy loop throgh nodelist*** like:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-6.PNG)

### TRAVERSING THE DOM :
by using these proparties to select an element that in relation with other element
1. `.parentNode`
2. `.previousSibling`,`.nextSibling`
3. `.firstChild`,`.lastChild`

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture06-7.PNG)



<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
