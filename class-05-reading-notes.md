# Design web pages with CSS

Click these links to view the full blogs:

- [What is CSS?](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS)
- [How To Add CSS](https://www.w3schools.com/css/css_howto.asp)
- [CSS Color Property](https://www.w3schools.com/cssref/pr_text_color.asp)
- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
- [CSS Tools: Reset CSS](https://meyerweb.com/eric/tools/css/reset/)

## What is CC?

CCS stands for Cascading Style Sheets and is a language that specifies how documents are presented to users - how they are styled, laid out, etc.

A **document** is a text file structured with a markup language like HTML

**Presenting** a document means concerting into a form usable by your audience - with browsers

## CSS Syntax

CSS is a rule-based language and you create the rules. Create each rule with:

- A **selector** which selects the HTML element that will be styled
- Add curly braces
- Inside the braces, add **declarations** which include **property** and **value** pairs. For example: color (property): red (value)

**CSS Modules** - Since there are so many things you can styl with CSS, the language is broken down into modules. You will see reference to these modules as you explore MDN.

**CSS Specifications** - All web standard technologies are defined in giant docuements called specifications, which are published by standards organizations and define how those technologies behave. CSS is developed by a group within W3C.

**Browser Support Information** - Browers have to implement features after they have been specified. Check the browser support status on the MDN CSS propery page under "Browser compatibility" to see if the property can be used on your website.

## How to Add CSS

Three ways to insert CSS:

- External CSS
- Internal CSS
- Inline CSS

**External CSS** - change the look of an entire website by changing only one file! Refer to the external sheet inside the 'link' element inside the head section. Must be saved with a .css extension and does not contain any HTML tags.

    <!DOCTYPE html>
      <html>
        <head>
          <link rel="stylesheet" href="mystyle.css">
        </head>
        <body>
          <h1>This is a heading</h1>
          <p>This is a paragraph.</p>
        </body>
      </html>

**Internal CSS** - Used if one HTML page has a unique style. Defined inside the 'style' element inside the head section.

    <!DOCTYPE html>
      <html>
        <head>
          <style>
            body {
              background-color: linen;
            }

            h1 {
              color: maroon;
              margin-left: 40px;
            }
          </style>
        </head>
        <body>

          <h1>This is a heading</h1>
          <p>This is a paragraph.</p>

        </body>
      </html>

**Inline CSS** - used to apply unique style for a single element. Add the style attribute to the relevent element.

    <!DOCTYPE html>
      <html>
        <body>

          <h1 style="color:blue;text-align:center;">This is a heading</h1>
          <p style="color:red;">This is a paragraph.</p>

        </body>
      </html>

**Multiple style sheets** - if multiple sheets give a different value to the same property, the last read style will be used.

**Cascading order** - when more than one style is specified for an element, Following the priority of:

1. Inline
2. External and Internal
3. Browser default

## CSS color property

The **color** property specifies the color of the text.

**CSS syntax** color: color|initial|inherit;

**Property Values** - *color* specifies the text color. *Initial* sets the this property to its default value. *Inherit* inherits this property from its parent element.

Click the link for "CSS Reference" as the top of this page for access to an index of property names for CSS

[Return home](https://khofstetter94.github.io/reading-notes/)
