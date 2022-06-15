# Lists and Keys, The Spread Operator, and Passing Functions as Props

[React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

## Lists and Keys

- **What does .map() return?** - it loops through an array and manipulates the values with a function, then returns a new array with the changed values
- **If I want to loop through an array and display each value in JSX, how do I do that in React?** - you can attach the .map() function to your array which would loop through the values, then in the function you can return an li element for each item. Assign this resulting array of elements to a varaible which you can then place inside a ul element
- **Each list item needs a unique ____.** - Key
- **What is the purpose of a key?** - Keys help React identify which items have changed, are added, or are removed. If you extract a ListItem component, you should keep the key on the ListItem/ elements in the array rather than on the li element in the ListItem itself.

## The Spread Operator

- **What is the spread operator?** - The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
- **List 4 things that the spread operator can do.** - Copying an array, Concatenating or combining arrays, Using Math functions, Using an array as arguments, Adding an item to a list, Adding to state in React, Combining objects, Converting NodeList to an array
- **Give an example of using the spread operator to combine two arrays.** -

        let oneArr = [1, 2, 3]
        let twoArr = [4, 5, 6]
        let bothArr = [...oneArr, ...twoArr]
        console.log(...bothArr) // 1 2 3 4 5 6

- **Give an example of using the spread operator to add a new item to an array.** -

        let smallArr = [1, 2, 3, 4]
        let addArr = [5, 6, 7, 8, ...smallArr]
        console.log(addArr) // Array (8) [1, 2, 3, 4, 5, 6, 7, 8]

- **Give an example of using the spread operator to combine two objects into one.** -

        let objectOne = {first: "KC"}
        let objectTwo = {last: "Hofstetter"}
        let objectThree = {...objectOne, ...objectTwo}
        console.log(objectThree) // object {first: "KC", last: "Hofstetter"}

## How to Pass Functions Between Components

- **In the video, what is the first step that the developer does to pass functions between components?** - create the function wherever the state is that youre going to change
- **In your own words, what does the increment function do?** - the increment function takes in an argument and then changes it's value (increments it) and returns the new value
- **How can you pass a method from a parent component into a child component?** - just like any other prop. While in the parent component, add a property inside the object of the child component - create a key/name and then add the value using 'this.theMethodName' (matching the name of of the method you created in the parent). The name you created is what will be used in the child component to invoke the method
- **How does the child component invoke a method that was passed to it from a parent component?** - you use 'this.props.theMethod()'

### Things I want to know more about

- I really need another example and personnal practice with the passing of functions between components, I watched the video twice and tried my best answering the questions but I still don't think I understand it

[Return home](https://khofstetter94.github.io/reading-notes/)
