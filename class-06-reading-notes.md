# Dynamic Wed Pages with JavaScript - Reading Notes

View the full blogs:

[JS Intro Paragraph](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

[Input and Output in JS](https://code-maven.com/input-output-in-plain-javascript)

[Variables](https://www.w3schools.com/js/js_variables.asp)

**JavaScript** is a prototype-based, multi-paradigm, slingle-threaded, dynamic language, supporting object-oriented, imperative, and declarative styles.

*Do not confuse JavaScript with Java programming language.*

Visit the link for "JS Intro Paragraph" above for access to several tutorials ranging from beginner to advanced.

- JavaScript allows interaction with the user - the user can provide input that will create an output

- You can create buttons with the button tag and the user can click it to get a result.
- Add an input tag to create a blank field that the user can type in.
- Label each input tag with an id
- You can then use document.getElementById along with the id in parentheses, follow that with a method 'value' that will return the text the user typed in that field

## Four Ways to Declare a JavaScript Variable

- Using var
- Using let
- Using const
- Using nothing

**Variables** are containers for storing data (storing data values)

For example: Declate that 'x' is a variable by writing 'var x' followed by = a value '5'. This says that x stores the value 5. You can replace 'var' with 'let', 'const', or nothing and they will all mean the same thing.

- Always declare JavaScript variable with var, let, or const. 'Var' has been used from 1995-2015, with 'let' and 'const' added in 2015. Use 'var' for older browsers.

- Use 'const' for variable that are constant/cannot change and 'let' for variables that can change

- Just like in algebra - variables hold values, and variables are used in expresions. Example: let z = x + y

## JavaScript Indentifiers

All JavaScript **variables** must be **identified** with **unique names** called **identifiers**

Rules for consrtucting names for variables:

- Names cna contain letters, digits, underscores, and dollar signs
- Names must begin with a letter
- Names can also begin with $ and _
- Names are case sensitive (y and Y are different variables)
- Reserved words (like JavaScript keywords) cannot be used as names

The **=** is an assignment operator not an "equal to" operator, meaning it's just telling you what the variable stands for

Variables can be numbers or text, and text is referred to as text strings. So, variables are numbers and strings. Strings are written inside double or single quotes, numbers do not have quotes

Note: *Its good programming practice to declare all variables at the beginning of a script*

- Output the value inside an HTML paragraph with id="demo". Here is an example of a declared variable with an assigned value with the output value described:

        <p id="demo"></p>

          <script>
            let carName = "Volvo";
            document.getElementById("demo").innerHTML = carName;
          </script>

**One statement, many variables**: if on one line, separate the variables with commas. Or put on one each following line.

**Value = undefined** if something has to be calculated or provided later. For example: let carName;

You can **re-declare** JavaScript variables with 'var' and it will not lose it's original value, but this will not work with 'let' or 'const'

**JaveScript Arithmetic** using operators like = and +. For example: let x = 5 + 2 + 3; which with show 10 **OR** let x = "John" + " " + "Doe"; which will show John Doe. **NOTE** a number in quotes makes the other numbers strings and will be concatenated. For example: let x = 2 + 3 + "5"; which will show 55.

JavaScript treats **a dollar sign** as a letter, identifiers containing $ are valid variable names

JavaScript treats **underscore** as a letter, identifiers containing _ are valid variable names

[Return home](https://khofstetter94.github.io/reading-notes/)
