# The JavaScript Call Stack & Error Messages

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

- **What is a ‘call’?** - function invocation
- **How many ‘calls’ can happen at once?** - Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
- **What does LIFO mean?** - Last In, First Out
- **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.** -

        function firstFunction(){
          throw new Error('Stack Trace Error');
        }

        function secondFunction(){
          firstFunction();
        }

        function thirdFunction(){
          secondFunction();
        }

        thirdFunction();

- **What causes a Stack Overflow?** - when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

- **What is a ‘reference error’?** - This is as simple as when you try to use a variable that is not yet declared you get this type os errors.This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occur.
- **What is a ‘syntax error’?** - this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
- **What is a ‘range error’?** - Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
- **What is a ‘tyep error’?** - this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
- **What is a breakpoint?** - The breakpoint can be achieved by putting a debugger statement in your code in the line you want to break. You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met.
- **What does the word ‘debugger’ do in your code?** - it breaks it at the point where the debugger is placed so that you can evaluate the history created before that point to make sure you are getting the results you want.

[Return home](https://khofstetter94.github.io/reading-notes/)
