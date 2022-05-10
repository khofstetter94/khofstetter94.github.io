# Operators and Loops

View the full blogs:

[Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

[Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

JavaScript hass both *binary* and *unary* operators, and a special *ternary* operator, the conditional operator.

A **binary** operator requires two operands, one before the operator and one after:

    operand1 operator operand2
    Ex: 3+4 or x*y

A **unary** operator requires a single operand, either before or after the operator:

    operator operand
    Ex: x++ or ++x

## Assignment Operators

An **assignment operator** assigns a value to its left operand based on the value of its right operand.

    Simple assignment operator is equal (=)
    x = f()

- view blog Expressions and Operators linked above a for table of compound assignment operators that are shorthand for the operations listed in the table.

**Assigning to properties** - if a variable refers to an *object* then the left-hand side of an assignment expression may make assignments to properties of that variable

**Destructuring** - extract data from arrays or objects using a syntax that mirrors the construction of array and object literals

**Evaluation and nesting** - by chaining or nesting an assignment expression, its results can itself be assigned to another variable. It can be logged, it can be put inside an array literal or function call, and so on.

- When chaining these expressions without parentheses or other grouping operators like array literals, the assignment expressions are **grouped right to left** but they are evaluated **left to right**
- Note that, for all assignment operators other than '=' itself, the resulting values are always based on the operands' values *before* the operation
- Chaining assignments in the same statement is discouraged: let z = y = x = f();

## Comparison Operators

A **comparison operator** compares its operands and returns a logical value based on whether the comparison is true.

- The operands can be numerical, string, logical, or object values

View the table for comparision operators but clicking the link above for 'Expressions and Operators'

## Loops and iteration

A **for** statement - a 'for' loop repeats until a specified condition evalutaes to false. It looks as follows:

    for ([initialExpression]; [conditionExpression];          [incrementExpression])
       statement

A **while** statement executes its statement as long as a specified condition evaluates to 'true'. A **while** statements looks as follows:

    while (condition)
       statement

- If the 'condition' becomes **false**, 'statement' within the loop stops executing and control passes to the statement following the loop.
- If the condition returns 'true', statement is executed and the 'condition' is tested again. This continues until the 'condition' returns 'false'
- **AVOID** infinite loops - make sure the condition will eventually lead to a 'false'

[Return home](https://khofstetter94.github.io/reading-notes/)
