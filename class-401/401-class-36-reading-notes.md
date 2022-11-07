# Application State with Redux

[Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

- What is the first principle of Redux?
  - The first principle of Redux is whether your app is a really simple one like this counter example, or a complex application with a lot of UI, and change of state, you are going to represent the whole state of your application as a single JavaScript object.
- what is a store and what do we use our reducers for within that store?
  - The store binds together the three principles of Redux. It holds the current application's state object. It lets you dispatch actions.
- Name three Redux store methods given to us by createStore and describe their use.
  - The first method of this store is called get state. It retrieves the current state of the Redux store.
  - The second and the most commonly used store method is called dispatch. It lets you dispatch actions to change the state of your application.
  - The third Redux store method, is called subscribe. It lets you register a callback that the Redux store will call any time an action has been dispatched, so that you can update the UI of your application. It will reflect the current application state.
- Explain to a non-technical recruiter what combineReducers() does and why it is useful.
  - We were using the reducer composition pattern to let different reducers handle different parts of the state tree, and then combine their results. Redux provides a function called combineReducers that lets you avoid writing the code by hand. Instead, it generates the top level reducer for you.
- Additional Questions
  - Looking ahead at this module’s course scheduleLinks to an external site., What do you look forward to learning?
    - Learning Redux, personal presentations - to hear more about my classmates
  - What are your learning goals after reading and reviewing the class README?Links to an external site.
    - Learning Redux!

[Return home](https://khofstetter94.github.io/reading-notes/)
