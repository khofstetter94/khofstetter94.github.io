# Problem Domain, Objects, and the DOM

- Sonmez, J. (2013, July 15). Understanding The Problem Domain Is The Hardest Part Of Programming [web log]. Retrieved May 15, 2022, from <https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming>.

- Geelhoed, C. (2020, January 16). What’s the Difference Between Primitive Values and Object References in JavaScript? [web log]. Retrieved May 15, 2022, from <https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b>.

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc. .

## The Problem Domain

- Programming is easy if you understands the problem domain
  - Make the problem domain easier
  - Get better at understanding the problem domain
- Cut out cases and narrow your focus to a part of the problem

## Primitive Values vs Object References

- JavaScript 8 data types:
  - Boolean
  - Null
  - Undefined
  - BigInt
  - String
  - Symbol
  - Objects

- **Primitive values" that are assigned to a variable, sets the varaible to that value diectly

- When the variable is assigned to an **object** that variable contains a **reference** to it

- Difference between primitive value and object references is **mutability** (or the ability to be changed), primitive values are **immutable** and object references are **mutable**

- Use **object.assign** to create a **new** object instead of a second reference to the same object

- Check whether the *contents* of two objects are the same by:
  - Iterate through the object and check that each key and value match
  - Convert the object to a suitable primitive before doing the quality check

## Object Literals

- **Objects** group together a set of variables and functions to create a model of something you would recognize from the real world.

- In an object, **variables** become known as **properties** and **functions** become known as **methods**

- Properties and methods have a name and a value, the name is called a **key**

- The value of a method is always a function

- Access the properties or methods of an object using dot notation, you can also use square brackets to access properties

        var hotelName = hotel.name;
        var roomsFree = hotel.checkAvailability();
        var hotelName = hotel['name'];

## Document Object Model

- The Document Object Model (DOM) specifies how browers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the brower window

- the DOM tree is stored in the browsers memory and has four main types of nodes: the **document node**, the **element node**, the **attribute node**, and the **text nodes**

- Working with the DOM tree:
  1. Access the Elements
  2. Work with those elements

- **DOM Queries** - methods that find elements in the DOM tree:
  - getElementById('one');
  - var itemOne = getElementById('one');

- Methods that return a single element node:
  - getElementById('id')
  - guerySelector('css selector')

- Methods that return one or more elements (as a nodelist):
  - getElementsByClassName('class')
  - getElementsByTagName('tagname')
  - querySelectorAll('css selector')

- Ways to select an element from a NodeList (both require the index number ofthe element you want):
  - the item() method
  - array syntax

- You can also select elements using class attributes, tag name, or CSS selectors

- In a NodeList, you can use a **for loop** to loop through each node in the collection and apply the same statments to each

- Select an element in relation to an different element node using one of these 5 properties - **parentNode**, **previousSibling**, **nextSibling**, **firstChild**, **lastchild**

- When you select a text node, you can retrieve or amend the content of it using the **nodeValue** property

- The **textContent** property allows you to collect or update just the text that is in the containing element (and its children)

- Two appraoches to adding and removing content from a DOM tree: the **innerHTML** property and DOM manipulation methods

- **innerHTML** lets your access and amend the contents of an element, including any child elements

- **DOM manipulation** offers another technique to add new content to a page (rather than innerHTML). Three steps: create the element, give it content, and add it to the DOM

- **DOM manipulation to remove** elements frmo the DOM tree: store the element to be removed in a variable, store the parent of that element in a variable, then remove the element from its containing element

- **Cross-Site Scripting Attacks or XSS** - happens when an attacker places malicious code into a site, XSS can give the attacker access to information

- **Prevention of XSS** - validate input going into the server using **validation** then escape the data comoing from the server and database

- Once you have an element node, you can use other properties and methods on that element node to access and change its attributes

- Modern browers come with tools that help you **inspect** tha page loaded in the browser and understand the struvture of the DOM tree - going to the **Properties** panel will tell you the type of object the selected element is

[Return home](https://khofstetter94.github.io/reading-notes/)
