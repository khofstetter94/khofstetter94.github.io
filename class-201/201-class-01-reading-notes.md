# Duckett HTML

Notes taken from:

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc. .

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

Ways to access the web:

- Browsers - software like Chrome or Firefox that allows browsing with web addresses and links
- Web servers - hosts the website, sends out web pages to users when prompted
- Devices - such as laptops, phones, tablets, all of which are unique in size and connections
- Screen readers - programs that read out what on the computer screen, making the web more accesible

## Structure

- use headings, sub headings, sections, quotes, ect to structure your webpage in order for it to br easier to navigate
- use HTMl tags to add meaning to text on your webpage - the tags are like containers
- **elements** have an opening and a closing tag with content between
- **attributes** give more information about the element. They are in the opening tag.

- The **body** element will house all the information to be viewed on the page
- The **head** element will house information about the page that will not be seen
- The **title** element resides within the head and gives your web page a name on the tab

## Extra Markup

- **DOCTYPE** declares what language the webpage is using
- Add comments throughout your code that wont be seen on the web page by writing it within these characters:

        <!--  -->

- Add **ID attributes** to make each element unique in order to manipulate them individually with CSS
- Add a **Class attribute** to manipulate many different elements under one class with CSS
- **Block elements** include h1, p, ul, and li - and they will start on a new line
- **Inline elements** appear on the same line as their neighboring elements
- Group elements together with the **'div'** element
- Group elements inline together with the **'span'** element - this also helps to add an ID or class to text inline to be altered with CSS later
- Create an iframe - or a window into another site -- with the 'iframe' tags, within the tags add the source, height, width, scrolling, framebar, and seamless
- Add a **meta** element to add information about the page that will not be seen. Add a description og the page, keywords, author, pragma, expires, robots.
- Use **escape characters** to make html code characters appear on the page.

## HTML5 Layout

- Rather than a ton of 'div' elements with unique IDs, the new set of elements say exactly what you will find within them
- Common HTML5 elements include: header, footer, nav, article, aside, section, hgroup, figure, figcaption, div
- Make an entire block into a link by wrapping it in an 'a' element
- Make sure to tell old browsers which elements are block-level elements

## Process & Design

- Think logistically about your target audience and design your webpage to meet their needs
- Consider their motivations for coming to your page and their goals once they get there
- Consider their goals and possible questions and be sure to provide their answers
- Depending on your topic, update your website as often as new information is required. Daily news sites need updatating daily, while websites that provide a service need updating as specials/deals/rates/ect change
- Group related pieces of information together and create a **site map** that moves the user along towards their goal. Use size, color, and style to direct the user's eyes
- Create a **wireframe** to create a plain black and white outline of your site - focus on importance of details and inclusion of everything necessary to navigate your site
- Consider a visual hierarchy that instinctly moves the user where you would like their focus
- Group related pieces of information together visually with - proximity, closure, continuance, white space, color, and borders
- Provide navigation by being consise, clear, and selective. Provide context, make it interative, and be consistent

## Duckett JS: The ABC of Programming

- A **script** is basically a set of instructions that your computer will follow to accomplish your goal
- Define the goal, design the script, code each step
- Remember that computers solve problems programmatically, one step after the other
- **Flowcharts** visually respresent the flow of the steps and how they lead to one another, sometimes one path may lead to a different step entirely

- Computers need to be told exactly what is on the page, define the objects, differentiate their types, determine their properties (or characteristics), distinguish each property's name and value
- **Events** are when the user interacts with the computer which in turn triggers different functionalities
- **Methods** are like questions and instructions that tell you someting about that object or change the value of one or more of that objects properties

- Three languages are used to create a web page - HTML (the content), CSS (the presentation), and JavaScript (the behavior)
Keep JavaScript in it's own file
- use the HTMl element 'script' to use JavaScript with a web page
- JavaScript will run wherever it is found in the HTML

[Return home](https://khofstetter94.github.io/reading-notes/)
