# Forms and JS Events

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc. .

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

## Forms

- **Form controls** - ways to collect info from users: adding text, making choices, submitting forms, uploading files
  -input gets sent to the server as name/value pairs

- **Form Structure** - the 'form' element, includes an 'action' attribute, usually includes a method and id attribute

- **Text Input** - using the 'input' element, including 'type=text', 'name', 'size', and 'maxlength' attributes

- **Password Input** - using the 'input' element, includes 'type="passowrd"', 'name', 'size', and 'maxlength'

- **Text area** - 'textarea' element used for multi line text input

- **Radio button** - 'input' element, needs attributes - 'type="radio"', 'value', 'checked'

- **Checkbox** - 'input' element, with attributes 'name', 'value', and 'checked'

- **Drop Down List Box** - 'select' element with 'name' attribute, followed by 'option' elements with a 'value' attribute, use the 'selected' attribute to indicate the option that should be selected when the page loads

- **Mulitple select box** - 'select' elements with attributes 'name' and 'multiple' for multiple options

- **File Input box** - 'input' element with 'type="file"', use this if you want a user to upload a file

- **Submit button** - 'input' element with 'type="submit"', 'name', and 'value' attributes

- **Image button** - 'input' element with 'type="image"' attribute and then your typical image attributes like height and width

- **Button & Hidden Controls** - 'button' element. Have an 'input' element with 'type="hidden"' for hidden form controls

- **Labelling form controls** - 'label' element for each form control to make the form more accesible, include a 'for' attribute

- **Grouping form elements** - 'fieldset' to group related form controls together, and use 'legend' to label the grouped together controls

- **HTML5: Date Input** - 'input' element with 'type="date"'

- **HTML5: Email & URL input** - 'input' element with 'type="email"' or 'type="url"'

- **HTML5: Search Input** - 'input' element with 'type="search"', use 'placeholder' attribute to have writing existing in the search field

## Lists, Tables, and Forms

- **Bullet point styles** - change the bullet point shape with **'list-style-type'** under the CSS for that list, use **'list-style-image'** to use an image for the bullet point

- **Position the marker** - use 'list-style-position' and choose either 'outside' or 'inside' to have the bullet sit inside or outside the text

- **Styling Tables** - Use properties including: witdh, padding, text-transform, letter-spacing, font-size, border-top, border-bottom, text-align, background-color, :hover. For emppty cells, decide if the border should be there with 'empty-cells' with either 'show, 'hide', or 'inherit'. Control the gaps between cells with 'border-spacing' and 'border-collapse'

- **Styling forms** - style the text inputs and text areas, submit buttons, labels... you can add a 'background-image' to the input fields, for submit buttons try 'text-shadow' and ':hover'. For fieldsets and legends, consider width, color, background color, border, padding.

- **Cursor styles** - use the'cursor' property and include values like auto, crosshair, default, pointer, move, text, wait, help, url("cursor.gif")

## Events

- Events occur and trigger functions in the JavaScript code

- **Event handling** - when a user interacts with the HTML on a webpage, three steps are involved in getting it to trigger JavaScript code: select the element node you want the script to respond to, indicate which event on the selected node will trigger the response, and state the code you want to run when the event occcurs

- **Bind an event to an element** - three ways: HTML event handlers (now considered bad practice), traditional DOM event handlers, DOM level 2 event listeners

- **Event listeners** - can handle more than one function at a time but they are not supported in older browsers

- **Event flow** - HTML elements nest inside other elements. If you hover or click on a link, you will also be hovering or clicking on its parent elements

- **The event object** - when an event occurs, the event object tells you information about the event, and the element it happened upon

- **Event Delegation** - Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element

- **Different types of events** - W3C DOM events (most commonly used), HTML5 events, and BOM events

- **Common Events** - Load, focus and & events, mouse events, click, keyboard events, form events, mutation events and obervers, HTML5 events

- **Where events occur** - The event object can tell you where the cursor was positioned when an event was triggered

[Return home](https://khofstetter94.github.io/reading-notes/)
