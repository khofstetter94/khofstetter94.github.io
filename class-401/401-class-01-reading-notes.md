# Node Ecosystem

[What Is Node and When Should I Use It?](https://www.sitepoint.com/an-introduction-to-node-js/)

- Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
- The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi.
  - It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.
- Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.
- Node has excellent support for ECMAScript 2015 (ES6) and beyond
- We can also install packages locally to a project, as opposed to globally, on our system
- Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior
- blocking I/O calls should be avoided, CPU-intensive operations should be handed off to a worker thread, and errors should always be handled correctly for fear of crashing the entire process
- Node is particularly suited to building applications that require some form of real-time interaction or collaboration
  - It’s also a good fit for building APIs where you’re handling lots of requests that are I/O driven, or for sites involving data streaming
- it can be used as a scripting language to automate repetitive or error prone tasks on your PC
- It can also be used to write your own command line tool
- Node.js can also can be used to build cross-platform desktop apps and even to create your own robots

## Discussion Questions

- How would you describe Node to a non-technical friend?
  - Node is a JavaScript runtime, which basically allows us to run our JS script on our computers rather than the browser. Its event-based (everything that happens in Node is in reaction to an event), non-blocking (acts in an asynchronous way so that the running of the script isn't blocked, it'll execute other pieces of code out of "order"), and asynchronous (The code can run "out of order").
- What does it mean that Node is a JavaScript runtime?
  - Node.js is a program we can use to execute JavaScript on our computers.
- What is Node used for?
  - Node not only allows you to run your JavaScript on your computer, but it comes with several tools that help you along the way to build and automate your application

### Things I want to know more about

- Using node in more advanced ways, I'd love to build my own robot!

[Return home](https://khofstetter94.github.io/reading-notes/)
