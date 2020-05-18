# CSS & Layouts :

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

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
