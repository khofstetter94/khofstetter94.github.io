# CSS Layout

- [Layout](https://web.dev/learn/css/layout/)

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

## Layout

- **Display** property determines if the box it is applied to acts as inline or block.
  - **Inline** elements sit side by side
  - **Block** elements create a new line for themselves
  - Display also determines how that element's children will behave

- **Flexbox** - layout mechanism for one-dimensional layouts (single axis). Will align the element's children next to eachother
  - converts the child elements to be flex items so you can write rules on how they behave

- **Grid** is designed to control multi-axis layouts. Write layout rules on an element with 'display: grid'
  - Use grid unit 'fr' which is a fraction of remaining space

- **Flow layout** - if not in grif or flex, then your elements display in **normal** flow
  - Use 'inline-block' to get a box that has some of the characteristics of a block-level element, but still flows inline with text

- **Floats** - allows text to wrap around images (kinda like a newspaper).

- **Multicolumn layout** - put a  long list into multiple columns for better space awareness using: 'column-count' and 'column-gap'

- **Positioning** - changes how an element behaes in the normal flow of the document and how it relates to other elements. 'relative', 'absolute
, 'fixed', 'sticky', with default value 'static'

- **Building Blocks** - HTML elements are their own box to be manipulated by CSS. **Block-level Elements** are on their own line and **Inline Elements** are surrounded by text

- **Containing Elements** - One block element inside another, the outside one is the containing/parent

- **Positioning schemes** - **normal flow** default behavior, everything is stacked on top of the other down the page. **Relative positioning** shifts to the top, right, bottom, or left of where it would have been. **Absolute positioning** positions the element in relation to its containing element

- **Fixed Positioning** - absolute positioning that sticks the element somewhere in relation to the browser window, doesnt move when scrolling. **Floating elements**  moves an element to the side of it's box, and other content can flow around it

- **Normal Flow** - default in browsers, block-level elements sit on top of the next

- **Relative Positioning** - you can move an element around from what it normally would be, use 'position: relative' then use offset properties 'top: 10px"

- **Absolute Positioning** - taken out of normal flow and doesnt affect other elements, then edited with box offset properties

- **Fixed Positioning** - 'position: fixed' glues it to the browser page and stays put when scrolling

- **Overlapping Elements** - relative, fixed, and absolute positioning make thing overlap, the elements later in the code sit on top, control the stack with 'z-index: #' where the number dictates which goes on top, the higher the number the higher on the stack

- **Floating Elements** - in normal flow, moves the element all the way right or left in it's box so that the other content flows around it

- **Clear Floats** - clear property says no element may touch the left/right/both/none sides of a box

- **Multi-Column layouts** - use 'width', 'float', 'margin' to have two side by side columns

- Due to differing sizes in screens, consider how your webpage will look on different screens. A **fixed layout** does not change size as the user increased or decreases the size of their browser. **Liquid layouts** stretch as the user increases or decreases the browser size.

- **Grids** - in order to layout your webpage professionally and with consistency, consider the **960 pixel grid** that provides thick vertical evenly spaced lines to base your boxes off of

- **Multiple style sheets** - utilize several CSS style sheets if it makes organizational sense to you, then either link one to your HTML and then use @import rule to import the other sheets to the first sheet. OR use separate link elements for each style sheet

[Return home](https://khofstetter94.github.io/reading-notes/)
