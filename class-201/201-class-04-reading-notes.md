# HTML Links, JS functions, and Intro to CSS Layout

Notes taken from:

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc. .

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

- Grampa, A. (2018, August 24). 6 Reasons for Pair Programming [web log]. Retrieved May 12, 2022, from <https://www.codefellows.org/blog/6-reasons-for-pair-programming/>.

## Links

- **Writing links** - Written between 'a' tags with the URL being an **'href'**attribute inside the opening tag

        <a href="https://github.com/khofstetter94">My Git Hub</a>

- **Relative URL** - used to link to a page within the same site. You do not need to specify the domain name in the URL. Helpful when just starting to create a website, quicker to write too. If you need to link to a page within the same folder, just use the file name 'filename.html'. For a child folder, 'childfolder/filename.html'. For a grandchild folder, 'childfolder/grandchildfolder/filename.html', for a parent folder, '../index.html', for grandparent folder, '../../index/html

- **Directory Structure** - Put the pages for each different section of the site in its own folder. The top level folder is known as the **root** folder. If the root folder has other folders inside of it, then the root folder is the **parent** and the indide folders are **children**, folders inside the children would be **grandchildren** of the root. Every homepage of every site is called 'index.html' and is the default page

- **Email Links** - link to start the user's email program and address an email to a specified email address:

        <a href="mailto:john@example.org">Email John</a>

- **Open in New Window** - to open the link in a new window include 'target="_blank"'

        <a href="https://github.com/khofstetter94" target="_blank">My Git Hub</a>

- **Linking to a different part of the same page** - Add 'id' as an attribute to a header on the page, then in the link to that spot - add #theIDname as teh 'href' value

        <h1 id="bottom">This is the bottom of the webpage</a>
        <a href="#bottom">Click here to go to the bottom of the webpage</a>

## Layout

- **Building Blocks** - HTML elements are their own box to be manipulated by CSS. **Block-level Elements** are on their own line and **Inline Elements** are surrounded by text

- **Containing Elements** - One block element inside another, the outside one is the containing/parent

- **Positioning schemes** - **normal flow** default behavior, everything is stacked on top of the other down the page. **Relative positioning** shifts to the top, right, bottom, or left of where it would have been. **Absolute positioning** positions the element in relation to its containing element

- **Fixed Positioning** - absolute positioning that sticks the element somewhere in relation to the browser window, doesnt move when scrolling. **Floating elements**  moves an element to the side of it's box, and other content can flow around it

- **Normal Flow** - default in browsers, block-level elements sit on top of the next

- **Relative Positioning** - you can move an element around from what it normally would be, use 'position: relative' then use offset properties 'top: 10px"

- **Absolute Positioning** - taken out of normal flow and doesnt affect other elements, then edited iwth box offset properties

- **Fixed Positioning** - 'position: fixed' glues it to the browser page and stays put when scrolling

- **Oerlapping Elements** - relative, fixed, and absolute positioning make thing overlap, the elements later in the code sit on top, control the stack with 'z-index: #' where the number dictates which goes on top, the higher the number the higher on the stack

- **Floating ELements** - in normal flow, moves the element all the way right or left in it's box so that the other content flows around it

- **Clear Floats** - clear property says no element may touch the left/right/both/none sides of a box

- **Multi-Column layouts** - use 'width', 'float', 'margin' to have two side by side columns

- Due to differing sizes in screens, consider how your webpage will look on different screens. A **fixed layout** does not change size as the user increased or decreases the size of their browser. **Liquid layouts** stretch as the user increases or decreases the browser size.

- **Grids** - in order to layout your webpage professionally and with consistency, consider the **960 pixel grid** that provides thick vertical evenly spaced lines to base your boxes off of

- **Multiple style sheets** - utilize several CSS style sheets if it makes organizational sense to you, then either link one to your HTML and then use @import rule to import the other sheets to the first sheet. OR use separate link elements for each style sheet

## Functions, Methods, & Objects

- **Functions** - group multiple statements together for a task, can be reused. Functions need a name which will be used to **call** it (envoke it), **parameters** are required pieces of infomration that the function needs to perform a given task (these would go in the parenthesis after the name, then used again as values or variables in the code block), the **return value** is the expected answer or result from the task.

        function functionName() {
          code block for task;
        }

- Calling a function - executing the the statements

        functionName();

- Use the **return** keyword to return the result of the function to the code that called it. Return more than one value with and **array**

- **Function Expression** - if the function is placed where an expression would normally be, then it is a function expression. Similiar to regular functions but with no name. You could declare a variable to be a function

- **Immediately invoked funtion expressions (IIFE)** - executed once as the interpreter comes across them. The declared variable will hold rather the store the returned value. Add a final set of parentheses between the closing curly brace and the closing expression parentheses

- **Variable Scope** - involved the location of a declared variable and where it can be used. **Local varioables** are declared inside a function and therefore can only be in that function, these usually have a return so that the value can be removed and a different set of parameters can be used. **Global variables** are outside the function and can be used anywhere in the script

- **6 Reasons for Pair Programming**

- This is where two developers share a workstation to complete a task together

- **Driver** is the person actually writing the code and the **navigator** is guiding them with only words. Work on the skills for listening, speaking, reading, and writing.

- The 6 reasons:

  - Greater efficiency - two sets of eyes are better than one, catch mistakes bett
  - Engaged collaboration - you're less likely to get distracted if someone else is there to hold you accountable
  - Learning from fellow students - everyone learns and creates differently, you could learn new techniques you hadn't thought of
  - Social skilles - working with someone else can cause conflict, its a skill to find composure and use your words
  - Job interview readiness - this kind of teamwork excercise if used in interviews, typically with the interviewee and an employee
  - Work environment readiness - this type of work is expected in tech companies, so this prepares you to hit the work force confidently

[Return home](https://khofstetter94.github.io/reading-notes/)
