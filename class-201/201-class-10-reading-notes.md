# Debugging

- Duckett, J. (2014). JavaScript &amp; JQuery. John Wiley &amp; Sons, Inc. .

## Error Handling & Debugging

- **Execution context** - every statement in a script lives in one of three execution contexts: Global context, function context, eval context (not shown)

- **Variable Scope** - global scope: variable outside a function can be used anywhere. Function-level scope: declared in a function, only used in that function

- **The stack** - The JS interpreter processes one line of code at a time. When a statement needs data from another function, it stacks (or piles) the new function on top of the current task

- **Scope** - each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution contect can also access its parents variables object

- **Errors** - If a JS statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code

- **Error Objects** - Error bojects can help uou find where your mistakes are and browsers have tools to help you read them. Error messages may vary by browser

- **Dealing with Errors** - Two things to do: Debug the script to fix errors or handle errors gracefully (using try, catch, throw, and finally statements)

- **JavaScript Console** - will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be

- **Console methods** - **'console.info()'** can be used for general information. **'console.warn()'** can be used for warnings. **'console.error()'** can be used to hold errors. **'console.log()'** writes values to the console. **'console.group()'** writes a set of related data to the console. **'console.table()'** lets you output a table showing objects and arrays that contain other objects or arrays. **'console.assert()'** you can test if a condition is met, and write to the console only if the expression evaluates to false

- **Breakpoints** - you can pause the execution of a script on any line using breakpoints. Then you can check the values stores in variables at that point in time

- **Stepping through code** - the debugger can **step over** functions by moving onto the line after it or it can **step into** a function to see what is happening inside

- **Conditional Breakpoints** - you can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.

- **Debugger Keyword** - can be placed in your code to cause a breakpoint. You can also put the keyword in a conditional statement so that it triggers if the condition is met

- **Handling exceptions** - If you know your code might fail, use **try**, **catch**, and **finally**. Each one is given its own code block

- **Throwing errors** - if you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them

[Return home](https://khofstetter94.github.io/reading-notes/)
