# Putting it all together

[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

- **What is the single responsibility principle and how does it apply to components?** - a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents
- **What does it mean to build a ‘static’ version of your application?** - build a version that takes your data model and renders the UI but has no interactivity, you’ll want to build components that reuse other components and pass data using props, don’t use state at all
- **Once you have a static application, what do you need to add?** - Identify the minimal representation of UI state. This is where you start to plan out how you want to trigger changes to your underlying data model using state
- **What are the three questions you can ask to determine if something is state?** - Is it passed in from a parent via props? If so, it probably isn’t state. Does it remain unchanged over time? If so, it probably isn’t state. Can you compute it based on any other state or props in your component? If so, it isn’t state.
- **How can you identify where state needs to live?** - Identify every component that renders something based on that state. Find a common owner component (a single component above all the components that need the state in the hierarchy). Either the common owner or another component higher up in the hierarchy should own the state. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

- **What is a “higher-order function”?** - Functions that operate on other functions, either by taking them as arguments or by returning them
- **Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?** - this function will return a boolean, line two compares m & n asking if the value of m is larger than the value of n. If so, then the function will return true, if not then false.
- **Explain how either map or reduce operates, with regards to higher-order functions.** - The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. Reduce builds a value by repeatedly taking a single element from the array and combining it with the current value. The parameters to reduce are, apart from the array, a combining function and a start value.

## Things I want to know more about

- I think I just need to read the "Thinking in React" article about 5 more times, cause it was pretty helpful! I would also like more examples of the reduce function.

[Return home](https://khofstetter94.github.io/reading-notes/)
