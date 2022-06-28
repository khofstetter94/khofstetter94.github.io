# CRUD

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

- **In your own words, describe what each group of status code represents:** -

        100’s = informational status codes, tells the client that the header part of the request has been recieved and the server will try to comply with a transmission of the clent
        200’s = success codes, the request was accepted
        300’s = redirection codes, the resource that is being requested isnt available at the expected location anymore
        400’s = when the user gives bad data, something is wrong with the user's data
        500’s = server error codes, problems with overwhelmed servers or unreachable servers behind proxies

- **What is a status code 202?** - Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.
- **What is a status code 308?** - Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore.
- **What code would you use if an update didn’t return data to a client?** - 204 No Content
- **What code would you use if a resource used to exist but no longer does?** - 410 Gone
- **What is the ‘Forbidden’ status code?** - 403 Forbidden

- **Why do we need to pull our MongoDB database string out of our server and put it into our .env?** - Because when we deploy our application, we are going to want to use something that is not our local host, so we need to pull it out and into an environment variable
- **What is middleware?** - code thats run once your server gets a request but before it gets passed to any routes
- **What does app.use(express.json()) do?** - lets our server accept JSON as a body instead of a post element or git element or whatever
- **What does the /:id mean in a route?** - this is a parameter, it gives us access to whatever they pass in after the first slash
- **What is the difference between PUT and PATCH?** - PATCH: when updating, we only what to update based on what the user passes us, PUT: updates all of the information of the subscriber all at once
- **How do you make a default value in a schema?** - in your schema constructor, one of the properties would be 'default' and it would be set to something that would populate it with some sort of default data. For example, 'default: Date.now' would default to the current date.
- **What does a 500 error status code mean?** - It means that there is an error on your server, the database caused something not to work and it had nothing to do with the user
- **What is the difference between a status 200 and a status 201?** - 201: successfully created an object/something, 200: everthing was successful

## Things I want to know more about

- What the 'header' part of a request is, using other verbs like PUT and PATCH in our applications, real life examples that would trigger the different error codes

[Return home](https://khofstetter94.github.io/reading-notes/)
