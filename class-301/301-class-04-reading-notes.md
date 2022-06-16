# React and Forms, The Ternary Operator

[React Docs - Forms](https://reactjs.org/docs/forms.html)

[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

## Forms - React

- **What is a ‘Controlled Component’?** - components in which the input's data is handled by the component's state
- **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.** - update as soon as they enter them, Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.
- **How do we target what the user is entering if we have an event handler on an input field?** - it will be an argument into the event handler, for example event.target.value

- mutable state is typically kept in the state property of components, and only updated with setState()

- \<textarea> uses a value attribute, This way, a form using a \<textarea> can be written very similarly to a form that uses a single-line input

- Instead of using a selected attribute, use a value attribute on the root select tag

- \<input type="text">, \<textarea>, and \<select> all work very similarly - they all accept a value attribute that you can use to implement a controlled component.

- setState() automatically merges a partial state into the current state, we only needed to call it with the changed parts.

## The Ternary Operator

- **Why would we use a ternary operator?** - You can do the same thing as an 'if' statement but in one line of code
- **Rewrite the following statement using a ternary statement:** -

        if(x===y){
          console.log(true);
        } else {

        x===y ? console.log(true) :

- an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met

        condition ? value if true : value if false

- Here’s what you need to know:

1. The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
2. A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.
3. Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

        let isStudent = false;
        let isSenior = true;
        let price = isStudent ? 8 : isSenior ? 6 : 10
        console.log(price);
        // 6

- Break it down:

1. First we check to see if our patron is a student. Since isStudent is false, only the code after the first : is executed. After the : we have a new conditional:
2. Our second conditional tests isSenior — since this is true, only the code after the ? but before the : is executed.
3. price is then assigned the value of 6 which which we later log to the screen.

- It is also possible to run **multiple operations** within a ternary. To do this, we must separate the operations with a comma. You can also, optionally, use parenthesis to help group your code

        let isStudent = true;
        let price = 12;
        isStudent ? (
          price = 8,
          alert('Please check for student ID')
        ) : (
          alert('Enjoy the movie')
        );

[Return home](https://khofstetter94.github.io/reading-notes/)
