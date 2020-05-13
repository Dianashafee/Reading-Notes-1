Go Cheak [HTML In Few Lines (Read01)](https://3madov-77.github.io/Reading-Notes/class-01) & [HTML CSS JS In Parm Lines (Read02)](https://3madov-77.github.io/Reading-Notes/class-02) & [lists & Boxes Or Looping (Read03)](https://3madov-77.github.io/Reading-Notes/class-03)
for an intro..

# HTML:

# Links :
***`<a>`***

use `<a>` tag to create clickable link in the page
the structre of the code will be:
`<a href="(the link you want to add)">(the text witch will contain the link)</a>`
you can use linking to navigate inside the website by adding the page name folowed with html like `examble.html` it caled "**Relative URLs**", also try to use words that people might use when searching

<br>

Being more orgnizer is essintal to make your website more profissional, by orgnize files in dirctorys it will give each one an link addres starts withe main file (root file) till the our file (child), also it can all be inside one dir and will called (Grandparent) and goes on....

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-1.PNG)

the link here for 'index.html' of music will be `www.examplearts.com/music/index.html`

## Email Links :
use 'mailto' tool to create a link that starts up the user's email program and addresses an email to a specified email address, you can serch for mailto tool on the web or just write it like:

`<a href="mailto:jon@example.org">Email Jon</a>`

## Opening Links in a New Window :
use `target="_blank"` attrbute after href to let the link start in new tap when it clicked

> its posible to Linking a Specific Part of the "Same Page" or in "Other Page" by add the elemnt id inside `href` tag like: `<a href="#arc_shot">Arc Shot</a><br />`

<br>
<br>
<hr>

# CSS :

As we mwntiond before CSS treats each HTML element as if it is in its own box, This box will either be a block-level box or an inline box

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-2.PNG)

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-3.PNG)

and it may contain elemnts inside..

## Controlling the Position of Elements:
**CSS** allow you to control the layout of a page: 
- Normal flow :witch is Every block-level element appears on a new line like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-4.PNG)
use `position:static` to let the elemnt Normal flow

- Relative positioning :witch will shifting the element to the top, right, bottom, or left of where it would have been placed like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-5.PNG)
use `position:relative` to let the element Relative positioning

- Absolute positioning :witch will taken out of normal flow, simply it ignore the space it would have taken up and look like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-6.PNG)
use `position:absolute` to let the element Absolute positioning

- Fixed Positioning :witch is positions the element in relation to the
browser window, as opposed to the containing element, and it do not affect the position of surrounding elements look like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-7.PNG)
use `position:fixed` to let the element Fixed Positioning

- Floating Elements :witch allows you to take that element out of normal flow and position it to the far left or right of a containing box looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-8.PNG)
use `float` to let the element Floating, also you can use `z-index` witch allows you to difine witch layer this elemnt will be, it only can used with relative, fixed, or absolute positioning boxes
also `float` allows you to **Place Elements Side-by-Side**  eitch can happen by adding the side as value for the float attr...
use `clear` to clear the sides of the box if there any element touchin it and it takes: `right, left, none, both` as values

 You specify the positioning scheme using the position property in CSS

<br>
<br>

# Screen Sizes :
Since computers have been sold to the public, the size of screens has been steadily increasing, This means that some people viewing your site might have 13 inch monitors while others may have 27+ inch monitors, that means you have to keep this in your mined wille design the page

<br>

# Page Sizes :
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide

<br>

# Fixed Width Layouts :
witch do not change size as the user increases or decreases the size of their browser window, Measurements tend to be given in pixels example:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-11.PNG)

> always keep in mind these tips about the advantegs and disadvantegs with **Fixed Width Layouts**

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-9.PNG)

# Liquid Layouts :
witch designs stretch and contract as the user increases or decreases the
size of their browser window, They tend to use percentages example:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-12.PNG)

> always keep in mind these tips about the advantegs and disadvantegs with **Liquid Layouts**

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-10.PNG)

<br>
<br>

***Possible Layouts: 960 Pixel wide, 12 Column Grid***

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture04-13.PNG)

> A Grid-Based Layout Using 960.GS is CSS Framework used to make cooding by CSS more easier 

## Multiple Style Sheets :
use `@import url("the link")` to improt from the link another style sheets and add to your Like: 'Reset.css' .. witch let you reset all defult margins and the paddings before start use your design, `@import` usble in CSS file, you can use `<link>`in html file for the same perpose..

<br>
<br>
<hr>

# JS :

# FUNCTIONS :
simply its bunsh of steps that work step by step to achive goal, and its reusable

## How to creat a Function :
first of all you need to start by calling `function`, then give it a name after space like `function sleep()` *follwd with prentheses, and finly we add the curly braces `function sleep(){}` and betwin them will have the task like `function sleep(){document.write('Heloo world')};`

## Calling a Function :
after creating the function it will stay there wating for call to start, and this happen with only 1 line! by caling the function name folowed with parantheses like: `sleep();`, after excuting the function it will countinue the code at the after the same calling line...

### Function witch need information:
sometimes the function needs specafic information to use in and it will be inside the paranthases acting like varubles only inside the function.. like: `function pluse(x, y){}`, and we must let th last step of the function in this case is to return the varubles like: `function pluse(x, y){(the steps); return x + y}`
and when we call that kind of functions we must to mention the informations value inside the paranthses like: `pluse(5, 6)`

<br>
<br>
<hr>

# Pair Programs :
simply “two heads are better than one”, the pair programs helps you improve the quality of your code produce

## How does it works :
the main idea depends on tow **Props**:
1. Driver :
is the programmer who is typing codes, Handling the “mechanics” of coding, manages the text editor, switching files, version control
the programmer also should had skills like: explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves

2. Navigator :
who are uses their words to guide the Driver, thinks about the big picture,what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs

## What Pair Programs provide to you?
- Greater efficiency
- Engaged collaboration
- Learning from fellow students
- More Social skills
- Job interview readiness
- Work environment readiness

<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
