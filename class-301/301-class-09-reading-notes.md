# Functional Programming

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

- **What is functional programming?** - Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia
- **What is a pure function and how do we know if something is a pure function?** -It returns the same result if given the same arguments (it is also referred as deterministic). It does not cause any observable side effects
- **What are the benefits of a pure function?** - The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts. Immutability:
Unchanging over time or unable to be changed. Referential transparency
- **What is immutability?** - Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created.
- **What is Referential transparency?** - Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

        pure functions + immutable data = referential transparency

- **What is a module?** - splitting one file of code into logical modules, different modules for different chunks of code that serve a different purpose. Essentially another JS file.
- **What does the word ‘require’ do?** - It is on the global object of node.js. It brings another module into the file you need to use it in.
- **How do we bring another module into the file the we are working in?** - in the file we are working in, we need to 'require' the file (require(./filename))...
- **What do we have to do to make a module available?** -...(see above) and then in the file we are requiring, we need to have a 'module.exports=' and assign it to the functions we want to use in our current file. Then set the require to a variable to be used where needed.

[Return home](https://khofstetter94.github.io/reading-notes/)
