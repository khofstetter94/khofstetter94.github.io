# Component Based UI

[react hello world](https://reactjs.org/docs/hello-world.html)

- What are the building blocks of a React app?
  - elements and components.
- What is the difference between an element and a React component?
  - An element is a description of what you want to see on the screen, and React elements are plain objects, and are cheap to create. Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
- What are some advantages of React’s component based architecture?
  - Components are reusable and can be used across the application. It also allows repitiion that directly helps with scalability. Its more manageable and thus creates faster development.

[introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

- What is JSX and why do we use it?
  - It is a syntax extension to JavaScript. We use it with React to describe what the UI should look like. React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

```javascript
const element = <h1>Hello, world!</h1>;
```

- Describe the process of embedding JavaScript expressions in JSX.
  - You can put any valid JavaScript expression inside the curly braces in JSX. For example, 2 + 2, user.firstName, or formatName(user) are all valid JavaScript expressions.

```javascript
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```

- Is it safe to embed user input in JSX? Explain.
  - Yes, by default, React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered. This helps prevent XSS (cross-site-scripting) attacks.

[rendering elements](https://reactjs.org/docs/rendering-elements.html)

- Explain what a React Component is to a non-technical friend.
  - Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML. [source](https://www.w3schools.com/react/react_components.asp#:~:text=Components%20are%20independent%20and%20reusable,will%20concentrate%20on%20Function%20components.)
- Describe mutability and React Components, specifically, how is the UI updated?
  - The State in React components are mutable, and whenever there are changes to the state, the UI updates
- If changes are made to the UI, what does React update?
  - By utilizing the State, when the state changes, it re-renders

[Return home](https://khofstetter94.github.io/reading-notes/)
