# Asynchronous Actions

- [async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

  - Why use Redux middleware?
    - Redux reducers must never contain "side effects", but Redux middleware were designed to enable writing logic that has side effects. a Redux middleware can do anything when it sees a dispatched action: log something, modify the action, delay the action, make an async call, and more. Also, since middleware form a pipeline around the real store.dispatch function, this also means that we could actually pass something that isn't a plain action object to dispatch, as long as a middleware intercepts that value and doesn't let it reach the reducers. Middleware also have access to dispatch and getState. That means you could write some async logic in a middleware, and still have the ability to interact with the Redux store by dispatching actions.
  - Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.
    - The Redux asycn data flow begins with an action triggered in the UI by the user, that click event is sent to the event handler which in turn sets off a dispatch with the action/thunk, the middleware catches that action and sends off the API call request and waits for the response back, once the information is recieved the middleware sends a dispatch to the store with the action/data, the state is affected throughout the reducers with the action and then updates the UI with the new data.
  - How are we accommodating async in our Redux app?
    - By using async function middleware called the Redux "Thunk" middleware.

- [thunk middleware](https://github.com/reduxjs/redux-thunk)

  - Why would you need redux-thunk middleware?
    - It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.
  - Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.
    - Function
  - Describe how any return value from the inner thunk function will be made available.
    - Any return value from the inner function will be available as the return value of dispatch itself. This is convenient for orchestrating an asynchronous control flow with thunk action creators dispatching each other and returning Promises to wait for each other’s completion.

- Reflection

  - What are your learning goals after reading and reviewing the class README?
    - To better understand asynchronous actions with Redux middleware/Thunk

[Return home](https://khofstetter94.github.io/reading-notes/)
