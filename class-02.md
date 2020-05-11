## Fast Intro:
As we mention previosly in **HTML topic** there is alot of tags in HTML.. (if you had no idea what im talking about go check this *previuos topic* **[HERE](https://3madov-77.github.io/learning-journal/HTML)**),

So today we are gona meat some of others tags of tags family.. :)

<br>

- ### Headings Tags:
HTML has six "levels" of headings from biger to smaler header:
**`<h1>, <h2>, <h3>, <h4>, <h5>, <h6>`**

- ### Paragraphs :
To create a paragraph, surround the words that make up the paragraph with an opening `<p>` tag and closing `</p>` tag

- ### Bold & Italic :
By enclosing words in the tags `<b>` and `</b>` we can make characters appear bold
and By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic

> Evrey HTML editor has 2 views of the page: - visual view  and  - code view 

- ### Superscript & Subscript :
`<sup>` wich used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts
`<sub>` witch used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas

- ### Line Breaks & Horizontal Rules :
Use `<br />` to add Line Breaks and `<hr />` to add Horizontal Rules

- ### Strong & Emphasis :
By default, browsers will show the contents of a `<strong>` element in bold
also will show the contents of an `<em>` element in italic

- ### Quotations :
1. `<blockquote>` :witch used for longer quotes that take up an entire paragraph
2. `<q>` :witch used for shorter quotes that sit within a paragraph

- ### Abbreviations & Acronyms :
use `<abbr> or <dfn>` to acronym, or abbreviation the pargraph you want

- ### Citations & Definitions :
use `<>` to referencing a piece of work and indicate where the citation is from

> The Semantic Markup is: text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages

- ### Auth or Details :
you can use `<address>` tag to  to contain contact details for the author of
the page and the result will be like :

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture02-1.PNG)

- ### Changes to Content :
use `<ins> and <del>` to show content that has been inserted into a document, while `<del>` element can show text that has been deleted from it
also use `<s>` to indicates something that is no longer accurate

<br>

now lets change the subject to the other side of webpage the:

# CSS :

## What is **CSS** :
stylin languge that alows you to create rules that control the way that each elment will look like in browser after rendering, **It** depends basicly on **HTML** so you cant just have CSS without HTML page first, consisting of tow parts:
- ***A selector:*** witch mean the elment witch we should give it the ruls and must look like `p {` and there is many kinds of like:

     ![CAP](https://3madov-77.github.io/learning-journal/New%20folder/Capture-1a.PNG)
 
- ***A declaration:*** witch mean the rules section witch refrence to the first part and looks like: `the rule: the property;}`
so CSS declarations always sit inside curly brackets `{}` 

<hr>

## How to write CSS :
so there is three esintals ways to write **CSS** :
## 1. The External Way:
when we write the whole css code in diferint file then link to it in the HTML code inside the tag `<link>`
## 2. The Internal Way:
when you write the **CSS** code inside the same HTML code ***Under*** the Tag `<style>`
## 3. The Inline Way:
when you write only the **CSS** rules in the same element line after attrbute `style="the rule name='the property'"`
<hr>

# Selctors in CSS :
ther is alot of selectors i will mention them in table :

|   Selctor  |   meaning of   | how it looks |
| ---------- |:--------------:| ------------ |
| Universal Selector|Applies to all elements in the document | `* {}` |
| Type Selector|Matches element names |`h1, h2, h3 {}` |
| Cl ass Selector|Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol | `p.note {}` |
| ID Selector|Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol | `#introduction {}` |
| Child Selector|Matches an element that is a direct child of another | `li>a {}` |
| Descendant Selector|Matches an element that is a descendent of another specified element (not just a direct child of that element) | `p a {}` |
| Adjacent Sibling Selector|Matches an element that is the next sibling of another | `h1+p {}` |
| General Sibling Selector|Matches an element that is a sibling of another, although it does not have to be the directly preceding element | `h1~p {}` |

<br>
<br>
<hr>
<br>

# JS :

- ### The STATEMENTS :
as we know before that the **script** : is a series of instructions that a computer can follow one-by-one
Well each of these individual instruction known as a ***statement***

> Always remumber that JS is sensitive for cases so DOCUMENT means something difrent than document

- ### Comments :
always use comments to describe what hapinig in the code so you dont get lost in some point..
and in Js comments looks like `//` in the start of the line, you can also add multi line comments by add `/*`at the begin and `*/` 

## The data that JS support :
JavaScript distinguishes between numbers, strings, true or false and even values and the three data types is:

***1. STRING DATA :*** it used when we worked on any kind of text, and it enclosed within singel or double quotes

***2. NUMERIC DATA :*** witch always used with tasks such as determining the size of the screen, moving the position of an element on a page or tasks that involve counting or calculating sums

***3. BOOLEAN DATA :*** witch simply only mention to tow answrs.. `True` OR `False`

<br>

- ### WHAT IS A VARIABLE?
its kind of container for bits of information that JS needs, variables sometimes contain steps that you want script to rember like: `var x = y*y` + 'this is the cube space' so evry time will mention `X` it will depends witch `y` is and use it had the cube space..
you can assign value to them like: `(the varuble name) = (the value)`, 

***Also it is important to know that there is rules to name variables you have to folwo like:***

1. The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_)
3. You cannot use keywords or reserved words
4. All variables are case sensitive, so score and Score would be different variable names
5. Use a name that describes the kind of information that the variable stores
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word
you can store diferint types of data in variables (**String**, **Intger**, or **Booleans**)

<br>

- ### Arrys And What Is It:
it is a special type of variable that stores a list of values, its helpful when you do not know how many items a list will contain
you can creat **Arrays** by using the **var**keyword followed by the name of
the array it looks like:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture02-2.PNG)

> remember: that the numbering of arrays list starts at **zero**

<br>

- ### EXPRESSIONS :
an evaluates into (results in) a single value, and there are two types of:
- THAT JUST ASSIGN A VALUE TO A VARIABLE (witch the var will be 1 specifc value)
- THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE (when it could be math maybe)

- ### OPERATORS :
it is things relayed to exprissions that they allow programmers to create a single value from one or more values and there is many taypes of like :

![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-7-2a.PNG)

## The mathematical operators in JS :
which you can use with numbers, You may remember some from math class..

![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-7-3a.PNG)

> remeber that is there is performed mathmatical than others (same in math)

<br>
<hr>
<br>

# The Decision Making in JS :
often there is places in script where decisions are made to determine which lines of code to should run next

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture02-3.PNG)

i think the picture explin evreything

<br>

# Evaluating Conditions in opreators:
so simply it mean comparing a Value to other in the script..
the result will be onr of tow (True OR False)

- ### Is Equal To :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-1a.PNG)

witch compares tow values to see if they are the same

- ### Strict Equal to :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-2a.PNG)

witch used to compare two values to cheak that both the data type are same

- ### Is Not Equal To :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-3a.PNG)

witch compares tow values to see if they are the ***Not*** the same

- ### Strict Not Equal To :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-4a.PNG)

witch used to compare two values to cheak that both the data type are ***Not*** the same

- ### Greater Than :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-5a.PNG)

witch cheaks if the numbers on the left is greater than the numbers in the right

- ### Greater Than Or Equal To :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-6a.PNG)

witch cheaks if the numbers on the left is greater or equal the numbers in the right

- ### Less Than :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-7a.PNG)

witch cheaks if the numbers on the left is less than the numbers in the right

- ### Less Than Or Equal To :
![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-8a.PNG)

witch cheaks if the numbers on the left is less or equal the numbers in the right

<br>

# Logical Operators :
whitch alows you compare the results of more than 1 comparison operator

- ### Logical ***AND (`&&`)*** :
it tastes if the both evalute to **true** then the expression returns **true**
if just one of these it returns **false**

- ### Logical ***OR (`||`)*** :
it taset if either expression evaluates to **true** then the expression returns **true**
if the both is **flase** it returns **false**

- ### Logical ***NOT (`!`)*** :
it just takes a single boolean value and inverts it

![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture-8-9a.PNG)

<br>

# the IF .. ELSE Statments :
witch cheacks an condition if it **True** then the first block of coding excuted
but if the condition is **False** then the second block of coding excuted
and you can use it like:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture02-4.PNG)

<br>
<br>
<hr>

**always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
