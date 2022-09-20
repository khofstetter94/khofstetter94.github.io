# Express, NPM, TDD, CI/CD

[An Introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

- Explain middleware, answer as though I were a non-technical recruiter.
  - Middleware serves as the connection between software and the application. It handles communication and data handling.
- Express the most popular __ __ ____.
  - Node web framework
- Express is “unopinionated.” What does that mean?
  - Unopinionated frameworks, by contrast, have far fewer restrictions on the best way to glue components together to achieve a goal, or even what components should be used. They make it easier for developers to use the most suitable tools to complete a particular task, albeit at the cost that you need to find those components yourself.
- What is a module and why is modularity useful to us as developers?
  - A module is a JavaScript library/file that you can import into other code using Node's require() function. Express itself is a module, as are the middleware and database libraries that we use in our Express applications.

[What is NPM?](https://docs.npmjs.com/about-npm)

- What version of npm are you running on your machine?
  - 8.13.2
- What command would you type to install a library/package called ‘jshint’ into your node project?
  - npm install jshint

[What is TDD](https://www.agilealliance.org/glossary/tdd/)

- Explain why tests are important. Please explain as though I were your non technical elder.
  - You need to test your work for expected outcomes before pushing it to production. You should confirm that your code functions before calling it finished.
- What are three expected benefits of testing
  - Testing will reducde defect rates, which in turn will reduce the effort in the project's final phases. Some have found that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality.
- Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.
  - Two individual pitfalls are forgetting to run tests frequently and writing too many tests at once. Two team pitfalls are partial adoption, where only a few developers on the team use TDD and poor maintenance of the test suite – most commonly leading to a test suite with a prohibitively long running time.

[CI/CD](https://www.youtube.com/watch?v=xSv_m3KhUO8)

- What are three benefits of Continuous Integration?
  - Ensures everyone's changes integrate, catches bugs, and reduces merge conflicts
- What is the difference between Continuos Delivery and Continuous Deployment?
  - Continous delivery is the practice of developing software in such a way that you could release it at any time. When coupled with CI, Continuous delivery lets you develop features with modular code in more manageabe increments. Continuous deployment is an extension of continuous delivery. It's a process that allows you to actually deploy newly developed features into production with confidence, and experience little, if any, downtime.
- Explain how GitHub fits into this process assuming the listener comes from a non-technical background
  - GitHub recieves all the changes completed locally on developer's machines, runs the changes through the CI process and determines if the changes will integrate with the main development branch or if the changes need a little more work before integration.

## Things I want to know more about

- Solving the merge conflicts if and when they occur.

[Return home](https://khofstetter94.github.io/reading-notes/)
