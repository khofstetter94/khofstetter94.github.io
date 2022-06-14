# State and Props

[React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

## React Lifecycle

- **Lifecycle Events** - React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

- Mounting, Updating, and Unmounting are the three phases of the component lifecycle.

- **Mounting** - Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount

- **Updating** - static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

- **Unmounting** - componentWillUnmount is the only lifecycle event during this phase

- **constructor()** - The constructor for a React component is called before it is mounted. Call super(props) for a subclass component. Avoid using this.setState()

- **staticgetDerivedStateFromProps()** - This method exists for rare cases where the state relies on changes in props over time

- **render()** - the only required method in a class component

- **componentDidMount()** - If you need to load anything using a network request or initialize the DOM, it should go here. setState() can be called here, but it should be used sparingly

- **shouldComponentUpdate()** - Setting this to false allows you to prevent a rerender from happening

- **getSnapshotBeforeUpdate()** - allows you to capture a picture of the DOM to check it before actually changing anything on the DOM

- **componentDidUpdate()** - useful for performing network requests after a change has occurred

- **componentWillUnmount()** - allows you to clean up the DOM and netwrok requests/ subscriptions

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? - the 'render'

2. What is the very first thing to happen in the lifecycle of React? - the constructor for a React component is called

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates - Constructor, render, componentDidMount, React Updates, componentWillUnmount

4. What does componentDidMount do? - If you need to load anything using a network request or initialize the DOM, it should go here. A good place to set up any subscriptions.

## React State vs Props

1. What types of things can you pass in the props? - arguments to a function, they're what you want to initialize your component to or what you want your component to render like. You can pass the initial count for a counter, the title and subtitle

2. What is the big difference between props and state? - props you pass into a component, state is handled inside of that component and props are handled outside of the component

3. When do we re-render our application? - when you change the state inside of your application

4. What are some examples of things that we could store in state? - with forms, you can use state to store what the user is updating the values to and what they're changing that value to and so on.

### Things I want to know more about

- I want to learn more about state vs props, I think I will learn the differences more when we have an example. I would also like to see an example of the React lifecycle.

[Return home](https://khofstetter94.github.io/reading-notes/)
