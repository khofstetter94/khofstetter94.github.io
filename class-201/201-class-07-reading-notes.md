# Object-Oriented Programming, HTML Tables

- [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc.

- Duckett, J. (2011). Html &amp; Css. John Wiley &amp; Sons, Inc.

## Domain Modeling

- **Domain modeling** is the process of creating a conceptual model in code for a specific problem

- **Object oriented model** is an entity that stores data in properties and encapsulates behaviors in methods

- **Constructor functions** define the same properties between many objects
  - The **new** keyword instantiates (or creates) an object
  - The constructor function initializes properties inside that object using the **this** variable
  - The object is stores in a variable for later use

- Methods can be added to a construcor function's **prototype** to do all the work for the object

- Use **Math.random()** function to generate a random number

- Model behaviors with small methods that do their job well

## Tables

- A **table** represents information in a grid format

- Basic structure of a table:
  - **'table'** used to create a table
  - **'th'** is the table heading, use a 'scope' attribute to indicate if its a column (col) or a row (row)
  - **'colspan="#"'** this attribute lets you make a cell span across multiple cells, the # would be replaced with the number of cells to occupy
  - **'rowspan="#"'** same goes for this attribute but for rows
  - **'tr'** the start of each row, and between the opening and closing element are:
  - **'td'** which represents each cell of the table

- Place headings inside the **'thead'** element, Place the body inside the **'tbody'** element, Place the footer inside the 'tfoot' element

- **Updating an object** - use dot notation or square brackets to update the value of properties. Use the **delete** keyword to delete a property

- **This** is a kewyword used inside functions and objectsm it refers to one object, usually the object in which the function operates

- In JS, data is represented in **name/value pairs**, you can organize your date using an array or obect to group a set of related values

- **Arrays** are objects, holds a related set of key/value pairs, but the key for each value is its index number. You can use arrays to store a series of objects and you can have objects that hold arrays

- Browsers come with a set of **built-in objects**, this new toolkit has three compartments: Broswer Object Model, Document Object Model, and Global JavaScript Objects

- **Browser Object Model** contains objects that represent the current brower window or tab

- **Document Object Model** uses objects to create a representation of the current page, new objects for each element

- **Global JasaScript Objects** represent things that the JS language needs to create a model of

- **Global Objects: String Objects** - when you have a value that is a string, you can use the properties and methods of the **String Object** on that value

- **JS 6 data types** - simple or primitive types: string, number, boolean, undefined, null. Complex data type: object

- Use **Number object** methods and properties on values that are a number

- Use **Math object** methods and properties for mathemetaical constants and functions

- The **Date object** you can secify the time and date that you want it to represent

        var today = new Date()

[Return home](https://khofstetter94.github.io/reading-notes/)
