# Event Driven Applications

[Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

- What native Node.js module allows us to get started with Event Driven Programming?
  - EventEmitter
- What is the value of Object Oriented Programming used in tandem with Event Driven Programming?
  - The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.
  - By registering event listeners we can actually reverse the flow of communication between our objects. Rather than one object needing to reach inside another object to trigger a function, our objects can just emit events and whichever objects are listening to those event will process it in the way they have been told to.
- Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.
  - Event driven programming in the web browser is useful because the server is built in a way that waits for the user to trigger something and in turn fires off the necessary functions to make it happen. Certain events are tied directly to certain functions which is also helpful for catching bugs.

## Things I want to know more about

- Everything that the EventEmitter provides us that makes EDP easier.

[Return home](https://khofstetter94.github.io/reading-notes/)
