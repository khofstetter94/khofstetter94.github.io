# Express REST API

[Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

- Classes are a template for creating ____.
  - Objects
- Can a class declaration be hoisted?
  - No, classes must be defined before they can be constructed.
- How would you describe a constructor and contextual “this” to a non-technical friend?
  - The constructor method is a special method for creating and initializing an object created with a class. There can only be one special method with the name "constructor" in a class. A constructor basically constructs an object, an object holds key value pairs that give description/details/qualities of a specific instance of the object, and the contextual "this" refers to the specific instance of the object being constructed.

[Using Express Routing](https://expressjs.com/en/guide/routing.html)

- Within Express, what does routing refer to?
  - Routing refers to how an application’s endpoints (URIs) respond to client requests.
- What is the difference between a route path and a route method?
  - A route method is derived from one of the HTTP methods, and is attached to an instance of the express class. Express supports methods that correspond to all HTTP request methods: get, post, and so on. Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.
- When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?
  - You can provide multiple callback functions that behave like middleware to handle a request. The only exception is that these callbacks might invoke next('route') to bypass the remaining route callbacks. You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there’s no reason to proceed with the current route.

[Express Routing](https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4)

- What is an Express Router?
  - It is a mini express application without all the bells and whistles of an express application, just the routing stuff. It doesn’t bring in views or settings but provides us with the routing APIs like .use, .get, .param, and route.
- By what mean do we initialize express.Router() in an express server?
  - Declare a variable and set it to express.Router(), then apply routes to it, and then tell our application to use those routes.
- What do we use route middleware for?
  - Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user.

## Things I want to know more about

- Putting routing into action

[Return home](https://khofstetter94.github.io/reading-notes/)
