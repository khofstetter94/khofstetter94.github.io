# Combined Reducers

- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

  - Why create multiple reducers?
    - One larger reducer is a mess to maintain. One reducer handles a part of the state and cannot affect the other.
  - How would you combine multiple reducers?
    - It will take in all the unique reducers and combine them into one reducer that can be utilixed throughout the application.
  - How will you manage state as an immutable object? why?
    - You need to make a deep copy of the current state and return a new state object because if you dont, the initial state will be overridden.

- [Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)

  - combineReducers is a utility function to simplify the most common use case when writing ________ .
    - Redux reducers
  - Explain how combineReducers assembles the new state tree.
    - In order to assemble the new state tree, combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.
  - How would you define initial state in an app using combineReducers?
    - combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object.

- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

  - Why will you want to split your reducing functions as your app becomes more complex?
    - As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state. This makes your entire application more manageable.
  - The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.
    - combineReducers, createStore
  - What is a popular convention when naming reducers?
    - A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: combineReducers({ counter, todos }). This is equivalent to writing combineReducers({ counter: counter, todos: todos }).

- Reflection

  - What are your learning goals after reading and reviewing the class README?
    - To be able to say and show that I understand how to use React and Redux.

[Return home](https://khofstetter94.github.io/reading-notes/)
