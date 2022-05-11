# HTML Lists, Control Flow with JS, and CSS Box Model

## Lists

- **Types of lists** - Ordered (numbered), unordered (bullet points), and definition lists (terms and definitions)

- **Ordered Lists** - Think of recipes, they need to go in order. Use 'ol' element with each individual list item in an 'il' element. Example:

        <ol>
          <li>Turn on the oven</li>
          <li>Combine all ingredients in the bowl</li>
          <li>Pour mixture into baking pan</li>
          <li>Bake for 15 minutes</li>
        </ol>

- **Unordered Lists** - Think of a packing list, the order doesnt matter. Use 'ul' element with each individual item in an 'il' element. Example:

        <ul>
          <li>Hiking boots</li>
          <li>Sleeping bag</li>
          <li>Raincoat</li>
        </ul>

- **Definition Lists** - Like a glossary. Use 'dl' element, each word to be defined goes in a 'dt' element and the definition goes in a 'dd' element. Example:

        <dl>
          <dt>Pencil</dt>
          <dd>A writing device made from wood and lead<dd>
          <dt>Pen</dt>
          <dd>A writing device that uses ink</dd>
        </dl>

- **Nested Lists** - Add a list under a list item by following the ordered or unordered list steps below an existing list item but indented

## Boxes

- **Dimensions** - Change the width and height using pixels, percentages, or ems. Example:

        p {
          height:300px;
          width:300px;
        }

- **Limiting width** - with different screen sizes being a variable, add a min-width and max-width to keep your content legible

- **Limiting height** - Same goes for the height, add a min-height and max-height

- **Overflowing content** - If the content is too big for the space it is in, you can have 'overflow: hidden' (hides the overflow) or 'overflow: scroll' (adds scrollbar)

- **Border, margin, & padding** - Properties of a box to adjust are border (seperates edge of one box to another), margin (creates a gap between two adjacent boxes), padding (space between the box and it's contents)

- **Border width** - control the thickness of a border with pixels or one of the words - thin, medium, thick. 'border-width: 2px;'

- **Border style** - Possible border style properties: solid, dashed, double, groove, ridge, inset, outset, hidden/none

- **Border color** - Use RGB values, hex codes, or CSS color names to change the color of the border. Change each side by speifying which one - 'border-top-color'

- **Border shorthand** - do all this in one property in the order of width, style, color - 'border: 3px dotted red'

- **Padding** - use pixels to say how far the content is from it's box walls, you can also specify individual space by naming the wall in question - 'padding-top', or do shorthand and name all sides in this order - top, right, bottom, left

- **Centering content** - set the left and right margin to 'auto' to center

- **Change Inline/Block** - change inline to block and vice versa with the display property

- **Visibility** - Use the visibility property to hide boxes from users, use 'hidden' to hide and 'visible' to show

- **Box Shadows** - Add shadow to your box with 'box-shadow' with 'horizontal offset', 'vertical offset', 'blur distance', 'spread of shadow'

- **Rounded Corners** - 'border-radius' with the value depicting the size of the radius

- **Elliptical Shapes** - create more complex shapes with different distances of the horizontal and vertical rounded corners. Ex: 'border-radius: 80px 50px;"

- **Type coercion & weak typing** - JavaScript will try to make your unknown data types work rather than send an error. **type coercion** is when JavaScript converts your data type to make it make sense. **weak typing** is what JavaScript uses because the data type values can change.

- **Truthy & Falsey** - Falsey values can be treated as the number 0 and are treated as *if* they are false. Truthy values are treated as 1 or as *if* they are true

- **Short circuit values** - logical operators stop procesessing when they find a result and they return that value - however the value may not be boolean because they could have been truthy or falsey

- **Loops** - To check a condition, the code block will be run through until a 'false' value is returned. Three loops, 'for', 'while', do while'

- **For loops** - The condition usually has a counter that will tell how many times the loop should run

- **While loop** - unsure how long the code should run? This loop will run until teh condition is false

- **Do while loop** - similar to the 'while' loop, but will run the statement in the curly brackets at least once even if the condition ends up false

- **Loop Counters** - require initialization (create a variable 'i' and set it to 0), condition (tell to the loop to run until the counter reaches a specific number 'i<10) and update (everytime the loop runs the statement in the curly braces, it adds one to the counter 'i++')

[Return home](https://khofstetter94.github.io/reading-notes/)
