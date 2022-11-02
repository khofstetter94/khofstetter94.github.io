# \<Login /> and \<Auth />

[What is Role Based Access Control (RBAC)?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

- What is Role Based Access Control (RBAC)?
  - Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
- Share some an example of RBAC including all possible CRUD operations and correlating roles.
  - Administrator can CREATE/READ/UPDATE/DELETE, a specialist user can CREATE/READ/UPDATE, or an end-user can READ
- What are the Benefits of RBAC?
  - Reducing administrative work and IT support. Maximizing operational efficiency. Improving compliance.

Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

[react-cookie library](https://www.npmjs.com/package/react-cookie)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

- Describe some react-cookie features.
  - Set the user cookies, Access and modify cookies using React hooks, Let you optionally specify a list of cookie names your component depend on or that should trigger a re-render. If unspecified, it will render on every cookie change, Javascript object with all your cookies - The key is the cookie name, Give access to your cookies anywhere, Your original static properties will be hoisted on the returned component. You can also access the original component by using the WrappedComponent static property, get/getAll/set/remove cookies.
- Describe some react-cookies features.
  - React cookies is the v1.0.4 of react-cookie with a couple changes, To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie. .loadAll() Load all available cookies - returns an object containing all cookies. Use .select([regex]) Find all the cookies with a name that match the regex - returns an object with the cookie name as the key.
- Which library would you prefer would you prefer? Why?
  - I want to say React cookie because it seems easier to use, at least I understand the docs a little better. Interested to see them both in practice..

- Reflection

  - What are your learning goals after reading and reviewing the class README?
    - Using cookies and reviewing Auth because that went right over my head the first time!

[Return home](https://khofstetter94.github.io/reading-notes/)
