# Svg workshop & src
## SVG def:

Scalable Vector Graphics







# Usefull Links:

## online svg editors:

- <a href="https://svgedit.netlify.app/editor/index.html">SvgEdit</a>

- <a href="https://vectr.com/">Vectr</a>

## articles:

- <a href="https://flaviocopes.com/svg/">Flavio Svg</a>
- <a href="https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial"> MDN Svg Full Tutorial </a>

# Svg lessons:

## **Svg elements:**


## ✨ text: 
creates a text element

The text element adds text. The text can be selected using the mouse. x and y define the starting point of the text

```html
<text>
  This is <tspan font-weight="bold" fill="red">bold and red</tspan>
</text>
```
---
## ✨ textPath
This element fetches via its xlink:href attribute an arbitrary path and aligns the characters, that it encircles, along this path:

```html
<path id="my_path" d="M 20,20 C 80,60 100,40 120,20" fill="transparent" />
<text>
  <textPath xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#my_path">
    A curve.
  </textPath>
</text>
```

---
## ✨ circle: creates a circle

Define a circle. cx and cy are the center coordinates, and r is the radius. fill is a common attribute and represents the figure color.

```html
<circle cx="25" cy="75" r="20"/>
```
 Attribute       | Description
 :-------------: |:-------------
r| The `radius` of the circle.
cx | The `x position` of the center of the circle.
cy|The `y position` of the center of the circle.
---

## ✨ Ellipse

```html
<ellipse cx="75" cy="75" rx="20" ry="5"/>
```
 Attribute       | Description
 :-------------: |:-------------
 rx| The `x radius` of the ellipse.
ry| The `y radius` of the ellipse.
cx| The `x position` of the center of the ellipse.
cy| The `y position` of the center of the ellipse.

---
## ✨ rect: creates a rectangle 

Defines a rectangle. x, y are the starting coordinates, width and height are self-explanatory.
```html
<rect x="60" y="10" rx="10" ry="10" width="30" height="30" />
```

| Attribute       | Description|
| :-------------: |:-------------|
| x | The `x` position of the top left corner of the rectangle. | 
| y | The `y` position of the top left corner of the rectangle. |
| width | The `width` of the rectangle |
| height   | The `height` of the rectangle. |
| rx  | The `x radius` of the corners of the rectangle |
| ry  | The `y radius` of the corners of the rectangle |

---

## ✨ line:
 creates a line
```html
<line x1="10" x2="50" y1="110" y2="150"/>
```
| Attribute       | Description|
| :-------------: |:-------------|
x1| The x position of point 1.
y1| The y position of point 1.
x2| The x position of point 2.
y2| The y position of point 2.

---
 
## ✨ Polyline
A polyline is a group of connected straight lines. Since the list of points can get quite long, all the points are included in one attribute
```html
<polyline points="60, 110 65, 120 70, 115 75, 130 80, 125 85, 140 90, 135 95, 150 100, 145"/>
```
| Attribute       | Description|
| :-------------: |:-------------|
points | A list of points. Each number must be separated by a space, comma, EOL, or a line feed character. Each point must contain two numbers: an x coordinate and a y coordinate. So, the list (0,0), (1,1), and (2,2) would be written as 0, 0 1, 1 2, 2.
---

## ✨ polygon: 

A polygon is similar to a polyline, in that it is composed of straight line segments connecting a list of points. For polygons though, the path automatically connects the last point with the first, creating a closed shape.

```html
<polygon points="50, 160 55, 180 70, 180 60, 190 65, 205 50, 195 35, 205 40, 190 30, 180 45, 180"/>
```
| Attribute       | Description|
| :-------------: |:-------------|
points| A list of points, each number separated by a space, comma, EOL, or a line feed character. Each point must contain two numbers: an x coordinate and a y coordinate. So, the list (0,0), (1,1), and (2,2) would be written as 0, 0 1, 1 2, 2. The drawing then closes the path, so a final straight line would be drawn from (2,2) to (0,0).

---

## ✨ path:
A path is the most general shape that can be used in SVG. Using a path element, you can draw rectangles (with or without rounded corners), circles, ellipses, polylines, and polygons. Basically any of the other types of shapes, bezier curves, quadratic curves, and many more.

```html
<path d="M20,230 Q40,205 50,230 T90,230" fill="none" stroke="blue" stroke-width="5"/>
```
A path is a sequence of lines and curves. It’s the most powerful tool to draw using SVG, and as such it’s the most complex.

| Attribute       | Description|
| :-------------: |:-------------|
d | contains the directions commands. These commands start with the command name, and a set of coordinates
M | means Move, it accepts a set of coordinates x, y
L | means Line, it accepts a set of coordinates x, y to draw the line to
H | is an Horizontal Line, it only accept an x coordinate
V | is a Vertical Line, it only accept an y coordinate
Z | means Close Path, puts a line back to the start
A | means Arch, it needs a whole tutorial on its own
Q | is a quadratic Bezier curve, again it needs a whole tutorial on its own

---

## ✨ textPath: 
create a path between two points, and a linked text element

Adds a text along the shape of a path element.

---
## ✨ g:
groups separate elements

Using the g element you can group multiple elements

---

## ✨ SVG viewport and viewBox
      
An important attribute is viewBox. It lets you define a new coordinates system inside the SVG canvas.

---
    
## ✨ SVG Symbols

Symbols let you define an SVG image once, and reuse it in multiple places. This is a great help if you need to reuse an image, and maybe just change a bit some of its properties.

You do so by adding a symbol element and assigning an id attribute

---

# **More infos**

### Inline SVG using a Data URL

You can use any of the above examples combined with Data URLs to inline the SVG in the HTML:

      <img src="data:image/svg+xml;<DATA>" alt="Flag" />

    <object data="data:image/svg+xml;<DATA>" type="image/svg+xml"></object>

    <iframe data="data:image/svg+xml;<DATA>" frameborder="0"></iframe>

and in CSS too:

    .svg-background {
        background-image: url('data:image/svg+xml;<DATA>');
    }


## Svg Css:
    
### svg background color:

    fill: background color;
    fill-opacity: background color opacity
    stroke: defines the border color
    stroke-width: sets the width of the border

