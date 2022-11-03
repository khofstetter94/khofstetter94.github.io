# API Integration

[Review API Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/)

- Explain the different between a query string parameter and a path parameter.
  - Query string parameters extend the URL, the string comes after the '?' and involves key/value pairs, they tell the server what content to deliver. Path parameters are typically used to point to a specific resource within a collection, such as a user identified by ID. A URL can have several path parameters.
- What would our API URL with a path id parameter be given the following information:
  - Domain: 'http://our-site.com'
  - v3
  - model name: stuff
  - id: things
    - 'http://our-site.com/api/v3/stuff/things'
- We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.
  - An application program interface (API) is code that allows two software programs to communicate with each other. An API defines the correct way for a developer to request services from an operating system (OS) or other application, and expose data within different contexts and across multiple channels. [source](<https://www.techtarget.com/searchapparchitecture/definition/application-program-interface-API#:~:text=An%20application%20program%20interface%20(API,contexts%20and%20across%20multiple%20channels/>)

[Review Auth Server Build](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/)

- Describe how you would use middleware to implement basic and bearer auth.
  - The Bearer Auth Middleware provides authentication by verifying an API token in the Request header. Basic auth middleware provides an HTTP basic authentication. For valid credentials it calls the next handler and for missing or invalid credentials, it sends “401 - Unauthorized” response.
- Describe the handshake necessary to implement OAuth.
  - The OAuth processes is initiated in the browser, using a 3rd party authentication/authorization service. It will, once the user has granted permission, invoke a GET on your /oauth route. The OAuth middleware should at this point complete the handshaking process, create/update a local user account in our database, and return an object with a re-authentication/bearer token and the user object
- Describe how Role Based Access Control works to a non-technical friend.
  - An organization assigns a role-based access control role to every employee; the role determines which permissions the system grants to the user. For example, you can designate whether a user is an administrator, a specialist, or an end-user, and limit access to specific resources or tasks. [souce](https://www.imperva.com/learn/data-security/role-based-access-control-rbac/#:~:text=An%20organization%20assigns%20a%20role,to%20specific%20resources%20or%20tasks.)

Reflection

- What are your learning goals after reading and reviewing the class README?
  - I definitely need a refresher on OAuth, maybe just authentication and authorization in general.

[Return home](https://khofstetter94.github.io/reading-notes/)
