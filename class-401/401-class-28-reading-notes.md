# Component Lifecycle / useEffect Hook

[effects hook](https://reactjs.org/docs/hooks-effect.html)

- What purpose does useEffect serve in a function component compared to its counterpart(s) in class components?
  - The Effect Hook lets you perform side effects in function components. If you’re familiar with React class lifecycle methods, you can think of useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined. In React classes, we put side effects into componentDidMount and componentDidUpdate.
- When using the useEffect Hook:
  - What does useEffect do?
    - By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. We could perform data fetching or call some other imperative API.
  - Why is useEffect called inside a component?
    - Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.
  - Does useEffect run after every render?
    - Yes! By default, it runs both after the first render and after every update. Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.
- Explain the importance of properly implementing effects with Cleanup
  - React performs the cleanup when the component unmounts. However, effects run for every render and not just once. This is why React also cleans up effects from the previous render before running the effects next time.

## Reflection

- What are your learning goals after reading and reviewing the class README?
  - I hoping to really do a deep dive into Hooks. After the reading, I'm really curious about the useEffect hooks as well.

## Things I want to know more about

- Implementing the useEffect!

[Return home](https://khofstetter94.github.io/reading-notes/)
