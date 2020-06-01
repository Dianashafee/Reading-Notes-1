# Chart.js API

witch is better ways to display data, and are easier to look and convey data quickly, Chart.js is a JavaScript plugin that uses the new HTML5 canvas element, to easily draw a graph onto the pages..

# Setting up :
The first thing we need to do is 
- download Chart.js
- Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in
- Then create a new html page and import the script:

`< !DOCTYPE html>
< html lang="en">
    < head>
        < meta charset="utf-8" />
        < title>Chart.js demo</>
        < script src='Chart.min.js'></>
    </ head>
    < body>
    </ body>
</ html>`

# Drawing shapes with canvas:

## Drawing rectangles :

`function draw() {
var canvas = document.getElementById(‘canvas’);
if (canvas.getContext) {
var ctx = canvas.getContext(‘2d’);
ctx.fillRect(25, 25, 100, 100);
ctx.clearRect(45, 45, 60, 60);
ctx.strokeRect(50, 50, 50, 50);} }`

## Drawing paths :
use :

`beginPath()`

`closePath()`

`stroke()`

`fill()`

## Lines:

by useing `lineTo(x, y)`

## Arcs:

`arc(x, y, radius, startAngle, endAngle, anticlockwise)
arcTo(x1, y1, x2, y2, radius)`



<br>
<br>
<hr>


**always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
