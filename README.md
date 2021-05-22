# Svg workshop & src
## SVG def:

Scalable Vector Graphics







# Usefull Links:

## online svg editors:

- <a href="https://svgedit.netlify.app/editor/index.html">SvgEdit</a>

- <a href="https://vectr.com/">Vectr</a>

## articles:

- <a href="https://flaviocopes.com/svg/">Flavio Svg</a>

# Svg lessons:

### Svg elements:

- text: creates a text element

        The text element adds text. The text can be selected using the mouse. x and y define the starting point of the text

- circle: creates a circle

        Define a circle. cx and cy are the center coordinates, and r is the radius. fill is a common attribute and represents the figure color.

- rect: creates a rectangle

        Defines a rectangle. x, y are the starting coordinates, width and height are self-explanatory.

- line: creates a line

        x1 and y1 define the starting coordinates. x2 and y2 define the ending coordinates. stroke is a common attribute and represents the line color.

- path: create a path between two points

        A path is a sequence of lines and curves. It’s the most powerful tool to draw using SVG, and as such it’s the most complex.

        d contains the directions commands. These commands start with the command name, and a set of coordinates:

        M means Move, it accepts a set of coordinates x, y
        
        L means Line, it accepts a set of coordinates x, y to draw the line to

        H is an Horizontal Line, it only accept an x coordinate

        V is a Vertical Line, it only accept an y coordinate

        Z means Close Path, puts a line back to the start

        A means Arch, it needs a whole tutorial on its own

        Q is a quadratic Bezier curve, again it needs a whole tutorial on its own

- textPath: create a path between two points, and a linked text element

      Adds a text along the shape of a path element.

- polygon: allows to create any kind of polygon

      Draw any random polygon with polygon. points represents a set of x, y coordinates the polygon should link

- g: groups separate elements

      Using the g element you can group multiple elements

- SVG viewport and viewBox
      
      An important attribute is viewBox. It lets you define a new coordinates system inside the SVG canvas.
    
- SVG Symbols

      Symbols let you define an SVG image once, and reuse it in multiple places. This is a great help if you need to reuse an image, and maybe just change a bit some of its properties.

      You do so by adding a symbol element and assigning an id attribute

# other infos

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

