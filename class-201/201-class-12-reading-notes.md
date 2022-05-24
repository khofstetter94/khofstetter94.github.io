# Chart.js, Canvas

- [Easily Create Stunning Animated Charts with Chart.JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

- [Basic Usage of Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

- [Drawing Shapes with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

- [Applying Styles and Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

- [Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

## Setting Up

        <html lang="en">
            <head>
                <meta charset="utf-8" />
                <title>Chart.js demo</title>
                <script src='Chart.min.js'></script>
            </head>
            <body>
            </body>
        </html>

- You will need a 'canvas' (opening and closing) element with an 'id', 'width', and 'height' attributes. Followed by script that includes variables with all the data and styling

- **Fallback Content** - needed for older browsers that dont support the 'canvas' element. Insert the alternate content inside the 'canvas' element

- **The rendering context** - the 'canvas' elements has a method called '.getContext()' use to obtain the rendering context and its drawing functions. Takes on parameter for the type of context. Retrieve the node in the DOM representing the 'canvas' element by calling the 'document.getElementById()'

## Drawing Shapes with Canvas

- **Rectangles** - these functions draw rectangles:

        fillRect(x, y, width, height)

        strokeRect(x, y, width, height)

        clearRect(x, y, width, height)

- **Drawing Paths** - A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. First create the path, then use drawing commands, then stroke or fill the path to render it. Here are the functions used to perform these steps:

        beginPath()

        closePath()

        stroke()

        fill()

- **Moving the Pen** - 'moveTo()' kinda like lifting a pen or pencil from one spot on a piece of paper and placing it on the next. Use coordinates specified by 2 parameters

- **Lines** - Use 'lineTo(x, y)' Draws a line from the current drawing position to the position specified by x and y

- **Arcs** - Use 'arc(x, y, radius, startAngle, endAngle, counterclockwise)' and 'arcTo(x1, y1, x2, y2, radius)'

- **Bezier and quadratic curves** - Use 'quadraticCurveTo(cp1x, cp1y, x, y)' and 'bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)'

## Applying styles and colors

- **Colors** - two important properties we can use: fillStyle and strokeStyle

- **Transparency** - This is done by either setting the globalAlpha property (globalAlpha = transparencyValue) or by assigning a semi-transparent color to the stroke and/or fill style

- **Line Styles** - several properties which allow us to style lines:

        lineWidth = value

        lineCap = type, with values 'butt', 'round', and 'square'

        lineJoin = type, with values 'round', 'bevel', 'and miter'

        miterLimit = value

        getLineDash()

        setLineDash(segments)

        lineDashOffset = value

- **Gradients** - We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.

        createLinearGradient(x1, y1, x2, y2)

        createRadialGradient(x1, y1, r1, x2, y2, r2)

        createConicGradient(angle, x, y)

- **Patterns** - Use 'createPattern(image, type)', with the type specifying how to use the image in order to create the pattern, use one of these values: repeat, repeat-x, repeat-y, no-repeat

- **Shadows** - Four properties:

        shadowOffsetX = float

        shadowOffsetY = float

        shadowBlur = float

        shadowColor = color

## Drawing Text

- Two methods to render text:

        fillText(text, x, y [, maxWidth])

        strokeText(text, x, y [, maxWidth])

- **Styling Text** - Properties to let you adjust the way the text gets displayed on the canvas:

        font = value

        textAlign = value

        textBaseline = value

        direction = value

- **Advanced text measurements** - 'measureText()' allows you to measure text, returns a TextMetrics object with width in pixels

[Return home](https://khofstetter94.github.io/reading-notes/)
