# Class 07 Reading Notes

View the full blogs:

[MDN Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)

[JavaScript Functions](https://www.w3schools.com/js/js_functions.asp)

[JavaScript Operators](https://www.w3schools.com/js/js_operators.asp)

## Control Flow

The *control flow* is the order in which the computer exectues statements in a script.

Code is typically run from the first line to the last unless told otherwise by structures like **conditionals**, **functions**, and **loops**.

Often times user input is required and if the user messes up and misses something, you can use a conditional to ask them to fix the mistake. For example:

        if (field==empty) {
             promptUser();
        } else {
             submitForm();
        }

A loop iterates through through all of the fields in the form, checking each one in turn.

## JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task and is executed when "something" invokes it.

- use the 'function' keyword, followed by a name (same rules as variables - letters, digits, underscores, and dollar signs), followed by parentheses
- In the parentheses include parameter names separated by commas
- The code to be executed will go in curly brackets

        function name(parameter1, parameter2, parameter3) {
          // code to be executed
        }

**Function invocation** occurs when:

- an event occurs (user clicks a button)
- it is invoked (called) from JavaScript code
- Automatically (self invoked)

**Function return** - the function will stop executing when a 'return' statement is reached. If invoked by a statment, will "return" to execute the code after the invoking statment. Functions often compute a return value - the return value is "returned" back to the "caller".

Why functions? *You can reuse code: define the code once, and use it many times*

**The () operator invokes the function** - accessing a function without () will return the function object instread of the function result.

Functions can be used directly as **variable values**

Variables declared **WITHIN** a function become **LOCAL** to the function and can only be accessed from within that function.

## JavaScript Arithmetic Operators

| Operator    | Description |
| ----------- | ----------- |
| +           | Addition    |
| -           | Subtraction |
| *           | Multiplication |
| **          | Exponentiation |
| /           | Division |
| %           | Modulus |
| ++          | Increment |
| --          | Decrement |

## JavaScript Assignment Operators

| Operator | Example | Same As |
| -------- | ------- | ------- |
| =   | x = y | x = y |
| +- | x += y | x = x + y |
| -+ | x -+ y | x = x - y |
| *= | x *= y | x = x * y |
| /= | x /= y | x = x / y |
| %= | x %= y | x = x % y |
| **= | x **= y | x = x ** y |

- The + operator can also be used to add strings
- The += assignment operator can also be used to add strings
- Adding two numbers will return the sum, but adding a number and a string will return a string

## JavaScript Comparision Operators

| Operator | Description |
| -------- | ------------ |
| == | equal to |
| === | equal value and equal type |
| != | not equal |
| !== | not equal value or not equal type |
| > | greater than |
| < | less than |
| >= | greater than or equal to |
| <= | less than or equal to |
| ? | ternary operator |

## JavaScript Logical Operators

| Operator | Description |
| -------- | ----------- |
| && | logical and |
| \| \|| logical or |
| ! | logical not |

## JavaScript Type Operators

| Operator | Description |
| -------- | ----------- |
| typeof | Returns the type of a variable |
| instanceof | Returns true if an object is an instance of an object type |

[Return home](https://khofstetter94.github.io/reading-notes/)
