# Context API - Behaviors

[Hooks and Context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

- With regard to the React Context API, what does a “provider” do?
  - Our context provider is responsible for both displaying the local state of the snackbars (we call them alerts), and for exposing an API for globally managing them.
- With regard to the React Context API, how would we implement a “consumer” role?
  - We need a consumer for the provider.

```js
import { useContext } from 'react'
import { SnackBarContext } from 'components/snack-bar-provider'
const useSnackBars = () => useContext(SnackBarContext)
export default useSnackBars
```

- Specifically with Context, how are we “wrapping” components to achieve our goals?
  - It turns out that our custom hook is nothing more than a small wrapper around the useContext internal React hook, which consumes our new context.

[Awesome React Context links](https://github.com/diegohaz/awesome-react-context)

- Consume content from (at least) two more of the Awesome React Context links. After some familiarity with React Context, once again share your takeaways from each:
  - Takeaway 1: [source](https://reactjs.org/blog/2018/03/29/react-v-16-3.html) Version 16.3 introduces a new context API that is more efficient and supports both static type checking and deep updates. Version 16.3 adds a new option for managing refs that offers the convenience of a string ref without any of the downsides. In addition to deprecating unsafe lifecycles, we are also adding a couple of new lifecyles:
    - getDerivedStateFromProps is being added as a safer alternative to the legacy componentWillReceiveProps. (Note that in most cases you don’t need either of them.)
    - getSnapshotBeforeUpdate is being added to support safely reading properties from e.g. the DOM before updates are made.
  - Takeaway 2: [source](https://medium.com/@DidierFranc/replacing-redux-with-the-new-react-context-api-8f5d01a00e8c) Redux Devtools has been integrated by default in the version 4.0.0, you’ve nothing to do, it just works.
    - Pros
      - Easier to implement
      - Weight and performance
      - Cleaner action return with state chunk (as in setState)
    - Cons
      - It only works with React ^16.3

## Reflection

- What are your learning goals after reading and reviewing the class README?
  - Understand and implent hooks better, especially with context providers and consumers

[Return home](https://khofstetter94.github.io/reading-notes/)
