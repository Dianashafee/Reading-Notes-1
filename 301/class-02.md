# jQuery 

 is a fast, lightweight, and feature-rich JavaScript library that is based on its motto “write less, do more”. jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, and animation much simpler.
All the power of jQuery is accessed via JavaScript, in order to use jQuery, the first thing you need to do is include the jQuery script in your page just like other scripts. You can download a copy of the jQuery library from www.jquery.com, or, as an alternative, you can include it from a CDN (Content Delivery Network), like Google or Microsoft.

## WHY :
If you’re not familiar with jQuery, you might be wondering what makes jQuery so special. There are several advantages why one should opt for jQuery:

1. SIMPLE SELECTORS
2. COMMON TASKS IN LESS CODE
3. CROSS-BROWSER COMPATIBILITY

# jQuery Selectors :

jQuery is used to select (query) HTML elements and perform “actions” on them. Basic syntax is:

`$("selector").action()`
The $ accesses jQuery.
The (selector) finds HTML elements.
The action() is then performed on the element(s).

jQuery holds refrence to the selected elements, basically what it is doing is storing the location a piece of information in the browser’s memory. The jQuery object is an array-like object because it stores a list of the elements in the same order that they appear in the HTML document (unlike other objects where the order of the properties is not usually preserved).

Caching Jquery Selections in Variables
Each time you use a selector in jQuery the DOM is searched for elements that match your query. Doing this too often or repeatedly will decrease performance. If you refer to a specific selector more than once you should add it to the cache by assigning it to a variable:

` let nav = $('#navigation');
nav.show();`

This would replace:
`$('#navigation').show(); `

## Updating Elements

Here are four methods that update the content of all elements in a jQuery selection:

`.html()`

Get the HTML contents of the first element in the set of matched elements or set the HTML contents of every matched element.

`.text()`

Get the combined text contents of each element in the set of matched elements, including their descendants, or set the text contents of the matched elements.

`.replaceWith()`

Replace each element in the set of matched elements with the provided new content and return the set of elements that was removed.

`.remove()`

Remove the set of matched elements from the DOM.

Inserting Elements
Inserting new elements involves two steps:

- Create the new elements in a jQuery object
- Create new jQuery objects to hold text and markup
- Use a method to insert the content into the page

Once you have a variable holding the new content, you can use the following methods to add the content to the DOM tree:

`.before()`

This method inserts content before the selected element(s) .

`.prepend()`

This method inserts content inside the selected element(s), after the opening tag

`.after()`

This method inserts content after the selected element(s).

`.append()`

This method inserts content inside the selected element(s), before the closing tag

Getting and Setting CSS properties
The `.css()` method lets you retrieve and set the values of CSS properties.

To GET the value of a CSS property, you indicate which property you want to retrieve in parentheses. If the matched set contains more than one element, it will return the value from the first element. For example:

`var backgroundColor = $(‘li’).css(‘background-color’);`    

To SET the values of a CSS property, you specify the property name as the first argument in the parentheses, then a comma, followed by its value as the second argument. This will update every element in the matched set. You can also specify multiple properties in the same method using object literal notation. For example:

`$(‘li’).css(‘background-color’, ‘#272727’);`

To set a value in pixels, do:

`$(‘li’).css(‘padding-left’, ‘+=20’);`

Working with each element in a selection: `.each()` allows you to perform one or more statements on each of the items in the selection of elements that is returned by a selector, like a loop. this or `$(this)` uses the this keyword to create a new jQuery selection containing the current element. It allows you to use jQuery methods on the current element.

## Event Methods

JQuery provides an efficient way to handle events. Events occur when the user performs an action, such as clicking an element, moving the mouse, or submitting a form. When an event occurs on a target element, a handler function is executed.



<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
