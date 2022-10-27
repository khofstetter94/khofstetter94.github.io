# Advanced State with Reducers

- [useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

  - Name an alternative to the useState Hook.
    - useReducer
  - Why might the useReducer Hook be preferable to the useState Hook?
    - useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.
  - What are two ways to set the initial state?
    - The simplest way is to pass the initial state as a second argument
    - You can also create the initial state lazily. To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg).

- [Ultimate Guide to useReducer](https://blog.logrocket.com/react-usereducer-hook-ultimate-guide/)

  - In terms of state, what does useReducer expect to receive as a parameter?
    - It accepts a reducer function as its first parameter and the initial state as the second.
  - What does useReducer return?
    - useReducer returns an array that holds the current state value and a dispatch function to which you can pass an action and later invoke it.
  - Explain dispatch to a non-technical recruiter.
    - The dispatch function accepts an object that represents the type of action we want to execute when it is called. Basically, it sends the type of action to the reducer function to perform its job, which, of course, is updating the state. The action to be executed is specified in our reducer function, which in turn, is passed to the useReducer. The reducer function will then return the updated state.

- Reflection

  - What are your learning goals after reading and reviewing the class README?
    - I need more practice with useState, useEffect, and now useReducer

## Things I want to know more about

- This useReducer business isn't quite sticking in my head. I'm looking forward to lecture for an example of how to implement this.

[Return home](https://khofstetter94.github.io/reading-notes/)
