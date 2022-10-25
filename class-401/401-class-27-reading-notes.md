# useState() Hook

[Introducing Hooks](https://reactjs.org/docs/hooks-intro.html#motivation)

- What was the motivation for introducing Hooks?
  - They let you use state and other React features without writing a class. Hooks solve a wide variety of seemingly unconnected problems in React that we’ve encountered over five years of writing and maintaining tens of thousands of components. It’s hard to reuse stateful logic between components - Hooks allow you to reuse stateful logic without changing your component hierarchy. Complex components become hard to understand - Hooks let you split one component into smaller functions based on what pieces are related (such as setting up a subscription or fetching data). Classes confuse both people and machines - Hooks let you use more of React’s features without classes.
- What changes are important regarding implementing Hooks versus Component Classes?
  - Hooks work side-by-side with existing code so you can adopt them gradually. It’s best to practice using Hooks in new and non-critical components first, and ensure that everybody on your team feels comfortable with them.
- Hooks allow you to reuse stateful logic without changing __________.
  - your component hierarchy.

[hooks api](https://reactjs.org/docs/hooks-overview.html)

- Name two rules imposed by React Hook usage.
  - Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
  - Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)
- How would you identify a custom Hook and why might you create one?
  - If a function’s name starts with ”use” and it calls other Hooks, we say it is a custom Hook. You can write custom Hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers, and probably many more we haven’t considered.

[the state hook](https://reactjs.org/docs/hooks-state.html)

- What is a Hook?
  - A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.
- When would I use the useState Hook?
  - In a function component, we have no 'this', so we can’t assign or read this.state. Instead, we call the useState Hook directly inside our component:

```js
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);
```

- If you were to add React state to a function component by declaring a state variable:
  - What does calling useState do?
    - It declares a “state variable”. This is a way to “preserve” some values between the function calls — useState is a new way to use the exact same capabilities that this.state provides in a class. Normally, variables “disappear” when the function exits but state variables are preserved by React.
  - What do we pass to useState as an argument?
    - The only argument to the useState() Hook is the initial state. Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need.
  - What does useState return?
    - It returns a pair of values: the current state and a function that updates it. This is similar to this.state.count and this.setState in a class, except you get them in a pair.

## Reflection

- What are your learning goals after reading and reviewing the class README?
  - I hoping to really do a deep dive into Hooks. After the reading, I'm really curious about custom hooks as well.

## Things I want to know more about

- Implementing Hooks, everything about Hooks! They sound awesome, but I can't quite wrap my head around them yet.

[Return home](https://khofstetter94.github.io/reading-notes/)
