# Basics of HTML, CSS, & JS

## Text

**Headings** - 6 levels ranging from the most important to the least, h1-h6, h1 being the largest font and most important heading
**Paragraphs** - Use the 'p' tag to create a paragraph, each tag will represent a new line
**Bold** - make your text bold by wrapping it with a 'b' tag
**Italic** - make your text italic by wrapping with a 'i' tag
**Superscript & subscript** - for characters that need to be raised or lowered (like raising a number to a power or foot notes), use the 'sup' tag or 'sub' tag:

        4<sup>th</sup>
        CO<sub>2</sub>

- **White space** - browers see any number of spaces or line breaks as a single space, known as *white space collapsing*

- **Line breaks** - add a line break with the 'br' tag

- **Horizontal rules** - use the 'hr /' tag to create a break between topics. This is a type of empty element, it only has one tag

### Semantic Markup

These text elements do not change how your webpage looks, but gives more information and meaning to the text. This is important for search engines and screen readers. This will help dictate importance of text and description of the type of text.

- **Strong** - use the 'strong' tag for content that is very important, this will show up bold by default

- **Emphasis** - use the 'em' tag to add emphasis and change the meaning of a sentance, this will show up italic by default

- **Quotations** - Use 'blockquote' for long paragraph quotes but be sure to add the 'p' tag inside the 'blockquote' as well. Use the 'q' tag for shorter quotes

- **Abbreviations & acronyms** - Use 'abbr' if you are going to abbreviate a word, and 'acronym' for any acronyms, then add a title attribute inside the tag to write out the full word

- **Citations and Definitions** - Use the 'cite' tag to cite where the reference is from. Use the 'dfn' tag when you introduce a new term for the first time
**Author details* - Use the 'address' tag for the contact information of the page's author

- **Changes to content** - If you add content into a document, use the 'ins' tag and if you remove content, use the 'del' tag. If content is inaccurate but shouldn't be deleted, use the 's' tag and it will appear striked through

## Introducing CSS

CSS makes your website pretty! Add borders and color, change the size and look of text, add background color, change the shape of images and boxes, ect. It's helpful to imagine each HTML element is in its own box that can be manipulated with CSS.

- **CSS rule** - given to HTML elements, a CSS rule includes a selector and a declaration. The *selector* shows with HTML element will be assigned the rule, and the *declaration* indicates how the element should be styled (it includes a property and a value)

- **Properties and values** - the properties are what you will be changing (color, font, height, ect) and values are the settings you want to set (yellow, Arial, 5px). You can use multiple properties separated by semi-colons

        h1 {
          font-family: Arial;
          color: yellow;
        }

**External CSS** - Use for sites with more than one page. If you have your CSS in a separate file, add a 'link' tag into your HTML so that your document can access it. Put it in the 'head' tag. There is no closing tag. Inside the 'link' tag add the 'href' to provide the path, write the 'type' which would be 'text/css'. Add the 'rel' to specify the relationship, which would be 'stylesheet'

        <link href="css/styles.css" type="text/css" rel="stylesheet" />

**Internal CSS** - Add CSS directly into your HTML with the 'style' tag located within your 'head' tag. Add an attribute 'type' to state that the styles are CSS with value 'text/css'

- There are several **css selectors** that lets you target rules to specific HTML elements. They are case sensitive and must match element names and values exactly.

- **Precedence** - If there is more than one rule for the same element, the **LAST RULE** will take precedence. If the selector is more **SPECIFIC** then it will take precedence. You can always add '!important' to show that it should take precedence

- **Inheritance** - Some properties are inherited by child elements. If you specify the font-family or color for the 'body' tag, they will get inherited

It is a good idea to have an external style sheet so that you dont have to repeat code throughout other pages. This will also make the HTML easier to read. Editing the overall look of your website is easier and faster when editing one file rather than many different areas of code

Be sure to test your new site on many different browsers before launching because some may not support your version of CSS

## Basic JavaScript Instructions

- **Statements** - are the steps for instruction, they end with a semi-colon, Each one should start on a new line.
- **Comments** - explains what your code does, helps make your code eassier to read and understand. For a multi-line comment, write it between:

        /* Write a longer, multi line comment here, usually to describe how the script will work */

for single-line comments, write it with two // before the text.

- **Variable** - temporarily stores data to be used for computations or calculations. Variables need to be declared - use variable keyword 'let' followed by a variable name (use camelCase for names with more than one word). Then assign a value with the **assignment operator** '='. For example:

        let totalVolunteers = 20

- **Date types** - Numeric data types are numbers (1, 2, 3), string data types are letters and characters ('Hello, Jeremy'), and boolean data types have one or two values (true/false)

- Use a variable to store a string by placing the string inside quotes - be sure to start and end with the same single or double quote. Using quotes inside a string requires the outside quotes to be the opposite of the inside quotes (one set is double and one set if single quote marks)

- Using a variable to store a boolean, it must be true or false or used when your code may take more than one path

- **Rules for naming variables** - begins with a letter/$/underscore and NOT a number. Contains letters/numbers/$/underscores and NOT dashes or periods. Do NOT use keywords. Case sensitive!! Use names that describe the information beingn stored. Use camelCase with more than one word names.

- **Arrays** - Use an array when working with a list or set of related values. Values are assigned inside square brackets and separated by commas. Each item is given a number called an **index** which starts at zero (0) then counts up. To retrieve an item in the list, specify the array name then the index number in square brackets. Change a value by stating the array name followed by the index number of the value to be changed inside square brackets, then asign it a new value using '='

- **Expressions** - Evaluates into a single value. Two types - expressions that just assign a value to a variable or expressions that use two or more values to return a single value.

- **Operators** - allow programmers to create a single value from one or more values. Assignment operators like '=', arithmetic operators perform math like multiplication '*', string operators combine two strings 'Hi' + ' Jeremy'

- **Concatenation** - the process of joining together two or more strings to create one new string

## Decisions & Loops

As the user makers their way through your webpage, different interactions may move them down different paths - which can be determined by evaluations, decisions, and loops

- **Decision making** -  in script, there may be times where a decision must be made to move on, and the next path depends on the answer. Comparision operators like >, <, == compare values and determine if a condition has been met

- **Decision making & conditional statments** - In a decision, an expression is evaulated and returns a value, then a conditional statement determines what to do in a given situation. The comparision operator determines if the given value is true or false. *If* the value meets the conditions (true) *then* your code executes more statements *else* it does something else

- **Comparision operators: evaluating conditions** - Comparing two values with the result being true or false. '==' represents being equal, '!=' represents not being equal, '===' requires being strictly equal in both data and value, '!==" requires being strictly NOT equal, '>' the number on the left is greater than the right, '<' the number on the left is less than the right, '>=' the number on the left is greater than or equal to the right, '<=' the number on the left is less than or equal to the right. Example structured comparision:

        (age >= 21)

- Note that an operand can be an expression, where each expression evaluates into a single value to be compared. This can be done by setting variables as different values, then using an arithmetic operator to combine the values, then use a comparision operator to compare the two resulting values.

- **Logical operators** - allow comparision of results of more than one comparison operator. On either side of the logical operator, two different expressions use different comparision operators to return a value, these two values are then compared with the logical operator between them. With '&&' both values need to be true. '&&' logical 'and', '||' logical 'or', '!' logical 'not'. Logical expressions read left to right, once a 'true' value is read, the reading stops and the value is true.

- **If statements** - *if* statements allows the executions of subsequent code blocks only *if* a condition evaluates to true. Example:

        if (age >= 21) {
          drink();
        }

- **If..Else statements** - This statement checks a conditions, *if* it is true then the first code block is executed, *else* (if it is false) then the second code block is executed. Example:

        if (age >= 21) {
          msg = 'You may enter the bar';
        }
        else {
          msg = 'You may not enter the bar';
        }

- **Switch statements** - This statements starts with a variable that will determine which code block runs. This switch value is followed by different 'cases' with different possible values for the variable, which ever matches the value will be exectuted. Example:

[Return home](https://khofstetter94.github.io/reading-notes/)
