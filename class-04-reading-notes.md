# Introduction to HTML - Reading Notes

Read the full blogs:

[Wireframe and Design](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)

[Mozilla HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)

[Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)

## Wireframe and Design

**What is a wireframe?**
A wireframe is basically an architectural blueprint for you website or app. A two-dimensional skeletal outline that lays out how you want the information to be processed by the user.

- Use pen and paper to make changes easily along the way and during early discussions
- Paper prototypes make making changes easier and therefore cheaper
- Switching to software afterwards lets you keep track of detailed decisions

There are many ways to go from design to implementation - it all depends on the project and the user.

Tools for wireframing include pen and paper or free online tools such as UXPin, InVision, or Wireframe.cc

### Six Steps to Make a Wireframe

1. Research - who is your audience, detail requirements, creating user personas, defining use cases, competitor and industry competition
2. Prepare your research for quick reference - make a cheatsheet with your business goals and user goals, your personas, use cases, and cool features found along the way
3. Map out your user flow - provide good information architecture to make moving through the site less frustrating for the user
4. Draft, don't draw. Sketch, don't illustrate - don't get fancy, just create the bare bones for now.
5. Add some detail and get testing - you have the skeleton, now start adding the tendons and ligaments. Consider usability conventions, simple-instructional wording, trust building elements, and tool tips to indicate functionality
6. Start turning your wireframe into a prototype - tools like Pronto.io, Adobe XD, Framer, Sketch (very popular), or Figma to start developing your high-fidelity prototype. Use InVision to interlink screens for the second round of testing

### Three Key Principles

1. Clarity - answer the questions and achieve the goals
2. Confidence - easy to navigate and clear calls-to-action = confidence
3. Simplicity - Don't over do it, too many distractions = the inability to achieve goals

## Mozilla HTML Basics

HTML stands for HyperText Markup Language - it is the coe that is used to structure a webpage and its content.

Wrap content in tags to change the way they appear and behave on the website

**An HTML element** is composed of an opening tag, a closing tag, and the content.

- **opening tag** - contains the name of the element wrapped in opening and closing angle brackets.
- **closing tag** - the same as the opening tag but has a forward slash before the element in order to end it.
- **content** - the content of the element, which is commonly text

**Attributes** add extra information to the element but do not appear in the content. They can have a name and a value. The attribute 'class="editor-note"' gives the element a label so that you can easily find it later. Attritbutes should have:

- A space between it and the element name
- The attritbute name followed by an equal sign
- The attribute value wrapped by opening and closing quotation marks

**Nesting elements** means you have an element inside an element. Be sure to close the elements from the inside out, do not overlap tags.

**Empty elements** have no content and no closing tag. An empty element doesnt wrap content to affect it. Placing an image into your website requires an empty image element with attributes of information about the image.

### Anatomy of an HTML Document

    <!DOCTYPE html>
    <html>
      <head>
        <meta charset="utf-8">
        <title>My test page</title>
      </head>
      <body>
        <img src="images/firefox-icon.png" alt="My test image">
      </body>
    </html>

Above is an example of the beginning of a basic website. Let's break it down:

- The **doctype** are just needed to make sure the document behaves properly
- The **HTML** element warps all the content on the entire page
- The **head** element includes information about the website that isnt the main content of the page's viewers
- The **meta charset** element sets the character set to UTF-8 which has the characters of almost all languages
- The **title** element sets the title of your page - to be seen in the brower tab, and when bookmarked
- The **body** element contains all the main content of the page

### Images

    <img src="" alt="">

This empty element will place and image in the position it appears. It has a src (source) attritbute that has the path to the file and an alt (alternative) attribute that describes the image. Alternative text provides the information for screen readers as well as explains what should be there if the photo doesnt display properly.

### Headings

HTML has 6 levels of headings with the most important being number 1.

    <h1>My Main Title</h1>
    <h2>My Top Level Heading</h2>
    <h3>My Subheading</h3>
    <h4>My Sub-subheading</h4>

*NOTE* you can add a comment in your HTML code that wont appear on the page by writing text between

    <!-- and -->

### Paragraphs

Create paragraphs by wrapping each individual paragraph in this element:

    <p>This is a single paragraph</p>

### Lists

1. Unordered lists are for lists where the order doesnt matter
2. Ordered lists are for lists where the order matters
3. Add items in the list by wrapping each one in this element:

### Links

Links are very very important when creating a website! You can make any text a link to another page by following these steps:

    <a href="">click here</a>

1. Choose text to make a link - ex: 'click here'
2. Wrap it in an 'a' element
3. Add an href attribute
4. Make the value of the href the web address that you want the link to lead to

## Semantics

The *meaning* of the code. A level one heading holds weight of importance in HTML, you can make a font size as big as you want but the most important heading on your page will always be between h1 tags.

What are the benefits of semantic markup?

- Search engines will see important keywords which will influence search rankings
- Screen readers use it to help the visually impaired understand a page
- Finding meaningful blocks of code is easier than searching through endless div's
- Suggests to the developer the type of data that will be populated
- Semantic naming mirrors proper custom element/component naming

Examples of semantic elements:

    <article>
    <aside>
    <details>
    <figcaption>
    <footer>
    <header>
    <main>

[Return home](https://khofstetter94.github.io/reading-notes/)
