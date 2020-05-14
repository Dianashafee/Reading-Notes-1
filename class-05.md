Go Cheak [HTML In Few Lines (Read01)](https://3madov-77.github.io/Reading-Notes/class-01) & [HTML CSS JS In Parm Lines (Read02)](https://3madov-77.github.io/Reading-Notes/class-02) & [lists & Boxes Or Looping (Read03)](https://3madov-77.github.io/Reading-Notes/class-03) & [Links, Layouts and Functions (Read4)](https://3madov-77.github.io/Reading-Notes/class-04)
for an intro..

<br>
<br>

# CSS

<br>

# Images :
images is one of the most important thing in the webpag, as they say *A picture can say a thousand words* so try to be carefull when you **Choosing Images for Your Site**, and slways remember Images should be:
> relevant, Convey information, Convey the right mood, instantly recognisable, and Fit the color palette

## How to add images :
usualy we use `<img>` tag in HTML with 'href="the link"' OR 'src="parent/thefile.jpg"' attrbutes also there's 'alt, title' attr you can use

## Saizing of Images:
actuly there is 2 ways to size the images 
1. in CSS : by using `img{width:25px; height:25px}`
2. in HTML : by only adding `width="25px" height="25px"` as attrbutes in the same `<img` line...

## Images Places In Code :
you can add images where you want to but usualy images add:
- before a paragraph
- inside the start of a paragraph
- in the middle of a paragraph
EX:
![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-1.PNG)

## Rules for Creating Images :
keep in mind thses three important rules:
1. Save images in the right format
2. Save images at the right size
3. Use the correct resolution

## Tools to Edit & Save Images:
There are several tools you can use to edit images like: Adobe Photoshop, Adobe Fireworks, Pixelmator, PaintShop Pro, Paint.net

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-2.PNG)

## Image Formats :
actuly there is many images formats like: `JPEG`, `GIF`, `PNG`, `JPG`

## Image Dimensions :
all images in your website should be saved in the same width and height always you can: **Reducing image size** witch will let image quicker to download, OR **Increasing image size** witch will let image look blurry or blocky, OR **Changing image shape**

## Cropping Images :
you can aways cropping images as you want but remember not to lose a valuble information 

## Image Resolution :
the main resolution of the webpages images should be '72 ppi' but the difrence of the size of the images and the type of it changes that value so It is important to remember that:
Each extra frame or dpi or ppi of the image will increases the size of the file, and can therefore add to the time it takes for an image to download (and web users do not like waiting a long time for images to
download)

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-3.PNG)

<br>
<br>

# Colors :

there is many types of colors like:
1. ## Text colors:
and also there is three ways to specify colors to text :
#### - color names:
witch is the simplest one and it just mention the color name after `color:`

#### - rgb values : 
witch shortcut to (**RED** **GREEN** **BLUE**) and the values for each color start from 0 to 255 and looks like `rgb(22, 33, 44)`

#### - The hex codes :
witch is six digits only start with `#`, and evry color has one

2. ## Background colors :
witch css spuort for each HTML element to had one, you have to secify the color you want or it will be defultly as white color..

3. ## Hue Colors :
Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue

4. ## Saturation colors :
Saturation refers to the amount of gray in a color, At maximum saturation, there would be no gray in the color. At minimum
saturation, the color would be mostly gray

5. ## Brightness colors :
Brightness (or "value") refers to how much black is in a color, At maximum brightness, there would be no black in the color At minimum brightness, the color would be very dark

6. ## Contrast :
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible
<br>

 ![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture1-1b.PNG)

<br>

When text is harder to read, low contrast between background and foreground colors in difernt worlds
<br>

 ![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture1-2b.PNG)

<br>

For long spans of text, reducing the contrast a little bit improves readability
<br>

 ![cap](https://3madov-77.github.io/learning-journal/New%20folder/Capture1-3b.PNG)

<br>

it is easier to read when there is higher contrast between background and foreground colors (some times you can use it If you want people to read a lot of text on your page)
<br>

7. ## The Opacity :
witch is property lows you to specify the opacity of an element, and it should be number betwin 0.0 AND 1.0, it caled alpha value in some css attr like `rgb`

<br>
<br>

# Texts :

## Typeface Terminology :

- Serif :witch has extra details on the ends of the main strokes of the letters and looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-4.PNG)

- Sans-Serif :witch has have straight ends to letters, and more cleaner design and looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-5.PNG)

- Monospace :witch has for every letter the same width and looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-6.PNG)

- Cursive :witch has joining strokes or other cursive characteristics and looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-8.PNG)

- Fantasy :witch has usually decorative fonts and are often used for titles, They're not designed for long bodies of text they looks like: ![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-9.PNG)

## Main structure :

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-7.PNG)

> Remumber when Choosing a Typeface for your Website that browser will only display it if it's installed on that user's computer, like:",Sans Snas-Serif"

## Techniques That Offer a Wider Choice of Typefaces :
There are several ways to use fonts other than those listed typefaces and they are:

1. Font-Family :witch s used to specify the typeface for CSS, and you can use it by using `font-family` property

2. Font-Face :specifies where a font can be downloaded from if it is not installed on the computer

3. Service-based Font-Face :witch give users access to a wider range of fonts using `@font-face` witch take values: "font-family, src, format" 

## Size of Type :
**font-size** :by using `font-size` proparty witch you can define there value with: "pixels, percentages, EMS"

> The default size of text in a browser is 16 pixels

## Units of Type Size :

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-10.PNG)

## Bold :
**font-weight** use `font-weight` atrr and it can take "bold, normal, or numbers" as values

## Italic :
**font-style** use `font-style` atrr and it can take "normal, italic, oblique"

## UpperCase & LowerCase :
**text-transform** use `text-transform` atrr and it can take "uppercase, lowercase, capitalize"

## Underline & rticle :
**text-decoration** use `text-decoration` atrr and it can take "none, underline, overline, line-through, blink"

## Leading :
**line-height** use `line-height` atrr

## Letter & Word Spacing :
**letter-spacing, word-spacing** use `letter-spacing, word-spacing` atrr

## Alignment :
**text-align** use `text-align` atrr and it can take "left, right, center, justify"

## Vertical Alignment
**vertical-align** use `vertical-align` atrr and it can take "baseline, sub, super, top, text-top, middle, bottom, text-bottom"

## Indenting Text
**text-indent** use `text-indent` atrr

## CSS3: Drop Shadow
**text-shadow** use `text-shadow` atrr and valus looks like:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-11.PNG)

## First Letter or Line :
**:first-letter** , **:first-line** :You can specify different values for the first letter or first line of text inside an element using `:first-letter` and `:first-line`

## Styling Links :
**:link** :This allows you to set styles for links that have not yet been visited, **:visited** :This allows you to set styles for links that have been clicked on

Responding to Users :
- **:hover** :applied when a user hovers over an element with a pointing device such as a mouse, This has commonly been used to change the appearance of links and buttons when a user places their cursor over them, 
- **:active** :witch applied when an element is being activated by a user
- **:focus** :witch applied when an element has focus

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-12.PNG)

<br>
<br>

# Attribute Selectors :
ther is a set of attribute selectors that allow you to create rules that apply to elements that have an attribute with a specific value witch is:

![cap](https://3madov-77.github.io/Reading-Notes/Resorses/Capture05-13.PNG)


<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
