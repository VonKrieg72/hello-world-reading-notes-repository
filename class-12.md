# Chart.js, Canvas

## Create Stunning Animated Charts with chart.js

Instead of using tables to display data, Charts may be a better option to use. Charts convey data quickly, and are easier to look at; however, they may not be easier to create in some instances. You can start by downloading chart.js, and import the script onto a newly created HTML page. After doing this you can start drawing a line chart, by creating a canvas element in you HTML chart.js can draw the chart. Then you will need to write a script that will retrieve the context of the canvas. You can add this part to the foot of your body element. Within the script tags you can start creating your data. Chart.js is a very great tool to have at your disposal. It is easy to use, and offer great flexibility. *(Vieira, Sara, “Easily Create Stunning Animated Charts With Chart.js”, 2013 NOV 04)*


## Basic usage of canvas

When using the **< canvas >** element it is important to note that it looks similar to the < img >  except there is no src attribute, and no alt attribute, instead the canvas element uses width and height attributes. These attributes are optional and can be set using DOM properties. If you don’t include a height and width attribute within your < canvas > element, then by default it will be 300 pixels wide and 150 pixels high. You also have the ability to change the size using CSS; however, be aware that if the sizing doesn’t respect the ration of the initial canvas, it will appear distorted.

The **< canvas >** element also has the ability to have the **id** attribute applied to it, which is a universal attribute. It is always a good idea to include the id attribute, because it will make it easier to identify in the script. 

Just like you can do with the < video >, < audio >, and < picture > elements, with the < canvas > element you can define some fallback content, to be displayed in older browsers not supporting it, such as versions of Internet Explorer, which are older than version 9 . It is always a good idea to provide fallback content to be displayed by those browsers. *(Mozilla and individual contributors, “Basic usage of canvas”, 2005-2021)*


## Drawing Shapes with Canvas (rectangles, triangles, lines, arcs, and curves)

The canvas grid is called the **coordinate space.** In normal use, 1 unit in the grid corresponds to 1 pixel on the canvas. The origin or starting point of this grid is in the top left corner of the coordinate(0,0), and all of the elements are placed relative to this origin. 

In order to draw a rectangle on canvas, you have a choice of three functions to do so. 

**fillRect (x, y, width, height)** - this draws a filled rectangle

**strokeRect (x, y, width, height)** - this draws a rectangular outline

**clearRect (x, y, width, height)** - this clears the specified rectangular area, making it fully transparent

In order to draw a triangle, the code would look like…

Function draw ( ) {
Var canvas = document. getElementById(‘canvas’);
If (canvas. getContext) {
Var ctx = canvas. getContext(‘2d’);

ctx.beginPath( );
ctx.moveTo(75, 50)
ctx.lineTo(100, 75)
ctx.lineTo(100, 25)
ctx.fill( );
  }
}

In order to draw a line you would use the **lineTo( )** method. 

**lineTo(x, y)** - this method draws a line from the current drawing position to the position specified by x and y.


In order to draw arcs or circles, you use the **arc( )** or **arcTo( )** methods.

**arc(x, y, radius, startAngle, endAngle, conterclockwise)** - this draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by counterclockwise (defaulting to clockwise).

**arcTo(x1, y1, x2, y2, radius)** - this draws an arc with the given control points and radius, connected to the previous point by a straight line. 


In order to draw complex organic shapes you would want to use **Bezier curves.**

**quadraticCurveTo(cplx, cply, x, y)** - this draws a quadratic Bezier curve from the current pen position to the end point specified by x and y, using the control point specified by cplx and cply.

**bezierCurveTo(cplx, cply, cp2x, cp2y, x, y)** - this draws a cubic Bezier curve from the current pen position to the end point specified by x and y, using the control points specified by (cplx, cply) and (cp2x, cp2y).

*(Mozilla and individual contributors, “Drawing shapes with canvas”, 2005-2021)*


## Applying Styles and Colors

In order to apply color to a shape, you are able to use fillStyle and strokeStyle.

**fillStyle = color** - this sets the style used when filling shapes

**strokeStyle = color** this sets the style for the shapes outlines

You also have the ability to draw semi-transparent (translucent) shapes. You can use the **globalAlpha** property in order to to do this.

**globalAlpha = transparencyValue** - this applies the specified transparency value to all future shapes drawn on the canvas the value must be between 0.0, which is fully transparent, and 1.0, which is fully opaque.

*(Mozilla and individual contributors, “Applying styles and colors”, 2005-2021)*


## Drawing text

**fillText (text, x, y, [ , maxWidth])** - this fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

**strokeText (text, x, y [ , maxWidth])** Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

In regards to font, there are additional properties, which enable you to adjust the way the text gets displayed on the canvas.

**font = value** -this string uses the same syntax as the CSS font property. The default font is 10px sans-serif

**textAlign = value** - the text alignment setting. The possible values are start, end, left, right or center. The default value is start.

**textBaseline = value** - possible values include top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

**direction = value** - possible values are qtr, rtf, inherit. The default value is inherit. 

*(Mozilla and individual contributors, “Drawing text”, 2005-2021)*

